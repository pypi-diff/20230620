# Comparing `tmp/dls-utilpack-1.6.0.tar.gz` & `tmp/dls-utilpack-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-utilpack-1.6.0.tar", last modified: Mon Jun  5 16:58:46 2023, max compression
+gzip compressed data, was "dls-utilpack-1.6.1.tar", last modified: Tue Jun 20 08:20:47 2023, max compression
```

## Comparing `dls-utilpack-1.6.0.tar` & `dls-utilpack-1.6.1.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/.dae-devops/
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.dae-devops/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/docs/testing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/prepare_git_dependencies.sh
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.dae-devops/project.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/pages/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/_static/css/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/explanations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/conventions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/docs_structure.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/explanations/todo.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/how-to/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/developing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/devops.rst
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/documenting.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/installing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/how-to/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.594851 dls-utilpack-1.6.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.598851 dls-utilpack-1.6.0/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/classes.rst
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/command_line.rst
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/reference/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.598851 dls-utilpack-1.6.0/docs/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/docs/tutorials/tbd.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.590851 dls-utilpack-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.598851 dls-utilpack-1.6.0/src/dls_utilpack/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7015 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/client_context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/describe.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/envvar.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/global_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/import_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/isodatetime.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/modify_process_title.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/qualname.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/require.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/search_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/server_context_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/things.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/visit.py
--rw-r--r--   0 runner    (1001) docker     (123)     4774 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/src/dls_utilpack/whatenv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 16:58:46.000000 dls-utilpack-1.6.0/src/dls_utilpack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/base_tester.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:58:46.602851 dls-utilpack-1.6.0/tests/task_classes/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/task_classes/task_z.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_bash_composer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_callsign.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_hazzathread.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_sanitize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_server_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_sigint1.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_sigint2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_substitute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_visit.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-05 16:58:37.000000 dls-utilpack-1.6.0/tests/test_whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.772351 dls-utilpack-1.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.752349 dls-utilpack-1.6.1/.dae-devops/
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.752349 dls-utilpack-1.6.1/.dae-devops/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/docs/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/prepare_git_dependencies.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.dae-devops/project.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     1624 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.748349 dls-utilpack-1.6.1/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/pages/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3273 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-20 08:20:47.772351 dls-utilpack-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.748349 dls-utilpack-1.6.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/docs/_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/_static/css/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6738 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.756350 dls-utilpack-1.6.1/docs/explanations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/explanations/conventions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/explanations/docs_structure.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/explanations/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/explanations/todo.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.760350 dls-utilpack-1.6.1/docs/how-to/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/how-to/developing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/how-to/devops.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/how-to/documenting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/how-to/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/how-to/installing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/how-to/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.760350 dls-utilpack-1.6.1/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    99678 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.760350 dls-utilpack-1.6.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/reference/classes.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/reference/command_line.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/reference/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.760350 dls-utilpack-1.6.1/docs/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/docs/tutorials/tbd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:20:47.772351 dls-utilpack-1.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.752349 dls-utilpack-1.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.764350 dls-utilpack-1.6.1/src/dls_utilpack/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/client_context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/describe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/envvar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/global_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/import_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/isodatetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/modify_process_title.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/qualname.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/require.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/search_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/server_context_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/things.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/src/dls_utilpack/whatenv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.768350 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13910 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-20 08:20:47.000000 dls-utilpack-1.6.1/src/dls_utilpack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.768350 dls-utilpack-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/base_tester.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:20:47.772351 dls-utilpack-1.6.1/tests/task_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/task_classes/task_z.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_bash_composer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_callsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_hazzathread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_sanitize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_server_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_sigint1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_sigint2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_substitute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_visit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-20 08:20:35.000000 dls-utilpack-1.6.1/tests/test_whatenv.py
```

### Comparing `dls-utilpack-1.6.0/.dae-devops/Makefile` & `dls-utilpack-1.6.1/.dae-devops/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/conventions.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/conventions.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/developing.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/developing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/devops.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/devops.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/docs_structure.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/docs_structure.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/documenting.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/documenting.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/installing.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/docs/testing.rst` & `dls-utilpack-1.6.1/.dae-devops/docs/testing.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.dae-devops/project.yaml` & `dls-utilpack-1.6.1/.dae-devops/project.yaml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.devcontainer/Dockerfile` & `dls-utilpack-1.6.1/.devcontainer/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.devcontainer/devcontainer.json` & `dls-utilpack-1.6.1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/CONTRIBUTING.rst` & `dls-utilpack-1.6.1/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/actions/install_requirements/action.yml` & `dls-utilpack-1.6.1/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/dependabot.yml` & `dls-utilpack-1.6.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/pages/index.html` & `dls-utilpack-1.6.1/.github/pages/index.html`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/pages/make_switcher.py` & `dls-utilpack-1.6.1/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/workflows/code.yml` & `dls-utilpack-1.6.1/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/workflows/docs.yml` & `dls-utilpack-1.6.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/workflows/docs_clean.yml` & `dls-utilpack-1.6.1/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.github/workflows/linkcheck.yml` & `dls-utilpack-1.6.1/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.gitignore` & `dls-utilpack-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.gitlab-ci.yml` & `dls-utilpack-1.6.1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/.vscode/launch.json` & `dls-utilpack-1.6.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/LICENSE` & `dls-utilpack-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/Makefile` & `dls-utilpack-1.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/PKG-INFO` & `dls-utilpack-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.6.0
+Version: 1.6.1
 Summary: Library of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-utilpack-1.6.0/docs/conf.py` & `dls-utilpack-1.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/docs/images/dls-favicon.ico` & `dls-utilpack-1.6.1/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/docs/images/dls-logo.svg` & `dls-utilpack-1.6.1/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/docs/reference/modules.rst` & `dls-utilpack-1.6.1/docs/reference/modules.rst`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/pyproject.toml` & `dls-utilpack-1.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/__main__.py` & `dls-utilpack-1.6.1/src/dls_utilpack/__main__.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/bash_composer.py` & `dls-utilpack-1.6.1/src/dls_utilpack/bash_composer.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 class Print(Element):
     def __init__(self, message):
         self.__message = message
 
     def compose(self) -> List[str]:
         lines = []
 
