# Comparing `tmp/dls-bxflow-2.5.0.tar.gz` & `tmp/dls-bxflow-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-bxflow-2.5.0.tar", last modified: Wed Jun 14 04:47:16 2023, max compression
+gzip compressed data, was "dls-bxflow-2.6.0.tar", last modified: Tue Jun 20 10:03:16 2023, max compression
```

## Comparing `dls-bxflow-2.5.0.tar` & `dls-bxflow-2.6.0.tar`

### file list

```diff
@@ -1,445 +1,448 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.371026 dls-bxflow-2.5.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.359026 dls-bxflow-2.5.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.375026 dls-bxflow-2.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.359026 dls-bxflow-2.5.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/jobs.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.379026 dls-bxflow-2.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14425 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/aiohttp_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.383026 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_launchers/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/bx_launchers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_api/remex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.387026 dls-bxflow-2.5.0/src/dls_bxflow_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.387026 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/dataface_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/news_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.387026 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/execute_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/find_xanes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/fire_i22.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/recipe_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_dcg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_ispyb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/start_services.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/submit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.391026 dls-bxflow-2.5.0/src/dls_bxflow_lib/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-14 04:47:16.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/base_aiohttp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.391026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.391026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gdascan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/bx_composers.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/html.py
--rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/classic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24323 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/bx_databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.395026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    30122 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/explicit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/scandir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40198 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/bx_guis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/curses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.399026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/images/
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
--rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
--rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
--rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
--rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
--rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.403026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
--rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.367025 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
--rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
--rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24839 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/island.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/popener.py
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/qsubber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/slurmer.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.407026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/graylogger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aio_pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/bx_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/pika.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/dask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/boolean.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/bx_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/float.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/integer.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/string.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19775 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/envvar.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/overall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/parser1.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_lib/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.411026 dls-bxflow-2.5.0/src/dls_bxflow_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.415026 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/bx_gates.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/standard.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/states.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.415026 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/execution_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/filename_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/module_classname.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/pickled_class.py
--rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/symlink.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.415026 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/bx_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/src/dls_bxflow_run/main_isolated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base_context_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base_specification_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/base_tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/configurations/
--rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/backend.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/filestore.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/ispyb-local.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/configurations/ptypy_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.419026 dls-bxflow-2.5.0/tests/configurations/ptyrex_configfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/datafiles/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/dawn2_configuration.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.371026 dls-bxflow-2.5.0/tests/datafiles/gaml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow1/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow1/settings.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow2/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/gaml/workflow2/settings.yaml
--rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/datafiles/i22-4996.nxs
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/gda_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/gda_workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/jupyter/
--rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/execute.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/jupyter1.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/jupyter2.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/jupyter_bad_cell.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/jupyter/random_string.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/notebooks/c.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/stub_commands/
--rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/dawn
--rwxr-xr-x   0 runner    (1001) docker     (123)      389 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/mpirun
--rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe
--rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/qstat
--rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/stub_commands/qsub
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_collector_scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dataface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dataface_revision5.py
--rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dawn1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_dawn2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_extract_error_lines_dawn.py
--rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_extract_error_lines_dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_filestore.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_gaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_a.py
--rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_a_bc_d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_pubcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_job_x.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_capacity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_direct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_multiple.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_launcher_restart.py
--rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_logstore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_news.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_protocolj.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_ptypy_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_ptyrex_mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_scheduler_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/test_workflow_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/a/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/a/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/b/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/b/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/b/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/c/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/c/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/c/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/e/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/e/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.423026 dls-bxflow-2.5.0/tests/workflows/f/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/f/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/f/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:16.427026 dls-bxflow-2.5.0/tests/workflows/g/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/g/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/g/workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-14 04:47:05.000000 dls-bxflow-2.5.0/tests/workflows/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.118254 dls-bxflow-2.6.0/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.118254 dls-bxflow-2.6.0/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.110254 dls-bxflow-2.6.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     6913 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2083 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.110254 dls-bxflow-2.6.0/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6752 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/explanations/jobs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.122254 dls-bxflow-2.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.114254 dls-bxflow-2.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-06-20 10:03:16.000000 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14520 2023-06-20 10:03:16.000000 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 10:03:16.000000 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-20 10:03:16.000000 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-20 10:03:16.000000 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 10:03:16.000000 dls-bxflow-2.6.0/src/dls_bxflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/aiohttp_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_databases/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13706 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/bx_launchers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_api/remex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.126254 dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/dataface_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/news_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6648 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.130254 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/execute_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/find_xanes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/fire_i22.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/recipe_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7339 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/report_dcg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/report_ispyb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5079 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/start_services.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/submit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.130254 dls-bxflow-2.6.0/src/dls_bxflow_lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 10:03:15.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/base_aiohttp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.130254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16313 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.130254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/gdascan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/bx_composers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10921 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8348 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_configurators/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_configurators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17729 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/classic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_databases/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24323 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_databases/bx_databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30122 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7487 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/scandir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.134254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40198 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/bx_guis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/curses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/system_health_ux.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png
+-rw-r--r--   0 runner    (1001) docker     (123)   105264 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10939 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/events.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4732 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/page.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5981 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10690 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/version.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/dls_common/base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.114254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.138254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    89501 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.114254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.142254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30801 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   255077 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.114254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.142254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.142254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_dadada_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7111 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (123)    18024 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.142254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/
+-rw-r--r--   0 runner    (1001) docker     (123)     5370 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/runtime.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.142254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8655 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.146254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11327 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24839 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/island.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/popener.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/qsubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/slurmer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.146254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7876 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/graylogger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.146254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/aio_pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6888 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/bx_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/pika.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.146254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10234 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.150254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/bx_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/float.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/string.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.150254 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19775 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.150254 dls-bxflow-2.6.0/src/dls_bxflow_lib/dummies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/dummies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/dummies/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/envvar.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.150254 dls-bxflow-2.6.0/src/dls_bxflow_lib/recipe_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/recipe_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/recipe_parser/overall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/recipe_parser/parser1.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_lib/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.150254 dls-bxflow-2.6.0/src/dls_bxflow_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.150254 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2995 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/bx_gates.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/standard.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/states.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.154254 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4790 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7562 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dawn_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/execution_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/filename_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/module_classname.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/pickled_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16811 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15845 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/ptyrex_srun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6071 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/symlink.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.154254 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_variables/bx_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_variables/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/bx_variables/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8529 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/src/dls_bxflow_run/main_isolated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.158254 dls-bxflow-2.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/base_context_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/base_specification_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/base_tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.158254 dls-bxflow-2.6.0/tests/configurations/
+-rw-r--r--   0 runner    (1001) docker     (123)    13245 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/configurations/backend.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/configurations/filestore.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/configurations/ispyb-local.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.158254 dls-bxflow-2.6.0/tests/configurations/ptypy_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.158254 dls-bxflow-2.6.0/tests/configurations/ptyrex_configfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.158254 dls-bxflow-2.6.0/tests/datafiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/datafiles/dawn2_configuration.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.118254 dls-bxflow-2.6.0/tests/datafiles/gaml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/datafiles/gaml/workflow1/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/datafiles/gaml/workflow1/settings.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/datafiles/gaml/workflow2/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/datafiles/gaml/workflow2/settings.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)  1105944 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/datafiles/i22-4996.nxs
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/gda_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/gda_workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/jupyter/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      207 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/jupyter/execute.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/jupyter/jupyter1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/jupyter/jupyter2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/jupyter/jupyter_bad_cell.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/jupyter/random_string.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/notebooks/c.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/stub_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/dawn
+-rwxr-xr-x   0 runner    (1001) docker     (123)      561 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/mpirun
+-rwxr-xr-x   0 runner    (1001) docker     (123)       47 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/nvidia-smi
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1407 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6186 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/qstat
+-rwxr-xr-x   0 runner    (1001) docker     (123)      511 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/qsub
+-rwxr-xr-x   0 runner    (1001) docker     (123)      352 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/stub_commands/srun
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10613 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5437 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_collector_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_dataface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_dataface_revision5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6451 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_dawn1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_dawn2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_extract_error_lines_dawn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_extract_error_lines_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_filestore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_gaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_job_a.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12275 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_job_a_bc_d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7991 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_job_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_job_pubcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_job_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13021 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_launcher_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8546 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_launcher_direct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_launcher_multiple.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_launcher_restart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_logstore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_protocolj.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_ptypy_mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8424 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_ptyrex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_scheduler_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5861 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7501 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5253 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3989 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/test_workflow_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.162254 dls-bxflow-2.6.0/tests/workflows/a/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/a/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/tests/workflows/b/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/b/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/b/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/tests/workflows/c/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/c/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/c/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/tests/workflows/e/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/e/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/tests/workflows/f/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/f/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/f/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:16.166254 dls-bxflow-2.6.0/tests/workflows/g/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/g/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/g/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-20 10:03:06.000000 dls-bxflow-2.6.0/tests/workflows/utilities.py
```

### Comparing `dls-bxflow-2.5.0/.dae-devops/Makefile` & `dls-bxflow-2.6.0/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/conventions.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/developing.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/devops.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/docs_structure.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/documenting.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/installing.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/docs/testing.rst` & `dls-bxflow-2.6.0/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.dae-devops/project.yaml` & `dls-bxflow-2.6.0/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.devcontainer/Dockerfile` & `dls-bxflow-2.6.0/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.devcontainer/devcontainer.json` & `dls-bxflow-2.6.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/CONTRIBUTING.rst` & `dls-bxflow-2.6.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/actions/install_requirements/action.yml` & `dls-bxflow-2.6.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/dependabot.yml` & `dls-bxflow-2.6.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/pages/index.html` & `dls-bxflow-2.6.0/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/pages/make_switcher.py` & `dls-bxflow-2.6.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/workflows/code.yml` & `dls-bxflow-2.6.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/workflows/docs.yml` & `dls-bxflow-2.6.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/workflows/docs_clean.yml` & `dls-bxflow-2.6.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.github/workflows/linkcheck.yml` & `dls-bxflow-2.6.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.gitignore` & `dls-bxflow-2.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.gitlab-ci.yml` & `dls-bxflow-2.6.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/.vscode/launch.json` & `dls-bxflow-2.6.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/LICENSE` & `dls-bxflow-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/PKG-INFO` & `dls-bxflow-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.5.0
+Version: 2.6.0
 Summary: Distributed beamline automated data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-2.5.0/docs/conf.py` & `dls-bxflow-2.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/docs/explanations/jobs.rst` & `dls-bxflow-2.6.0/docs/explanations/jobs.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/docs/explanations/todo.rst` & `dls-bxflow-2.6.0/docs/explanations/todo.rst`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/docs/images/dls-favicon.ico` & `dls-bxflow-2.6.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/docs/images/dls-logo.svg` & `dls-bxflow-2.6.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/pyproject.toml` & `dls-bxflow-2.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow.egg-info/PKG-INFO` & `dls-bxflow-2.6.0/src/dls_bxflow.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-bxflow
-Version: 2.5.0
+Version: 2.6.0
 Summary: Distributed beamline automated data processing workflow engine and gui platform core.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow.egg-info/SOURCES.txt` & `dls-bxflow-2.6.0/src/dls_bxflow.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -264,14 +264,15 @@
 src/dls_bxflow_run/bx_tasks/execution_summary.py
 src/dls_bxflow_run/bx_tasks/filename_classname.py
 src/dls_bxflow_run/bx_tasks/jupyter.py
 src/dls_bxflow_run/bx_tasks/module_classname.py
 src/dls_bxflow_run/bx_tasks/pickled_class.py
 src/dls_bxflow_run/bx_tasks/ptypy_mpi.py
 src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py
+src/dls_bxflow_run/bx_tasks/ptyrex_srun.py
 src/dls_bxflow_run/bx_tasks/shell.py
 src/dls_bxflow_run/bx_tasks/states.py
 src/dls_bxflow_run/bx_tasks/symlink.py
 src/dls_bxflow_run/bx_variables/__init__.py
 src/dls_bxflow_run/bx_variables/bx_variables.py
 src/dls_bxflow_run/bx_variables/simple.py
 src/dls_bxflow_run/bx_variables/states.py
@@ -309,15 +310,15 @@
 tests/test_launcher_direct.py
 tests/test_launcher_multiple.py
 tests/test_launcher_restart.py
 tests/test_logstore.py
 tests/test_news.py
 tests/test_protocolj.py
 tests/test_ptypy_mpi.py
-tests/test_ptyrex_mpi.py
+tests/test_ptyrex.py
 tests/test_scheduler_naive.py
 tests/test_settings.py
 tests/test_shell.py
 tests/test_task.py
 tests/test_workflow.py
 tests/test_workflow_finder.py
 tests/configurations/backend.yaml
@@ -333,17 +334,19 @@
 tests/jupyter/jupyter1.ipynb
 tests/jupyter/jupyter2.ipynb
 tests/jupyter/jupyter_bad_cell.ipynb
 tests/jupyter/random_string.png
 tests/notebooks/c.ipynb
 tests/stub_commands/dawn
 tests/stub_commands/mpirun
+tests/stub_commands/nvidia-smi
 tests/stub_commands/ptychotools.ptypy_mpi_recipe
 tests/stub_commands/qstat
 tests/stub_commands/qsub
+tests/stub_commands/srun
 tests/task_classes/task_z.py
 tests/workflows/__init__.py
 tests/workflows/base.py
 tests/workflows/utilities.py
 tests/workflows/a/__init__.py
 tests/workflows/a/workflow.py
 tests/workflows/b/__init__.py
```

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow.egg-info/requires.txt` & `dls-bxflow-2.6.0/src/dls_bxflow.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_databases/constants.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/bx_databases/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_datafaces/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/bx_launchers/constants.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/bx_launchers/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/exceptions.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_api/remex.py` & `dls-bxflow-2.6.0/src/dls_bxflow_api/remex.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     MEMORY_LIMIT = "m_mem_free"
     TIME_LIMIT = "h_rt"
     QUEUE = "q"
     PARALLEL_ENVIRONMENT = "pe"
     GPU = "gpu"
     GPU_ARCH = "gpu_arch"
     HOST = "host"