+        lines.append("")
         lines.append(f"eval echo '{self.__message}'")
 
         return lines
 
 
 # ---------------------------------------------------------------------
 class LoadModules(Element):
@@ -115,15 +116,15 @@
             composer.add(Command(f"module use --append {directory}"))
 
         for module in self.__modules:
             composer.add(Command(f"module load {module} 2>&1"))
 
         # Put a few things in the log.
         composer.add(Command("module list 2>&1"))
-        composer.add(Command("python --version"))
+        composer.add(Command("python3 --version"))
         composer.add(Print("------ end of modules_load_bash_lines ------"))
 
         return composer.compose_lines()
 
 
 # ---------------------------------------------------------------------
 class BashComposer:
```

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/callsign.py` & `dls-utilpack-1.6.1/src/dls_utilpack/callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/client_context_base.py` & `dls-utilpack-1.6.1/src/dls_utilpack/client_context_base.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/datatypes.py` & `dls-utilpack-1.6.1/src/dls_utilpack/datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/describe.py` & `dls-utilpack-1.6.1/src/dls_utilpack/describe.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/envvar.py` & `dls-utilpack-1.6.1/src/dls_utilpack/envvar.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/exceptions.py` & `dls-utilpack-1.6.1/src/dls_utilpack/exceptions.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/explain.py` & `dls-utilpack-1.6.1/src/dls_utilpack/explain.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/hazzathread.py` & `dls-utilpack-1.6.1/src/dls_utilpack/hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/ignore.py` & `dls-utilpack-1.6.1/src/dls_utilpack/ignore.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/import_class.py` & `dls-utilpack-1.6.1/src/dls_utilpack/import_class.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/module.py` & `dls-utilpack-1.6.1/src/dls_utilpack/module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/profiler.py` & `dls-utilpack-1.6.1/src/dls_utilpack/profiler.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/require.py` & `dls-utilpack-1.6.1/src/dls_utilpack/require.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/sanitize.py` & `dls-utilpack-1.6.1/src/dls_utilpack/sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/search_file.py` & `dls-utilpack-1.6.1/src/dls_utilpack/search_file.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/server_context_base.py` & `dls-utilpack-1.6.1/src/dls_utilpack/server_context_base.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/signal.py` & `dls-utilpack-1.6.1/src/dls_utilpack/signal.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/substitute.py` & `dls-utilpack-1.6.1/src/dls_utilpack/substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/thing.py` & `dls-utilpack-1.6.1/src/dls_utilpack/thing.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/things.py` & `dls-utilpack-1.6.1/src/dls_utilpack/things.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/version.py` & `dls-utilpack-1.6.1/src/dls_utilpack/version.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/visit.py` & `dls-utilpack-1.6.1/src/dls_utilpack/visit.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack/whatenv.py` & `dls-utilpack-1.6.1/src/dls_utilpack/whatenv.py`

 * *Files 19% similar despite different names*

```diff
@@ -60,38 +60,50 @@
         # Add keys from the provided extra_dict if given.
         if self.__extra_dict is not None:
             output_dict.update(self.__extra_dict)
 
         self.__compose_scalar("HOSTNAME", output_dict)
         self.__compose_scalar("USER", output_dict)
         output_dict["os.getcwd"] = os.getcwd()
-        self.__compose_scalar("SGE_CELL", output_dict)
-        self.__compose_scalar("SGE_EXECD_PORT", output_dict)
-        self.__compose_scalar("SGE_QMASTER_PORT", output_dict)
-
-        self.__compose_scalar("SGE_HGR_gpu", output_dict)
-        self.__compose_scalar("SGE_HGR_m_mem_free", output_dict)
-        self.__compose_scalar("SGE_HGR_TASK_gpu", output_dict)
-        self.__compose_scalar("SGE_HGR_TASK_m_mem_free", output_dict)
-        self.__compose_scalar("PE", output_dict)
-        self.__compose_scalar("QUEUE", output_dict)
-
-        self.__compose_scalar("JOB_ID", output_dict)
-        self.__compose_scalar("JOB_NAME", output_dict)
 
         self.__compose_scalar("VIRTUAL_ENV", output_dict)
 
-        self.__compose_scalar("CONDA_PREFIX", output_dict)
+        sge_dict: dict = {}
+        self.__compose_scalar("SGE_CELL", sge_dict)
+        self.__compose_scalar("SGE_EXECD_PORT", sge_dict)
+        self.__compose_scalar("SGE_QMASTER_PORT", sge_dict)
+        self.__compose_scalar("SGE_HGR_gpu", sge_dict)
+        self.__compose_scalar("SGE_HGR_m_mem_free", sge_dict)
+        self.__compose_scalar("SGE_HGR_TASK_gpu", sge_dict)
+        self.__compose_scalar("SGE_HGR_TASK_m_mem_free", sge_dict)
+        self.__compose_scalar("PE", sge_dict)
+        self.__compose_scalar("QUEUE", sge_dict)
+        self.__compose_scalar("JOB_ID", sge_dict)
+        self.__compose_scalar("JOB_NAME", sge_dict)
+        output_dict["sge"] = sge_dict
+
+        slurm_dict: dict = {}
+        for k in os.environ.keys():
+            if k.startswith("SLURM"):
+                self.__compose_scalar(k, slurm_dict)
+        output_dict["slurm"] = slurm_dict
+
+        conda_dict: dict = {}
+        self.__compose_scalar("CONDA_PREFIX", conda_dict)
         conda_shlvl = int(os.environ.get("CONDA_SHLVL", 0))
         for i in range(conda_shlvl - 1, 0, -1):
-            self.__compose_scalar(f"CONDA_PREFIX_{i}", output_dict)
+            self.__compose_scalar(f"CONDA_PREFIX_{i}", conda_dict)
+        output_dict["conda"] = conda_dict
 
-        self.__compose_paths("MODULEPATH", output_dict)
-        self.__compose_paths("LOADEDMODULES", output_dict)
-        self.__compose_paths("PATH", output_dict)
+        modules_dict: dict = {}
+        self.__compose_paths("MODULEPATH", modules_dict)
+        self.__compose_paths("MODULESHOME", modules_dict)
+        self.__compose_paths("LOADEDMODULES", modules_dict)
+        self.__compose_paths("PATH", modules_dict)
+        output_dict["modules"] = modules_dict
 
         uname = platform.uname()
         platform_dict = {}
         platform_dict["system"] = uname.system
         platform_dict["node"] = uname.node
         platform_dict["python_version"] = platform.python_version()
         platform_dict["release"] = uname.release
```

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack.egg-info/PKG-INFO` & `dls-utilpack-1.6.1/src/dls_utilpack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-utilpack
-Version: 1.6.0
+Version: 1.6.1
 Summary: Library of various useful Python classes and functions.
 Author-email: David Erb <david.erb@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `dls-utilpack-1.6.0/src/dls_utilpack.egg-info/SOURCES.txt` & `dls-utilpack-1.6.1/src/dls_utilpack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/base.py` & `dls-utilpack-1.6.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/base_tester.py` & `dls-utilpack-1.6.1/tests/base_tester.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/conftest.py` & `dls-utilpack-1.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_bash_composer.py` & `dls-utilpack-1.6.1/tests/test_bash_composer.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_callsign.py` & `dls-utilpack-1.6.1/tests/test_callsign.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_datatypes.py` & `dls-utilpack-1.6.1/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_hazzathread.py` & `dls-utilpack-1.6.1/tests/test_hazzathread.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_import.py` & `dls-utilpack-1.6.1/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_module.py` & `dls-utilpack-1.6.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_profiler.py` & `dls-utilpack-1.6.1/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_sanitize.py` & `dls-utilpack-1.6.1/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_server_context.py` & `dls-utilpack-1.6.1/tests/test_server_context.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         self.was_exited = 0
 
     # Minimal methods required for a "context" to provide.
     async def aenter(self):
         """ """
         self.was_entered += 1
 
-    async def aexit(self, type, value, traceback):
+    async def aexit(self, type=None, value=None, traceback=None):
         """ """
         self.was_exited += 1
 
 
 # ----------------------------------------------------------------------------------------
 class TestServerContext(BaseTester):
     def test(self, constants, logging_setup, output_directory):
```

### Comparing `dls-utilpack-1.6.0/tests/test_sigint1.py` & `dls-utilpack-1.6.1/tests/test_sigint1.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_sigint2.py` & `dls-utilpack-1.6.1/tests/test_sigint2.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_substitute.py` & `dls-utilpack-1.6.1/tests/test_substitute.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_visit.py` & `dls-utilpack-1.6.1/tests/test_visit.py`

 * *Files identical despite different names*

### Comparing `dls-utilpack-1.6.0/tests/test_whatenv.py` & `dls-utilpack-1.6.1/tests/test_whatenv.py`

 * *Files identical despite different names*