+    # When slurm is there, the it contains native slurm JobProperties keywords.
+    SLURM_JOB_PROPERTIES = "slurm_job_properties"
 
 
 class Clusters:
     HAMILTON = "dls_bxflow_api::remex::cluster::hamilton"
     SCIENCE = "dls_bxflow_api::remex::cluster::global/cluster"
     SLURM = "dls_bxflow_api::remex::cluster::slurm"
     TEST = "dls_bxflow_api::remex::cluster::global/testcluster"
```

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/dataface_client.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/dataface_client.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/filestore.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/contexts/news_consumer.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/contexts/news_consumer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/main.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/execute_workflow.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/execute_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/find_xanes.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/find_xanes.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/fire_i22.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/fire_i22.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/recipe_parser.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/recipe_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_dcg.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/report_dcg.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/report_ispyb.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/report_ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/start_services.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/start_services.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/subcommands/submit.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/subcommands/submit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_cli/version.py` & `dls-bxflow-2.6.0/src/dls_bxflow_cli/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/__main__.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/bx_catalogs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_catalogs/ispyb.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/bx_collectors.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/gda_parser_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/gdascan.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/gdascan.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/manual.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/manual.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_collectors/scraper.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_collectors/scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/bx_composers.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/bx_composers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/html.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/prettyhelper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_composers/text.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_composers/text.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_configurators/bx_configurators.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/bx_contexts.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_contexts/classic.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_contexts/classic.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_databases/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_databases/bx_databases.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_databases/bx_databases.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/aiosqlite.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/bx_datafaces.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_datafaces/news_producer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/bx_filestores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/explicit.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/explicit.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_filestores/scandir.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_filestores/scandir.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/bx_gamls.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_gamls/html.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_gamls/html.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/bx_guis.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/bx_guis.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/constants.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/curses.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/curses.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/images/dls_logo_50x50.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/job_data_grid_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/job_details_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/job_submit_ux.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/css/styles.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/images/green_dot_crosshair.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/images/radial1.666.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/index.html` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/index.html`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_data_grid_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_details_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_news_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_submit_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/job_variables_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/recent_jobs_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/system_health_ux.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/tabs_manager.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_auto_update.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/bxflow/ux_base.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/index.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jquery/3.6.0/jquery.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/jqueryui/1.13.1/themes/smoothness/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_guis/html/javascript/protocolj/client.js`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/bx_jobs.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_jobs/standard.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_jobs/standard.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/bx_launchers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/island.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/island.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/popener.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/popener.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/qsubber.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/qsubber.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_launchers/slurmer.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_launchers/slurmer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/bx_logstores.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_logstores/graylogger.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_logstores/graylogger.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aio_pika.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/aio_pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/bx_news.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/bx_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/constants.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/constants.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/pika.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/pika.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_news/zmq_pubsub.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/bx_schedulers.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/context.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/context.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/dask.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/dask.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/naive.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_schedulers/zocalo.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/boolean.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/boolean.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/bx_settings.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/bx_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/float.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/float.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/integer.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/integer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_settings/string.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_settings/string.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/main.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/main.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/notebook_helper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/bx_workflows/workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/dummies/writer.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/dummies/writer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/envvar.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/overall.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/recipe_parser/overall.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/recipe_parser/parser1.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/recipe_parser/parser1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_lib/version.py` & `dls-bxflow-2.6.0/src/dls_bxflow_lib/version.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_gates/bx_gates.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_gates/bx_gates.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/bx_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,19 @@
             return PtypyMpi
 
         if class_type == BxTaskTypes.PTYREX_MPI:
             from dls_bxflow_run.bx_tasks.ptyrex_mpi import PtyrexMpi
 
             return PtyrexMpi
 
+        if class_type == BxTaskTypes.PTYREX_SRUN:
+            from dls_bxflow_run.bx_tasks.ptyrex_srun import PtyrexSrun
+
+            return PtyrexSrun
+
         if class_type == "dls_bxflow_run.bx_tasks.shell":
             from dls_bxflow_run.bx_tasks.shell import Shell
 
             return Shell
 
         raise NotFound("unable to get bx_task class for %s" % (class_type))
```

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/constants.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/constants.py`

 * *Files 21% similar despite different names*

```diff
@@ -14,7 +14,8 @@
     DUMMY = "dls_bxflow_run.bx_tasks.dummy"
     SYMLINK = "dls_bxflow_run.bx_tasks.symlink"
     JUPYTER = "dls_bxflow_run.bx_tasks.jupyter"
     FILENAME_CLASSNAME = "dls_bxflow_run.bx_tasks.filename_classname"
     MODULE_CLASSNAME = "dls_bxflow_run.bx_tasks.module_classname"
     PTYPY_MPI = "dls_bxflow_run.bx_tasks.ptypy_mpi"
     PTYREX_MPI = "dls_bxflow_run.bx_tasks.ptyrex_mpi"
+    PTYREX_SRUN = "dls_bxflow_run.bx_tasks.ptyrex_srun"
```

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn1.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn2.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dawn_base.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dawn_base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/dummy.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/execution_summary.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/execution_summary.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/filename_classname.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/filename_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/jupyter.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/module_classname.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/module_classname.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/pickled_class.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/pickled_class.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/ptyrex_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/shell.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_tasks/symlink.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_tasks/symlink.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/bx_variables/bx_variables.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/bx_variables/bx_variables.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/src/dls_bxflow_run/main_isolated.py` & `dls-bxflow-2.6.0/src/dls_bxflow_run/main_isolated.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/base.py` & `dls-bxflow-2.6.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/base_context_tester.py` & `dls-bxflow-2.6.0/tests/base_context_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/base_specification_tester.py` & `dls-bxflow-2.6.0/tests/base_specification_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/base_tester.py` & `dls-bxflow-2.6.0/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/configurations/backend.yaml` & `dls-bxflow-2.6.0/tests/configurations/backend.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/configurations/filestore.yaml` & `dls-bxflow-2.6.0/tests/configurations/filestore.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml` & `dls-bxflow-2.6.0/tests/configurations/ptypy_configfiles/i14_unknown_probe_dm.yaml`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json` & `dls-bxflow-2.6.0/tests/configurations/ptyrex_configfiles/region_p4_p6.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/conftest.py` & `dls-bxflow-2.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/datafiles/dawn2_configuration.json` & `dls-bxflow-2.6.0/tests/datafiles/dawn2_configuration.json`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/datafiles/i22-4996.nxs` & `dls-bxflow-2.6.0/tests/datafiles/i22-4996.nxs`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/gda_parser.py` & `dls-bxflow-2.6.0/tests/gda_parser.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/gda_workflow.py` & `dls-bxflow-2.6.0/tests/gda_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/jupyter/jupyter1.ipynb` & `dls-bxflow-2.6.0/tests/jupyter/jupyter1.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/jupyter/jupyter2.ipynb` & `dls-bxflow-2.6.0/tests/jupyter/jupyter2.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/jupyter/jupyter_bad_cell.ipynb` & `dls-bxflow-2.6.0/tests/jupyter/jupyter_bad_cell.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/jupyter/random_string.png` & `dls-bxflow-2.6.0/tests/jupyter/random_string.png`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/notebooks/c.ipynb` & `dls-bxflow-2.6.0/tests/notebooks/c.ipynb`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe` & `dls-bxflow-2.6.0/tests/stub_commands/ptychotools.ptypy_mpi_recipe`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/stub_commands/qstat` & `dls-bxflow-2.6.0/tests/stub_commands/qstat`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_catalog.py` & `dls-bxflow-2.6.0/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_collector.py` & `dls-bxflow-2.6.0/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_collector_scraper.py` & `dls-bxflow-2.6.0/tests/test_collector_scraper.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_composer.py` & `dls-bxflow-2.6.0/tests/test_composer.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_configurator.py` & `dls-bxflow-2.6.0/tests/test_configurator.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_database.py` & `dls-bxflow-2.6.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_dataface.py` & `dls-bxflow-2.6.0/tests/test_dataface.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_dataface_revision5.py` & `dls-bxflow-2.6.0/tests/test_dataface_revision5.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_dawn1.py` & `dls-bxflow-2.6.0/tests/test_dawn1.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_dawn2.py` & `dls-bxflow-2.6.0/tests/test_dawn2.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_extract_error_lines_dawn.py` & `dls-bxflow-2.6.0/tests/test_extract_error_lines_dawn.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_extract_error_lines_dummy.py` & `dls-bxflow-2.6.0/tests/test_extract_error_lines_dummy.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_filestore.py` & `dls-bxflow-2.6.0/tests/test_filestore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_gaml.py` & `dls-bxflow-2.6.0/tests/test_gaml.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_gui.py` & `dls-bxflow-2.6.0/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_job_a.py` & `dls-bxflow-2.6.0/tests/test_job_a.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_job_a_bc_d.py` & `dls-bxflow-2.6.0/tests/test_job_a_bc_d.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_job_notebook.py` & `dls-bxflow-2.6.0/tests/test_job_notebook.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_job_pubcon.py` & `dls-bxflow-2.6.0/tests/test_job_pubcon.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_job_x.py` & `dls-bxflow-2.6.0/tests/test_job_x.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_jupyter.py` & `dls-bxflow-2.6.0/tests/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_launcher.py` & `dls-bxflow-2.6.0/tests/test_launcher.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_launcher_capacity.py` & `dls-bxflow-2.6.0/tests/test_launcher_capacity.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_launcher_direct.py` & `dls-bxflow-2.6.0/tests/test_launcher_direct.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_launcher_multiple.py` & `dls-bxflow-2.6.0/tests/test_launcher_multiple.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_launcher_restart.py` & `dls-bxflow-2.6.0/tests/test_launcher_restart.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_logstore.py` & `dls-bxflow-2.6.0/tests/test_logstore.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_news.py` & `dls-bxflow-2.6.0/tests/test_news.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_protocolj.py` & `dls-bxflow-2.6.0/tests/test_protocolj.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_ptypy_mpi.py` & `dls-bxflow-2.6.0/tests/test_ptypy_mpi.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_ptyrex_mpi.py` & `dls-bxflow-2.6.0/tests/test_ptyrex.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import logging
 import os
 
-import pytest
-
 # Utilities.
 from dls_utilpack.describe import describe
 from dls_utilpack.module import module_use
 
 # Remote execution.
 from dls_bxflow_api.remex import Clusters as RemexClusters
 from dls_bxflow_api.remex import Keywords as RemexKeywords
@@ -23,17 +21,14 @@
 # Base class for the tester.
 from tests.base_context_tester import BaseContextTester
 
 logger = logging.getLogger(__name__)
 
 
 # ----------------------------------------------------------------------------------------
-
-
-@pytest.mark.skipif("not config.getoption('gpu')")
 class TestPtyrexMpiGood:
     def test(self, constants, logging_setup, output_directory):
         """
         Tests that a ptyrex_mpi task can be run.
         """
 
         ptyrex_configfile = f"{os.path.dirname(__file__)}/configurations/ptyrex_configfiles/region_p4_p6.json"
@@ -62,23 +57,67 @@
                     "directories": [output_directory],
                     "modules": ["my_ptyrex_module"],
                 },
             },
         }
 
         configuration_file = "tests/configurations/filestore.yaml"
-        PtyrexMpiTester(task_specification).main(
+        PtyrexTester(task_specification).main(
+            constants,
+            configuration_file,
+            output_directory,
+        )
+
+
+# ----------------------------------------------------------------------------------------
+class TestPtyrexSrunGood:
+    def test(self, constants, logging_setup, output_directory):
+        """
+        Tests that a ptyrex_srun task can be run.
+        """
+
+        ptyrex_configfile = f"{os.path.dirname(__file__)}/configurations/ptyrex_configfiles/region_p4_p6.json"
+        ptyrex_configfile_updated_fields = {}
+        ptyrex_configfile_substitutions = {}
+
+        # The data filename is checked by the task, so it must exist.
+        data_filename = f"{output_directory}/some_data.hdf5"
+        with open(data_filename, "w") as stream:
+            stream.write("")
+
+        task_specification = {
+            "type": BxTaskTypes.PTYREX_SRUN,
+            "label": "my_ptyrex_srun",
+            "remex_hints": {
+                RemexKeywords.CLUSTER: RemexClusters.LOCAL,
+                RemexKeywords.SLURM_JOB_PROPERTIES: {},
+            },
+            "type_specific_tbd": {
+                "data_filename": data_filename,
+                "ptyrex_configfile": ptyrex_configfile,
+                "ptyrex_configfile_updated_fields": ptyrex_configfile_updated_fields,
+                "ptyrex_configfile_substitutions": ptyrex_configfile_substitutions,
+                # The pytrex_srun will run in a script in which these modules are loaded.
+                "load_modules": {
+                    "directories": [output_directory],
+                    "modules": ["my_ptyrex_module"],
+                },
+            },
+        }
+
+        configuration_file = "tests/configurations/filestore.yaml"
+        PtyrexTester(task_specification).main(
             constants,
             configuration_file,
             output_directory,
         )
 
 
 # ----------------------------------------------------------------------------------------
-class PtyrexMpiTester(BaseContextTester):
+class PtyrexTester(BaseContextTester):
     """
     Test the ptyrex_mpi task.
     """
 
     def __init__(
         self,
         task_specification,
@@ -94,56 +133,87 @@
         # This module will set the PATH to include the stub_commands directory,
         # in which there will be a dummy mpirun command.
         with open(f"{output_directory}/my_ptyrex_module", "w") as stream:
             stream.write("#%Module1.0\n")
             stream.write(
                 f"setenv  PATH my_good_path1:my_good_path2:{os.path.dirname(__file__)}/stub_commands:{os.environ['PATH']}\n"
             )
+            stream.write('puts stderr "my_ptyrex_module: some blather to stderr"\n')
 
         # Make sure there is at least a stderr.txt for extract_error_lines
         # to look in if there is no ptyrex_mpi_stderr.txt.
-        with open(f"{output_directory}/stderr.txt", "w") as stream:
-            stream.write("")
+        # with open(f"{output_directory}/stderr.txt", "w") as stream:
+        #     stream.write("")
 
         os.environ.update(module_use(output_directory))
 
         # --------------------------------------------------------------------
 
         os.makedirs(f"{output_directory}/.bxflow")
         original_directory = os.getcwd()
 
         bx_configurator = self.get_bx_configurator()
         specification = await bx_configurator.load()
         # Remex hints for task type.
-        specification["bx_task_remex_hints"] = {BxTaskTypes.PTYREX_MPI: {}}
+        specification["bx_task_remex_hints"] = {
+            BxTaskTypes.PTYREX_MPI: {},
+            BxTaskTypes.PTYREX_SRUN: {},
+        }
 
         bx_context = BxContexts().build_object(specification)
 
         async with bx_context:
             try:
                 os.chdir(output_directory)
 
                 # Define the class and its constructor arguments.
                 bx_task = BxTasks().build_object(self.__task_specification)
                 bx_task.set_directory(output_directory)
 
                 return_code = await bx_task.run()
 
+                self.__debug_files(output_directory)
+
                 if self.__expected_script_error is None:
+                    if return_code != 0:
+                        error_lines = bx_task.extract_error_lines()
+                        logger.debug(describe("error_lines", error_lines))
                     assert return_code == 0
                     error_lines = bx_task.extract_error_lines()
                     assert isinstance(error_lines, list)
                     assert len(error_lines) == 0
 
                     # TODO: In test_ptyrex_mpi, check the yaml file to make sure the visit.directory is replaced.
-                    assert os.path.exists(f"{output_directory}/ptyrex_configfile.yaml")
+                    assert os.path.exists(f"{output_directory}/ptyrex_configfile.json")
                 else:
                     # assert return_code != 0
                     error_lines = bx_task.extract_error_lines()
                     logger.debug(describe("error_lines", error_lines))
                     assert isinstance(error_lines, list)
                     assert len(error_lines) == 2
                     assert self.__expected_script_error in error_lines[0]
                     assert error_lines[1].startswith("for more")
 
             finally:
                 os.chdir(original_directory)
+
+    def __debug_files(self, output_directory):
+        files = [
+            "ptyrex_mpi.sh",
+            "ptyrex_mpi_stderr.txt",
+            "ptyrex_mpi_stdout.txt",
+            "ptyrex_srun.sh",
+            "ptyrex_srun_stderr.txt",
+            "ptyrex_srun_stdout.txt",
+        ]
+
+        for file in files:
+            self.__debug_file(f"{output_directory}/{file}")
+
+    def __debug_file(self, file):
+
+        if os.path.exists(file):
+            with open(file, "r") as stream:
+                lines = stream.readlines()
+            logger.debug(describe(file, lines))
+        else:
+            logger.debug(f"no file {file}")
```

### Comparing `dls-bxflow-2.5.0/tests/test_scheduler_naive.py` & `dls-bxflow-2.6.0/tests/test_scheduler_naive.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_settings.py` & `dls-bxflow-2.6.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_shell.py` & `dls-bxflow-2.6.0/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_task.py` & `dls-bxflow-2.6.0/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_workflow.py` & `dls-bxflow-2.6.0/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/test_workflow_finder.py` & `dls-bxflow-2.6.0/tests/test_workflow_finder.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/a/workflow.py` & `dls-bxflow-2.6.0/tests/workflows/a/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/b/workflow.py` & `dls-bxflow-2.6.0/tests/workflows/b/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/base.py` & `dls-bxflow-2.6.0/tests/workflows/base.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/c/workflow.py` & `dls-bxflow-2.6.0/tests/workflows/c/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/e/workflow.py` & `dls-bxflow-2.6.0/tests/workflows/e/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/f/workflow.py` & `dls-bxflow-2.6.0/tests/workflows/f/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/g/workflow.py` & `dls-bxflow-2.6.0/tests/workflows/g/workflow.py`

 * *Files identical despite different names*

### Comparing `dls-bxflow-2.5.0/tests/workflows/utilities.py` & `dls-bxflow-2.6.0/tests/workflows/utilities.py`

 * *Files identical despite different names*

