# Comparing `tmp/gretel-trainer-0.8.2.tar.gz` & `tmp/gretel-trainer-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gretel-trainer-0.8.2.tar", last modified: Thu Jun  1 19:27:37 2023, max compression
+gzip compressed data, was "gretel-trainer-0.9.0.tar", last modified: Tue Jun 20 17:56:26 2023, max compression
```

## Comparing `gretel-trainer-0.8.2.tar` & `gretel-trainer-0.9.0.tar`

### file list

```diff
@@ -1,140 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/data/cpu_states.csv
--rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/data/mitre-synthea-health.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/img/gretel-logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/img/gretel_logo_white.png
--rw-r--r--   0 runner    (1001) docker     (123)     3638 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/models.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/docs/trainer.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/benchmark.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/conditional-generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/custom-example.py
--rw-r--r--   0 runner    (1001) docker     (123)    18962 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/relational.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/simple-conditional-generation.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/simple-example.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/notebooks/trainer-examples.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.809153 gretel-trainer-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6549 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26448 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/drawing.py
--rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    45200 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/multi_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/
--rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/figures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/key_highlight.js
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.css
--rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_privacy_protection.css
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_synthetic_quality.css
--rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_template.html
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/sdk_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)    14201 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/ancestral.py
--rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/independent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/table_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/task_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5552 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/classify.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_train.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/relational/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/src/gretel_trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.813153 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 19:27:37.000000 gretel-trainer-0.8.2/src/gretel_trainer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.817153 gretel-trainer-0.8.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/data/core-221-train.csv
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/example_config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/mocks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.821153 gretel-trainer-0.8.2/tests/relational/
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:27:37.825153 gretel-trainer-0.8.2/tests/relational/example_dbs/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/art.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/documents.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/ecom.sql
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/mutagenesis.sql
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/pets.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/tpch.sql
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/example_dbs/trips.sql
--rw-r--r--   0 runner    (1001) docker     (123)    20868 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_ancestral_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_ancestry.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     5280 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_common_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_connectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7070 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_independent_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_model_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_multi_table_config_options.py
--rw-r--r--   0 runner    (1001) docker     (123)    25141 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_multi_table_restore.py
--rw-r--r--   0 runner    (1001) docker     (123)    12054 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_relational_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    30649 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_relational_data_with_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_synthetics_run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_task_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_train_synthetics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/relational/test_train_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-01 19:27:31.000000 gretel-trainer-0.8.2/tests/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.956721 gretel-trainer-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.964721 gretel-trainer-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11950 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.964721 gretel-trainer-0.9.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   108190 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/data/cpu_states.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   629637 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/data/mitre-synthea-health.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.968721 gretel-trainer-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.968721 gretel-trainer-0.9.0/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/img/gretel-logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/img/gretel_logo_white.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/models.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/relational.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/docs/trainer.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.972721 gretel-trainer-0.9.0/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/benchmark.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/conditional-generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/custom-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19041 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/relational.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/simple-conditional-generation.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/simple-example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/table_extraction_with_subsetting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/notebooks/trainer-examples.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.960721 gretel-trainer-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.972721 gretel-trainer-0.9.0/src/gretel_trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4089 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29056 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21916 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51127 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/multi_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/
+-rw-r--r--   0 runner    (1001) docker     (123)     4473 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/key_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_privacy_protection.css
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_synthetic_quality.css
+-rw-r--r--   0 runner    (1001) docker     (123)     6910 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_template.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/sdk_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)    14319 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/ancestral.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4560 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10888 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/independent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/table_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/task_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.980721 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/classify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7206 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/relational/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29826 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/src/gretel_trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.976721 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-20 17:56:26.000000 gretel-trainer-0.9.0/src/gretel_trainer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.984721 gretel-trainer-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.984721 gretel-trainer-0.9.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2927798 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/data/core-221-train.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/example_config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/mocks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/tests/relational/
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:56:26.988721 gretel-trainer-0.9.0/tests/relational/example_dbs/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/art.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/documents.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/ecom.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/mutagenesis.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/pets.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/tpch.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/example_dbs/trips.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    22755 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_ancestral_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8603 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_ancestry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5342 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_common_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_connectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7539 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_independent_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_model_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_multi_table_config_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25838 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_multi_table_restore.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12055 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_relational_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30572 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_relational_data_with_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8206 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6422 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_synthetics_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5813 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_task_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_train_synthetics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/relational/test_train_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13550 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-20 17:56:21.000000 gretel-trainer-0.9.0/tests/test_strategy.py
```

### Comparing `gretel-trainer-0.8.2/.github/workflows/python-publish.yml` & `gretel-trainer-0.9.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/.gitignore` & `gretel-trainer-0.9.0/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -167,7 +167,8 @@
 cdk.out
 
 _build
 
 trainer-runner.json
 seeds.csv
 *.csv
+*.db
```

### Comparing `gretel-trainer-0.8.2/LICENSE` & `gretel-trainer-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/PKG-INFO` & `gretel-trainer-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.8.2
+Version: 0.9.0
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
@@ -12,11 +12,12 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Provides-Extra: connectors
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: snowflake
+Provides-Extra: bigquery
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `gretel-trainer-0.8.2/README.md` & `gretel-trainer-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/data/cpu_states.csv` & `gretel-trainer-0.9.0/data/cpu_states.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/data/mitre-synthea-health.csv` & `gretel-trainer-0.9.0/data/mitre-synthea-health.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/docs/Makefile` & `gretel-trainer-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/docs/conf.py` & `gretel-trainer-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/docs/img/gretel-logo.png` & `gretel-trainer-0.9.0/docs/img/gretel-logo.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/docs/img/gretel_logo_white.png` & `gretel-trainer-0.9.0/docs/img/gretel_logo_white.png`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/docs/index.rst` & `gretel-trainer-0.9.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
 .. toctree::
    :maxdepth: 2
 
    quickstart.rst
    trainer.rst
    models.rst
+   relational.rst
 
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
```

### Comparing `gretel-trainer-0.8.2/docs/make.bat` & `gretel-trainer-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/docs/quickstart.rst` & `gretel-trainer-0.9.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/notebooks/benchmark.ipynb` & `gretel-trainer-0.9.0/notebooks/benchmark.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/notebooks/conditional-generation.py` & `gretel-trainer-0.9.0/notebooks/conditional-generation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/notebooks/custom-example.py` & `gretel-trainer-0.9.0/notebooks/custom-example.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/notebooks/relational.ipynb` & `gretel-trainer-0.9.0/notebooks/relational.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997831076875194%*

 * *Differences: {"'cells'": "{3: {'source': {insert: [(12, "*

 * *            '\'mt.train_synthetics(config="synthetics/amplify")\\n\')], delete: [12]}}, 15: '*

 * *            "{'source': {delete: [5]}}, 25: {'source': {insert: [(2, "*

 * *            '\'multitable.train_synthetics(config="synthetics/amplify")\\n\'), (7, \'# '*

 * *            'multitable.train_synthetics(config="synthetics/amplify", '*

 * *            'ignore={"distribution_center", "products"})\\n\'), (8, \'# '*

 * *            'multitable.train_synthetics(config="synthetics/amplify […]*

```diff
@@ -42,15 +42,15 @@
                 "!curl -o \"ecom_xf.db\" \"https://gretel-blueprints-pub.s3.us-west-2.amazonaws.com/rdb/ecom_xf.db\"\n",
                 "\n",
                 "\n",
                 "connector = sqlite_conn(\"ecom_xf.db\")\n",
                 "relational_data = connector.extract()\n",
                 "\n",
                 "mt = MultiTable(relational_data)\n",
-                "mt.train_synthetics()\n",
+                "mt.train_synthetics(config=\"synthetics/amplify\")\n",
                 "mt.generate()\n",
                 "\n",
                 "connector.save(mt.synthetic_output_tables, prefix=\"synthetic_\")"
             ]
         },
         {
             "attachments": {},
@@ -237,15 +237,14 @@
             "outputs": [],
             "source": [
                 "from gretel_trainer.relational import MultiTable\n",
                 "\n",
                 "multitable = MultiTable(\n",
                 "    relational_data,\n",
                 "    # project_display_name=\"multi-table\",\n",
-                "    # gretel_model=\"amplify\",\n",
                 "    # strategy=\"independent\",\n",
                 "    # refresh_interval=60,\n",
                 ")"
             ]
         },
         {
             "attachments": {},
@@ -389,21 +388,21 @@
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Train synthetic models for all tables\n",
                 "\n",
-                "multitable.train_synthetics()\n",
+                "multitable.train_synthetics(config=\"synthetics/amplify\")\n",
                 "\n",
                 "# Optionally limit which tables are trained for synthetics via `only` (included) or `ignore` (excluded).\n",
                 "# Given our example data, the two calls below will lead to the same tables getting trained, just specified different ways.\n",
                 "#\n",
-                "# multitable.train_synthetics(ignore={\"distribution_center\", \"products\"})\n",
-                "# multitable.train_synthetics(only={\"users\", \"events\", \"inventory_items\", \"order_items\"})"
+                "# multitable.train_synthetics(config=\"synthetics/amplify\", ignore={\"distribution_center\", \"products\"})\n",
+                "# multitable.train_synthetics(config=\"synthetics/amplify\", only={\"users\", \"events\", \"inventory_items\", \"order_items\"})"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `gretel-trainer-0.8.2/notebooks/simple-conditional-generation.ipynb` & `gretel-trainer-0.9.0/notebooks/simple-conditional-generation.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/notebooks/trainer-examples.ipynb` & `gretel-trainer-0.9.0/notebooks/trainer-examples.ipynb`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/setup.py` & `gretel-trainer-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,44 +1,48 @@
 import pathlib
 from setuptools import setup, find_packages
 
 local_path = pathlib.Path(__file__).parent
 install_requires = (local_path / "requirements.txt").read_text().splitlines()
 
 mysql_extras = [
-    "mysqlclient",
+    "mysqlclient~=2.1",
 ]
 postgres_extras = [
-    "psycopg2-binary",
+    "psycopg2-binary~=2.9",
 ]
 snowflake_extras = [
-    "snowflake-sqlalchemy",
+    "snowflake-sqlalchemy~=1.4",
 ]
-connectors_extras = mysql_extras + postgres_extras + snowflake_extras
+bigquery_extras = ["sqlalchemy-bigquery[bqstorage]~=1.6"]
 
-setup(name="gretel-trainer",
-      use_scm_version=True,
-      setup_requires=["setuptools_scm"],
-      package_dir={'': 'src'},
-      install_requires=install_requires,
-      extras_require={
-          "connectors": connectors_extras,
-          "mysql": mysql_extras,
-          "postgres": postgres_extras,
-          "snowflake": snowflake_extras,
-      },
-      python_requires=">=3.9",
-      packages=find_packages("src"),
-      package_data={'': ['*.yaml']},
-      include_package_data=True,
-      description="Synthetic Data Generation with optional Differential Privacy",
-      url="https://github.com/gretelai/gretel-trainer",
-      license="https://gretel.ai/license/source-available-license",
-      classifiers=[
+connectors_extras = mysql_extras + postgres_extras + snowflake_extras + bigquery_extras
+
+setup(
+    name="gretel-trainer",
+    use_scm_version=True,
+    setup_requires=["setuptools_scm"],
+    package_dir={"": "src"},
+    install_requires=install_requires,
+    extras_require={
+        "connectors": connectors_extras,
+        "mysql": mysql_extras,
+        "postgres": postgres_extras,
+        "snowflake": snowflake_extras,
+        "bigquery": bigquery_extras,
+    },
+    python_requires=">=3.9",
+    packages=find_packages("src"),
+    package_data={"": ["*.yaml"]},
+    include_package_data=True,
+    description="Synthetic Data Generation with optional Differential Privacy",
+    url="https://github.com/gretelai/gretel-trainer",
+    license="https://gretel.ai/license/source-available-license",
+    classifiers=[
         "Programming Language :: Python :: 3",
         "License :: Free To Use But Restricted",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS",
         "Operating System :: Microsoft :: Windows",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
-      ]
+    ],
 )
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/__init__.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/compare.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/compare.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/core.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/core.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/datasets.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/custom/executor.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/custom/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/datasets.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/datasets.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/executor.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/executor.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/models.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/benchmark/gretel/sdk.py` & `gretel-trainer-0.9.0/src/gretel_trainer/benchmark/gretel/sdk.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/models.py` & `gretel-trainer-0.9.0/src/gretel_trainer/models.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/README.md` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/README.md`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/ancestry.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/ancestry.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     for foreign_key in rel_data.get_foreign_keys(table):
         fk_lineage = _COL_DELIMITER.join(foreign_key.columns)
         next_lineage = f"{lineage}{_GEN_DELIMITER}{fk_lineage}"
 
         parent_table_name = foreign_key.parent_table_name
 
         if ancestral_seeding:
-            usecols = rel_data.get_safe_ancestral_seed_columns(parent_table_name)
+            usecols = list(rel_data.get_safe_ancestral_seed_columns(parent_table_name))
         else:
             usecols = rel_data.get_table_columns(parent_table_name)
 
         if tableset is not None:
             parent_data = tableset[parent_table_name][list(usecols)]
         else:
             parent_data = rel_data.get_table_data(parent_table_name, usecols=usecols)
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/artifacts.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/artifacts.py`

 * *Files 20% similar despite different names*

```diff
@@ -54,25 +54,46 @@
 
         latest = project.upload_artifact(path)
         if existing is not None:
             project.delete_artifact(existing)
         return latest
 
 
-def add_to_tar(targz: Path, src: Path, arcname: str) -> None:
+def archive_items(targz: Path, items: list[Path]) -> None:
+    with tempfile.TemporaryDirectory() as tmpdir:
+        for item in items:
+            shutil.copy(item, tmpdir)
+        _archive_dir(targz, Path(tmpdir))
+
+
+def archive_nested_dir(targz: Path, directory: Path, name: str) -> None:
+    """
+    Creates an archive of the provided `directory` with name `{name}.tar.gz`
+    and adds it to the provided `targz` archive (or creates it if `targz` does not yet exist).
+    """
+    with tempfile.TemporaryDirectory() as tmpdir:
+        nested_archive = Path(f"{tmpdir}/{name}.tar.gz")
+        _archive_dir(nested_archive, directory)
+        _add_to_archive(targz, nested_archive)
+
+
+def _archive_dir(targz: Path, directory: Path) -> None:
+    shutil.make_archive(
+        base_name=_base_name(targz),
+        format="gztar",
+        root_dir=directory,
+    )
+
+
+def _add_to_archive(targz: Path, item: Path) -> None:
     if targz.exists():
         with tempfile.TemporaryDirectory() as tmpdir:
-            tmpdir = Path(tmpdir)
-
-            backup = tmpdir / "backup.tar.gz"
-            shutil.copy(targz, backup)
+            shutil.unpack_archive(targz, extract_dir=tmpdir, format="gztar")
+            shutil.copy(item, tmpdir)
+            _archive_dir(targz, Path(tmpdir))
+    else:
+        archive_items(targz, [item])
 
-            with tarfile.open(targz, "w:gz") as w, tarfile.open(backup, "r:gz") as r:
-                w.add(src, arcname=arcname)
 
-                r.extractall(tmpdir)
-                for member in r.getnames():
-                    if os.path.isfile(tmpdir / member) and not member == arcname:
-                        w.add(tmpdir / member, arcname=member)
-    else:
-        with tarfile.open(targz, "w:gz") as tar:
-            tar.add(src, arcname=arcname)
+def _base_name(targz: Path) -> str:
+    # shutil.make_archive base_name expects a name *without* a format-specific extension
+    return str(targz).removesuffix(".tar.gz")
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/backup.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/backup.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/connectors.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/connectors.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,29 @@
+"""
+This module provides the "Connector" class which allows for reading from
+and writing to databases and data warehouses. This class can handle
+metadata and table extraction automatically. When this is done with
+the "Connector.extract" method, a "RelationalData" instance is provided
+which you can then use with the "MultiTable" class to process data with
+Gretel Transforms, Classify, Synthetics, or a combination of both.
+"""
+from __future__ import annotations
+
 import logging
+import tempfile
+from pathlib import Path
 from typing import Optional
 
 import pandas as pd
-from sqlalchemy import create_engine, inspect
+from sqlalchemy import create_engine
 from sqlalchemy.engine.base import Engine
 from sqlalchemy.exc import OperationalError
 
-from gretel_trainer.relational.core import (
-    MultiTableException,
-    RelationalData,
-    skip_table,
-)
+from gretel_trainer.relational.core import MultiTableException, RelationalData
+from gretel_trainer.relational.extractor import ExtractorConfig, TableExtractor
 
 logger = logging.getLogger(__name__)
 
 
 class Connector:
     """
     Wraps connections to relational databases and backups.
@@ -37,59 +46,68 @@
         try:
             self.engine.connect()
         except OperationalError as e:
             logger.error(f"{e}, {e.__cause__}")
             raise e
         logger.info("Successfully connected to db")
 
+    @classmethod
+    def from_conn_str(cls, conn_str: str) -> Connector:
+        """
+        Alternate constructor that creates a Connector instance
+        directly from a connection string.
+
+        Args:
+            conn_str: A full connection string for the target database.
+        """
+        engine = create_engine(conn_str)
+        return cls(engine)
+
     def extract(
         self,
         only: Optional[set[str]] = None,
         ignore: Optional[set[str]] = None,
         schema: Optional[str] = None,
+        config: Optional[ExtractorConfig] = None,
     ) -> RelationalData:
         """
         Extracts table data and relationships from the database. Optional args include:
-        - `only` (restrict extraction to these tables; cannot be used with `ignore`)
-        - `ignore` (exclude these tables from extraction; cannot be used with `only`)
-        - `schema` (limit scope to a specific schema; this is dialect-specific and not supported by all databases)
+
+        Args:
+            only: Only extract these table names, cannot be used with `ignore`
+            ignore: Skip extracting these table names, cannot be used with `only`
+            schema: An optional schema name that is passed through to SQLAlchemy, may only
+                be used with certain dialects.
+            config: An optional extraction config. This config can be used to only include
+                specific tables, ignore specific tables, and configure subsetting. Please
+                see the `ExtractorConfig` docs for more details.
         """
         if only is not None and ignore is not None:
             raise MultiTableException("Cannot specify both `only` and `ignore`.")
 
-        inspector = inspect(self.engine)
+        if config is None:
+            config = ExtractorConfig(
+                only=only, ignore=ignore, schema=schema  # pyright: ignore
+            )
 
-        relational_data = RelationalData()
-        foreign_keys: list[tuple[str, dict]] = []
+        with tempfile.TemporaryDirectory() as tmpdir:
+            extractor = TableExtractor(
+                config=config, connector=self, storage_dir=Path(tmpdir)
+            )
+            extractor.sample_tables()
 
-        for table_name in inspector.get_table_names(schema=schema):
-            if skip_table(table_name, only, ignore):
-                continue
-
-            logger.debug(f"Extracting source data from `{table_name}`")
-            df = pd.read_sql_table(table_name, self.engine, schema=schema)
-            primary_key = inspector.get_pk_constraint(table_name)["constrained_columns"]
-            for fk in inspector.get_foreign_keys(table_name):
-                if skip_table(fk["referred_table"], only, ignore):
-                    continue
-                else:
-                    foreign_keys.append((table_name, fk))
-
-            relational_data.add_table(name=table_name, primary_key=primary_key, data=df)
-
-        for foreign_key in foreign_keys:
-            table, fk = foreign_key
-            relational_data.add_foreign_key_constraint(
-                table=table,
-                constrained_columns=fk["constrained_columns"],
-                referred_table=fk["referred_table"],
-                referred_columns=fk["referred_columns"],
+            # We ensure to re-create RelationalData after extraction so
+            # we can account for any embedded JSON. This also loads
+            # each table as a DF in the object which is currently
+            # the expected behavior for later operations.
+            extractor._relational_data = extractor._create_rel_data(
+                extracted_tables=extractor.table_order
             )
 
-        return relational_data
+        return extractor.relational_data
 
     def save(self, tables: dict[str, pd.DataFrame], prefix: str = "") -> None:
         for name, data in tables.items():
             data.to_sql(
                 f"{prefix}{name}", con=self.engine, if_exists="replace", index=False
             )
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/core.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+"""
+This module exposes the "RelationalData" class to users, which allows the processing
+of relational databases and data warehouses with Gretel.ai.
+
+When using a "Connector" or a "TableExtractor" instance to automatically connect
+to a database, a "RelationalData" instance will be created for you that contains
+all of the learned metadata.
+
+If you are processing relational tables manually, with your own CSVs, you
+will need to create a "RelationalData" instance and populate it yourself.
+
+Please see the specific docs for the "RelationalData" class on how to do this.
+"""
+
 from __future__ import annotations
 
 import logging
 from dataclasses import dataclass, replace
 from enum import Enum
 from pathlib import Path
 from typing import Any, Optional, Union
@@ -70,24 +84,47 @@
     """
 
 
 @dataclass
 class TableMetadata:
     primary_key: list[str]
     data: pd.DataFrame
-    columns: set[str]
+    columns: list[str]
     invented_table_metadata: Optional[InventedTableMetadata] = None
     safe_ancestral_seed_columns: Optional[set[str]] = None
 
 
 class RelationalData:
+    """
+    Stores information about multiple tables and their relationships. When
+    using this object you could create it without any arguments and rely
+    on the instance methods for adding tables and key relationships.
+
+    Example::
+
+        rel_data = RelationalData()
+        rel_data.add_table(...)
+        rel_data.add_table(...)
+        rel_data.add_foreign_key_constraint(...)
+
+    See the specific method docstrings for details on each method.
+    """
+
     def __init__(self):
         self.graph = networkx.DiGraph()
         self.relational_jsons: dict[str, RelationalJson] = {}
 
+    @property
+    def is_empty(self) -> bool:
+        """
+        Return a bool to indicate if the `RelationalData` contains
+        any table information.
+        """
+        return not self.graph.number_of_nodes() > 0
+
     def restore(self, tableset: dict[str, pd.DataFrame]) -> dict[str, pd.DataFrame]:
         """Restores a given tableset (presumably output from some MultiTable workflow,
         i.e. transforms or synthetics) to its original shape (specifically, "re-nests"
         any JSON that had been expanded out.
 
         Users should rely on MultiTable calling this internally when appropriate and not
         need to do so themselves.
@@ -166,15 +203,15 @@
         data: pd.DataFrame,
         invented_table_metadata: Optional[InventedTableMetadata] = None,
     ) -> None:
         primary_key = self._format_key_column(primary_key)
         metadata = TableMetadata(
             primary_key=primary_key,
             data=data,
-            columns=set(data.columns),
+            columns=list(data.columns),
             invented_table_metadata=invented_table_metadata,
         )
         self.graph.add_node(name, metadata=metadata)
 
     def set_primary_key(
         self, *, table: str, primary_key: UserFriendlyPrimaryKeyT
     ) -> None:
@@ -279,14 +316,20 @@
         table: str,
         constrained_columns: list[str],
         referred_table: str,
         referred_columns: list[str],
     ) -> None:
         """
         Add a foreign key relationship between two tables.
+
+        Args:
+            table: The table name that contains the foreign key.
+            constrained_columns: The column name(s) defining a relationship to the `referred_table` (the parent table).
+            referred_table: The table name that the foreign key in `table` refers to (the parent table).
+            referred_columns: The column name(s) in the parent table that the `constrained_columns` point to.
         """
         known_tables = self.list_all_tables(Scope.ALL)
 
         abort = False
         if table not in known_tables:
             logger.warning(f"Unrecognized table name: `{table}`")
             abort = True
@@ -380,14 +423,17 @@
         if len(via) == 0:
             self.graph.remove_edge(table, key_to_remove.parent_table_name)
         else:
             edge["via"] = via
         self._clear_safe_ancestral_seed_columns(table)
 
     def update_table_data(self, table: str, data: pd.DataFrame) -> None:
+        """
+        Set a DataFrame as the table data for a given table name.
+        """
         if table in self.relational_jsons:
             _, original_pk, original_fks = self._remove_relational_json(table)
             if (
                 new_rj_ingest := self._check_for_json(table, original_pk, data)
             ) is not None:
                 self._add_rel_json_and_tables(table, new_rj_ingest)
                 parent_table_name = new_rj_ingest[0].root_table_name
@@ -424,21 +470,21 @@
                         table=fk.table_name,
                         constrained_columns=fk.columns,
                         referred_table=new_rj_ingest[0].root_table_name,
                         referred_columns=fk.parent_columns,
                     )
             else:
                 metadata.data = data
-                metadata.columns = set(data.columns)
+                metadata.columns = list(data.columns)
                 self._clear_safe_ancestral_seed_columns(table)
 
     def list_all_tables(self, scope: Scope = Scope.MODELABLE) -> list[str]:
         """
         Returns a list of table names belonging to the provided Scope.
-        See Scope enum documentation for details.
+        See "Scope" enum documentation for details.
         By default, returns tables that can be submitted as jobs to Gretel
         (i.e. that are MODELABLE).
         """
         graph_nodes = list(self.graph.nodes)
 
         json_source_tables = [
             rel_json.original_table_name
@@ -477,15 +523,16 @@
     def _is_invented(self, table: str) -> bool:
         return (
             table in self.graph.nodes
             and self.graph.nodes[table]["metadata"].invented_table_metadata is not None
         )
 
     def get_modelable_table_names(self, table: str) -> list[str]:
-        """Returns a list of MODELABLE table names connected to the provided table.
+        """
+        Returns a list of MODELABLE table names connected to the provided table.
         If the provided table is the source of invented tables, returns the modelable invented tables created from it.
         If the provided table is itself modelable, returns that table name back.
         Otherwise returns an empty list.
         """
         if (rel_json := self.relational_jsons.get(table)) is not None:
             return [
                 t
@@ -513,30 +560,45 @@
     ) -> Optional[InventedTableMetadata]:
         if table in self.relational_jsons:
             return None
 
         return self.graph.nodes[table]["metadata"].invented_table_metadata
 
     def get_parents(self, table: str) -> list[str]:
+        """
+        Given a table name, return the table names that are referred to
+        by the foreign keys in this table.
+        """
         return list(self.graph.successors(table))
 
     def get_ancestors(self, table: str) -> list[str]:
+        """
+        Same as `get_parents` except recursively keep adding
+        parent tables until there are no more.
+        """
+
         def _add_parents(ancestors, table):
             parents = self.get_parents(table)
             if len(parents) > 0:
                 ancestors.update(parents)
                 for parent in parents:
                     _add_parents(ancestors, parent)
 
         ancestors = set()
         _add_parents(ancestors, table)
 
         return list(ancestors)
 
     def get_descendants(self, table: str) -> list[str]:
+        """
+        Given a table name, recursively return all tables that
+        carry foreign keys that reference the primary key in this table
+        and all subsequent tables that are discovered.
+        """
+
         def _add_children(descendants, table):
             children = list(self.graph.predecessors(table))
             if len(children) > 0:
                 descendants.update(children)
                 for child in children:
                     _add_children(descendants, child)
 
@@ -551,42 +613,52 @@
         appears before any of its children. No other guarantees about order
         are made, e.g. the following (and others) are all valid outputs:
         [p1, p2, c1, c2] or [p2, c2, p1, c1] or [p2, p1, c1, c2] etc.
         """
         return list(reversed(list(topological_sort(self.graph))))
 
     def get_primary_key(self, table: str) -> list[str]:
+        """
+        Return the list of columns defining the primary key for a table.
+        It may be a single column or multiple columns (composite key).
+        """
         try:
             return self.graph.nodes[table]["metadata"].primary_key
         except KeyError:
             if table in self.relational_jsons:
                 return self.relational_jsons[table].original_primary_key
             else:
                 raise MultiTableException(f"Unrecognized table: `{table}`")
 
     def get_table_data(
-        self, table: str, usecols: Optional[set[str]] = None
+        self, table: str, usecols: Optional[list[str]] = None
     ) -> pd.DataFrame:
+        """
+        Return the table contents for a given table name as a DataFrame.
+        """
         usecols = usecols or self.get_table_columns(table)
         try:
-            return self.graph.nodes[table]["metadata"].data[list(usecols)]
+            return self.graph.nodes[table]["metadata"].data[usecols]
         except KeyError:
             if table in self.relational_jsons:
                 if (df := self.relational_jsons[table].original_data) is None:
                     raise MultiTableException("Original data with JSON is lost.")
                 return df
             else:
                 raise MultiTableException(f"Unrecognized table: `{table}`")
 
-    def get_table_columns(self, table: str) -> set[str]:
+    def get_table_columns(self, table: str) -> list[str]:
+        """
+        Return the column names for a provided table name.
+        """
         try:
             return self.graph.nodes[table]["metadata"].columns
         except KeyError:
             if table in self.relational_jsons:
-                return set(self.relational_jsons[table].original_columns)
+                return self.relational_jsons[table].original_columns
             else:
                 raise MultiTableException(f"Unrecognized table: `{table}`")
 
     def get_safe_ancestral_seed_columns(self, table: str) -> set[str]:
         safe_columns = self.graph.nodes[table]["metadata"].safe_ancestral_seed_columns
         if safe_columns is None:
             safe_columns = self._set_safe_ancestral_seed_columns(table)
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/json.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
 class _RelationalData(Protocol):
     def get_foreign_keys(
         self, table: str
     ) -> list:  # can't specify element type (ForeignKey) without cyclic dependency
         ...
 
-    def get_table_columns(self, table: str) -> set[str]:
+    def get_table_columns(self, table: str) -> list[str]:
         ...
 
     def get_invented_table_metadata(
         self, table: str
     ) -> Optional[InventedTableMetadata]:
         ...
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/log.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/log.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/model_config.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/model_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,50 +1,64 @@
 from copy import deepcopy
-from typing import Any
+from typing import Any, Optional
 
+from gretel_client.projects.exceptions import ModelConfigError
 from gretel_client.projects.models import read_model_config
 
 from gretel_trainer.relational.core import (
     GretelModelConfig,
     MultiTableException,
     RelationalData,
 )
 
 
-def _ingest(config: GretelModelConfig) -> dict[str, Any]:
-    return read_model_config(deepcopy(config))
+def get_model_key(config_dict: dict[str, Any]) -> Optional[str]:
+    try:
+        models = config_dict["models"]
+        assert isinstance(models, list)
+        assert isinstance(models[0], dict)
+        return list(models[0])[0]
+    except (AssertionError, IndexError, KeyError):
+        return None
+
+
+def ingest(config: GretelModelConfig) -> dict[str, Any]:
+    try:
+        return read_model_config(deepcopy(config))
+    except ModelConfigError as e:
+        raise MultiTableException("Invalid config") from e
 
 
 def _model_name(workflow: str, table: str) -> str:
     ok_table_name = table.replace("--", "__")
     return f"{workflow}-{ok_table_name}"
 
 
 def make_classify_config(table: str, config: GretelModelConfig) -> dict[str, Any]:
-    tailored_config = _ingest(config)
+    tailored_config = ingest(config)
     tailored_config["name"] = _model_name("classify", table)
     return tailored_config
 
 
 def make_evaluate_config(table: str) -> dict[str, Any]:
-    tailored_config = _ingest("evaluate/default")
+    tailored_config = ingest("evaluate/default")
     tailored_config["name"] = _model_name("evaluate", table)
     return tailored_config
 
 
 def make_synthetics_config(table: str, config: GretelModelConfig) -> dict[str, Any]:
-    tailored_config = _ingest(config)
+    tailored_config = ingest(config)
     tailored_config["name"] = _model_name("synthetics", table)
     return tailored_config
 
 
 def make_transform_config(
     rel_data: RelationalData, table: str, config: GretelModelConfig
 ) -> dict[str, Any]:
-    tailored_config = _ingest(config)
+    tailored_config = ingest(config)
     tailored_config["name"] = _model_name("transforms", table)
 
     key_columns = rel_data.get_all_key_columns(table)
     if len(key_columns) > 0:
         try:
             model = tailored_config["models"][0]
             try:
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/multi_table.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/multi_table.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,39 @@
+"""
+This module provides the "MultiTable" class to users. This allows you to
+take extracted data from a database or data warehouse, and process it
+with Gretel using Transforms, Classify, and Synthetics.
+"""
 from __future__ import annotations
 
 import json
 import logging
 import os
 import shutil
 import tarfile
+import tempfile
 from collections import defaultdict
 from contextlib import suppress
 from dataclasses import replace
 from datetime import datetime
 from pathlib import Path
-from typing import Optional, Union
+from typing import Any, Optional, Union
 
 import pandas as pd
 import smart_open
 from gretel_client.config import RunnerMode, get_session_config
 from gretel_client.projects import Project, create_project, get_project
 from gretel_client.projects.jobs import ACTIVE_STATES, END_STATES, Status
 from gretel_client.projects.records import RecordHandler
 
-from gretel_trainer.relational.artifacts import ArtifactCollection, add_to_tar
+from gretel_trainer.relational.artifacts import (
+    ArtifactCollection,
+    archive_items,
+    archive_nested_dir,
+)
 from gretel_trainer.relational.backup import (
     Backup,
     BackupClassify,
     BackupGenerate,
     BackupRelationalData,
     BackupSyntheticsTrain,
     BackupTransformsTrain,
@@ -34,14 +44,16 @@
     RelationalData,
     Scope,
     skip_table,
 )
 from gretel_trainer.relational.json import InventedTableMetadata, RelationalJson
 from gretel_trainer.relational.log import silent_logs
 from gretel_trainer.relational.model_config import (
+    get_model_key,
+    ingest,
     make_classify_config,
     make_evaluate_config,
     make_synthetics_config,
     make_transform_config,
 )
 from gretel_trainer.relational.report.report import ReportPresenter, ReportRenderer
 from gretel_trainer.relational.sdk_extras import ExtendedGretelSDK
@@ -69,16 +81,15 @@
 
 class MultiTable:
     """
     Relational data support for the Trainer SDK
 
     Args:
         relational_data (RelationalData): Core data structure representing the source tables and their relationships.
-        strategy (str, optional): The strategy to use. Supports "independent" (default) and "ancestral".
-        gretel_model (str, optional): The underlying Gretel model to use. Default and acceptable models vary based on strategy.
+        strategy (str, optional): The strategy to use for synthetics. Supports "independent" (default) and "ancestral".
         project_display_name (str, optional): Display name in the console for a new Gretel project holding models and artifacts. Defaults to "multi-table".
         refresh_interval (int, optional): Frequency in seconds to poll Gretel Cloud for job statuses. Must be at least 30. Defaults to 60 (1m).
         backup (Backup, optional): Should not be supplied manually; instead use the `restore` classmethod.
     """
 
     def __init__(
         self,
@@ -87,17 +98,29 @@
         strategy: str = "independent",
         gretel_model: Optional[str] = None,
         project_display_name: Optional[str] = None,
         refresh_interval: Optional[int] = None,
         backup: Optional[Backup] = None,
     ):
         self._strategy = _validate_strategy(strategy)
-        model_name, model_config = self._validate_gretel_model(gretel_model)
-        self._gretel_model = model_name
-        self._model_config = model_config
+        if gretel_model is not None:
+            if backup is None:
+                logger.warning(
+                    "The `gretel_model` argument is deprecated and will be removed in a future release. "
+                    "Going forward you should provide a config to `train_synthetics`."
+                )
+            model_name, model_config = self._validate_gretel_model(gretel_model)
+            self._gretel_model = model_name
+            self._model_config = model_config
+        else:
+            # Set these to the original default for backwards compatibility.
+            # When we completely remove the `gretel_model` init param, these attrs can be removed as well.
+            # We don't need to validate here because the default model (amplify) works with both strategies.
+            self._gretel_model = "amplify"
+            self._model_config = "synthetics/amplify"
         self._set_refresh_interval(refresh_interval)
         self.relational_data = relational_data
         self._artifact_collection = ArtifactCollection(hybrid=self._hybrid)
         self._extended_sdk = ExtendedGretelSDK(hybrid=self._hybrid)
         self._latest_backup: Optional[Backup] = None
         self._classify = Classify()
         self._transforms_train = TransformsTrain()
@@ -310,16 +333,25 @@
             self._extended_sdk.download_tar_artifact(
                 self._project,
                 synthetics_outputs_archive_id,
                 synthetics_output_archive_path,
             )
         if synthetics_output_archive_path.exists():
             any_outputs = True
-            with tarfile.open(synthetics_output_archive_path, "r:gz") as tar:
-                tar.extractall(path=self._working_dir)
+            # Extract the nested archives to a temporary directory, and then
+            # extract the contents of each run archive to a subdir in the working directory
+            with tarfile.open(
+                synthetics_output_archive_path, "r:gz"
+            ) as tar, tempfile.TemporaryDirectory() as tmpdir:
+                tar.extractall(path=tmpdir)
+                for run_tar in os.listdir(tmpdir):
+                    with tarfile.open(f"{tmpdir}/{run_tar}", "r:gz") as rt:
+                        rt.extractall(
+                            path=self._working_dir / run_tar.removesuffix(".tar.gz")
+                        )
 
         ## Then, restore latest, potentially in-progress run data if present
         backup_generate = backup.generate
         if backup_generate is None:
             if any_outputs:
                 # We shouldn't ever encounter this branch in the wild, but we define some guidance to log just in case.
                 msg = "Backup included synthetics outputs archive but no latest run detail. Review previous runs' outputs (see CSVs and reports in the local directory), or start a new one by calling `generate`."
@@ -384,14 +416,17 @@
             logger.info(
                 f"At time of last backup, generation run `{latest_run_id}` was still in progress. From here, you can attempt to resume that generate job via `generate(resume=True)`, or restart generation from scratch via a regular call to `generate`."
             )
             return None
 
     @classmethod
     def restore(cls, backup_file: str) -> MultiTable:
+        """
+        Create a `MultiTable` instance from a backup file.
+        """
         logger.info(f"Restoring from backup file `{backup_file}`.")
         with open(backup_file, "r") as b:
             backup = Backup.from_dict(json.load(b))
 
         return MultiTable(
             relational_data=RelationalData(),
             strategy=backup.strategy,
@@ -542,16 +577,15 @@
             all_rows=all_rows,
             multitable=self,
             out_dir=self._working_dir,
         )
         run_task(task, self._extended_sdk)
 
         archive_path = self._working_dir / "classify_outputs.tar.gz"
-        for arcname, path in task.result_filepaths.items():
-            add_to_tar(archive_path, path, arcname)
+        archive_items(archive_path, task.result_filepaths)
         self._artifact_collection.upload_classify_outputs_archive(
             self._project, str(archive_path)
         )
 
     def _setup_transforms_train_state(
         self, configs: dict[str, GretelModelConfig]
     ) -> None:
@@ -616,24 +650,29 @@
         run_task(task, self._extended_sdk)
 
     def run_transforms(
         self,
         identifier: Optional[str] = None,
         in_place: bool = False,
         data: Optional[dict[str, pd.DataFrame]] = None,
+        encode_keys: bool = False,
     ) -> None:
         """
-        identifier: (str, optional): Unique string identifying a specific call to this method. Defaults to "transforms_" + current timestamp
-
-        If `in_place` set to True, overwrites source data in all locations
-        (internal Python state, local working directory, project artifact archive).
-        Used for transforms->synthetics workflows.
+        Run pre-trained Gretel Transform models on Relational table data:
 
-        If `data` is supplied, runs only the supplied data through the corresponding transforms models.
-        Otherwise runs source data through all existing transforms models.
+        Args:
+            identifier: Unique string identifying a specific call to this method. Defaults to `transforms_` + current timestamp
+            in_place: If True, overwrites source data in all locations
+                (internal Python state, local working directory, project artifact archive).
+                Used for transforms->synthetics workflows.
+            data: If supplied, runs only the supplied data through the corresponding transforms models.
+                Otherwise runs source data through all existing transforms models.
+            encode_keys: If set, primary and foreign keys will be replaced with label encoded variants. This can add
+                an additional level of privacy at the cost of referential integrity between transformed and
+                original data.
         """
         if data is not None:
             unrunnable_tables = [
                 table
                 for table in data
                 if not _table_trained_successfully(self._transforms_train, table)
             ]
@@ -669,42 +708,58 @@
 
         task = TransformsRunTask(
             record_handlers=transforms_record_handlers,
             multitable=self,
         )
         run_task(task, self._extended_sdk)
 
-        output_tables = self._strategy.label_encode_keys(
-            self.relational_data, task.output_tables
-        )
+        output_tables = task.output_tables
+        if encode_keys:
+            output_tables = self._strategy.label_encode_keys(
+                self.relational_data, task.output_tables
+            )
 
         if in_place:
             for table_name, transformed_table in output_tables.items():
                 self.relational_data.update_table_data(table_name, transformed_table)
             self._upload_sources_to_project()
 
         reshaped_tables = self.relational_data.restore(output_tables)
 
         for table, df in reshaped_tables.items():
             filename = f"transformed_{table}.csv"
             out_path = run_dir / filename
-            df.to_csv(out_path, index=False)
+            df.to_csv(
+                out_path,
+                index=False,
+                columns=self.relational_data.get_table_columns(table),
+            )
 
-        archive_path = self._working_dir / "transforms_outputs.tar.gz"
-        add_to_tar(archive_path, run_dir, identifier)
+        all_runs_archive_path = self._working_dir / "transforms_outputs.tar.gz"
+
+        archive_nested_dir(
+            targz=all_runs_archive_path,
+            directory=run_dir,
+            name=identifier,
+        )
 
         self._artifact_collection.upload_transforms_outputs_archive(
-            self._project, str(archive_path)
+            self._project, str(all_runs_archive_path)
         )
         self._backup()
         self.transform_output_tables = reshaped_tables
 
     def _get_only_and_ignore(
         self, only: Optional[set[str]], ignore: Optional[set[str]]
     ) -> tuple[Optional[set[str]], Optional[set[str]]]:
+        """
+        Accepts the `only` and `ignore` parameter values as provided by the user and:
+        - ensures both are not set (must provide one or the other, or neither)
+        - translates any JSON-source tables to the invented tables
+        """
         if only is not None and ignore is not None:
             raise MultiTableException("Cannot specify both `only` and `ignore`.")
 
         modelable_tables = set()
         for table in only or ignore or {}:
             m_names = self.relational_data.get_modelable_table_names(table)
             if len(m_names) == 0:
@@ -714,43 +769,38 @@
         if only is None:
             return (None, modelable_tables)
         elif ignore is None:
             return (modelable_tables, None)
         else:
             return (None, None)
 
-    def _prepare_training_data(self, tables: list[str]) -> dict[str, Path]:
+    def _train_synthetics_models(self, configs: dict[str, dict[str, Any]]) -> None:
         """
-        Exports a copy of each table prepared for training by the configured strategy
-        to the working directory. Returns a dict with table names as keys and Paths
-        to the CSVs as values.
+        Uses the configured strategy to prepare training data sources for each table,
+        exported to the working directory. Creates a model for each table and submits
+        it for training. Upon completion, downloads the evaluation reports for each
+        table to the working directory.
         """
-        training_data = self._strategy.prepare_training_data(
-            self.relational_data, tables
-        )
-        training_paths = {}
-
-        for table_name in tables:
-            training_path = self._working_dir / f"synthetics_train_{table_name}.csv"
-            training_data[table_name].to_csv(training_path, index=False)
-            training_paths[table_name] = training_path
+        training_paths = {
+            table: self._working_dir / f"synthetics_train_{table}.csv"
+            for table in configs
+        }
 
-        return training_paths
+        self._strategy.prepare_training_data(self.relational_data, training_paths)
 
-    def _train_synthetics_models(self, training_data: dict[str, Path]) -> None:
-        for table_name, training_csv in training_data.items():
-            synthetics_config = make_synthetics_config(table_name, self._model_config)
+        for table_name, config in configs.items():
+            synthetics_config = make_synthetics_config(table_name, config)
             model = self._project.create_model_obj(
-                model_config=synthetics_config, data_source=str(training_csv)
+                model_config=synthetics_config,
+                data_source=str(training_paths[table_name]),
             )
             self._synthetics_train.models[table_name] = model
 
         archive_path = self._working_dir / "synthetics_training.tar.gz"
-        for table_name, csv_path in training_data.items():
-            add_to_tar(archive_path, csv_path, csv_path.name)
+        archive_items(archive_path, list(training_paths.values()))
         self._artifact_collection.upload_synthetics_training_archive(
             self._project, str(archive_path)
         )
 
         self._backup()
 
         task = SyntheticsTrainTask(
@@ -774,50 +824,100 @@
         """
         DEPRECATED: Please use `train_synthetics` instead.
         """
         logger.warning(
             "This method is deprecated and will be removed in a future release. "
             "Please use `train_synthetics` instead."
         )
-        tables = self.relational_data.list_all_tables()
+        # This method completely resets any existing SyntheticsTrain state,
+        # orphaning any existing models in the project.
         self._synthetics_train = SyntheticsTrain()
 
-        training_data = self._prepare_training_data(tables)
-        self._train_synthetics_models(training_data)
+        # This method only supports using a single config
+        # (the blueprint config set at MultiTable initialization)
+        # and cannot omit any tables from training.
+        config = ingest(self._model_config)
+        configs = {table: config for table in self.relational_data.list_all_tables()}
+
+        self._train_synthetics_models(configs)
 
     def train_synthetics(
         self,
         *,
+        config: Optional[GretelModelConfig] = None,
+        table_specific_configs: Optional[dict[str, GretelModelConfig]] = None,
         only: Optional[set[str]] = None,
         ignore: Optional[set[str]] = None,
     ) -> None:
         """
         Train synthetic data models for the tables in the tableset,
         optionally scoped by either `only` or `ignore`.
         """
         only, ignore = self._get_only_and_ignore(only, ignore)
 
-        all_tables = self.relational_data.list_all_tables()
-        include_tables = []
-        omit_tables = []
-        for table in all_tables:
+        include_tables: list[str] = []
+        omit_tables: list[str] = []
+        for table in self.relational_data.list_all_tables():
             if skip_table(table, only, ignore):
                 omit_tables.append(table)
             else:
                 include_tables.append(table)
 
         # TODO: Ancestral strategy requires that for each table omitted from synthetics ("preserved"),
         # all its ancestors must also be omitted. In the future, it'd be nice to either find a way to
         # eliminate this requirement completely, or (less ideal) allow incremental training of tables,
         # e.g. train a few in one "batch", then a few more before generating (perhaps with some logs
         # along the way informing the user of which required tables are missing).
         self._strategy.validate_preserved_tables(omit_tables, self.relational_data)
 
-        training_data = self._prepare_training_data(include_tables)
-        self._train_synthetics_models(training_data)
+        # Translate any JSON-source tables in table_specific_configs to invented tables
+        all_table_specific_configs = {}
+        for table, conf in (table_specific_configs or {}).items():
+            m_names = self.relational_data.get_modelable_table_names(table)
+            if len(m_names) == 0:
+                raise MultiTableException(f"Unrecognized table name: `{table}`")
+            all_table_specific_configs.update({m: conf for m in m_names})
+
+        # Ensure compatibility between only/ignore and table_specific_configs
+        omitted_tables_with_overrides_specified = []
+        for table in all_table_specific_configs:
+            if table in omit_tables:
+                omitted_tables_with_overrides_specified.append(table)
+        if len(omitted_tables_with_overrides_specified) > 0:
+            raise MultiTableException(
+                f"Cannot provide configs for tables that have been omitted from synthetics training: "
+                f"{omitted_tables_with_overrides_specified}"
+            )
+
+        # Validate the provided config
+        # Currently an optional argument for backwards compatibility; if None, fall back to the one configured
+        # on the MultiTable instance via the deprecated `gretel_model` parameter
+        if config is not None:
+            default_config_dict = self._validate_synthetics_config(config)
+        else:
+            logger.warning(
+                "Calling `train_synthetics` without specifying a `config` is deprecated; "
+                "in a future release, this argument will be required. "
+                "For now, falling back to the model configured on the MultiTable instance "
+                "(which is also deprecated and scheduled for removal)."
+            )
+            default_config_dict = ingest(self._model_config)
+
+        # Validate any table-specific configs
+        table_specific_config_dicts = {
+            table: self._validate_synthetics_config(conf)
+            for table, conf in all_table_specific_configs.items()
+        }
+
+        configs = {
+            table: table_specific_config_dicts.get(table, default_config_dict)
+            for table in include_tables
+        }
+
+        self._train_synthetics_models(configs)
 
     def retrain_tables(self, tables: dict[str, pd.DataFrame]) -> None:
         """
         Provide updated table data and retrain. This method overwrites the table data in the
         `RelationalData` instance. It should be used when initial training fails and source data
         needs to be altered, but progress on other tables can be left as-is.
         """
@@ -829,25 +929,32 @@
         tables_to_retrain = self._strategy.tables_to_retrain(
             list(tables.keys()), self.relational_data
         )
 
         for table in tables_to_retrain:
             with suppress(KeyError):
                 del self._synthetics_train.models[table]
-        training_data = self._prepare_training_data(tables_to_retrain)
-        self._train_synthetics_models(training_data)
+
+        config = ingest(self._model_config)
+        configs = {table: config for table in tables_to_retrain}
+
+        self._train_synthetics_models(configs)
 
     def _upload_sources_to_project(self) -> None:
         archive_path = self._working_dir / "source_tables.tar.gz"
         with tarfile.open(archive_path, "w:gz") as tar:
             for table in self.relational_data.list_all_tables(Scope.ALL):
                 filename = f"source_{table}.csv"
                 out_path = self._working_dir / filename
                 df = self.relational_data.get_table_data(table)
-                df.to_csv(out_path, index=False)
+                df.to_csv(
+                    out_path,
+                    index=False,
+                    columns=self.relational_data.get_table_columns(table),
+                )
                 tar.add(out_path, arcname=filename)
         self._artifact_collection.upload_source_archive(
             self._project, str(archive_path)
         )
         self._backup()
 
     def generate(
@@ -862,15 +969,15 @@
         Tables that did not train successfully will be omitted from the output dictionary.
         Tables listed in `preserve_tables` *may differ* from source tables in foreign key columns, to ensure
         joining to parent tables (which may have been synthesized) continues to work properly.
 
         Args:
             record_size_ratio (float, optional): Ratio to upsample real world data size with. Defaults to 1.
             preserve_tables (list[str], optional): List of tables to skip sampling and leave (mostly) identical to source.
-            identifier (str, optional): Unique string identifying a specific call to this method. Defaults to "synthetics_" + current timestamp.
+            identifier (str, optional): Unique string identifying a specific call to this method. Defaults to `synthetics_` + current timestamp.
             resume (bool, optional): Set to True when restoring from a backup to complete a previous, interrupted run.
 
         Returns:
             dict[str, pd.DataFrame]: Return a dictionary of table names and output data.
         """
         if resume:
             if identifier is not None:
@@ -931,15 +1038,19 @@
             record_size_ratio=self._synthetics_run.record_size_ratio,
         )
 
         reshaped_tables = self.relational_data.restore(output_tables)
 
         for table, synth_df in reshaped_tables.items():
             synth_csv_path = run_dir / f"synth_{table}.csv"
-            synth_df.to_csv(synth_csv_path, index=False)
+            synth_df.to_csv(
+                synth_csv_path,
+                index=False,
+                columns=self.relational_data.get_table_columns(table),
+            )
 
         evaluate_project = create_project(
             display_name=f"evaluate-{self._project.display_name}"
         )
         evaluate_models = {}
         for table, synth_df in output_tables.items():
             if table in self._synthetics_run.preserved:
@@ -996,19 +1107,24 @@
 
         logger.info("Creating relational report")
         self.create_relational_report(
             run_identifier=self._synthetics_run.identifier,
             target_dir=run_dir,
         )
 
-        archive_path = self._working_dir / "synthetics_outputs.tar.gz"
-        add_to_tar(archive_path, run_dir, self._synthetics_run.identifier)
+        all_runs_archive_path = self._working_dir / "synthetics_outputs.tar.gz"
+
+        archive_nested_dir(
+            targz=all_runs_archive_path,
+            directory=run_dir,
+            name=self._synthetics_run.identifier,
+        )
 
         self._artifact_collection.upload_synthetics_outputs_archive(
-            self._project, str(archive_path)
+            self._project, str(all_runs_archive_path)
         )
         self.synthetic_output_tables = reshaped_tables
         self._backup()
 
     def create_relational_report(self, run_identifier: str, target_dir: Path) -> None:
         presenter = ReportPresenter(
             rel_data=self.relational_data,
@@ -1035,31 +1151,51 @@
 
         individual_report_json = json.loads(smart_open.open(individual_path).read())
         cross_table_report_json = json.loads(smart_open.open(cross_table_path).read())
 
         self._evaluations[table].individual_report_json = individual_report_json
         self._evaluations[table].cross_table_report_json = cross_table_report_json
 
-    def _validate_gretel_model(self, gretel_model: Optional[str]) -> tuple[str, str]:
-        gretel_model = (gretel_model or self._strategy.default_model).lower()
-        supported_models = self._strategy.supported_models
+    def _validate_gretel_model(self, gretel_model: str) -> tuple[str, str]:
+        supported_models = self._strategy.supported_gretel_models
         if gretel_model not in supported_models:
             msg = f"Invalid gretel model requested: {gretel_model}. The selected strategy supports: {supported_models}."
             logger.warning(msg)
             raise MultiTableException(msg)
 
         _BLUEPRINTS = {
             "amplify": "synthetics/amplify",
             "actgan": "synthetics/tabular-actgan",
             "lstm": "synthetics/tabular-lstm",
             "tabular-dp": "synthetics/tabular-differential-privacy",
         }
 
         return (gretel_model, _BLUEPRINTS[gretel_model])
 
+    def _validate_synthetics_config(self, config: GretelModelConfig) -> dict[str, Any]:
+        """
+        Validates that the provided config:
+        - has the general shape of a Gretel model config (or can be read into one, e.g. blueprints)
+        - is supported by the configured synthetics strategy
+
+        Returns the parsed config as read by read_model_config.
+        """
+        config_dict = ingest(config)
+        if (model_key := get_model_key(config_dict)) is None:
+            raise MultiTableException("Invalid config")
+        else:
+            supported_models = self._strategy.supported_model_keys
+            if model_key not in supported_models:
+                raise MultiTableException(
+                    f"Invalid gretel model requested: {model_key}. "
+                    f"The selected strategy supports: {supported_models}."
+                )
+
+        return config_dict
+
 
 def _validate_strategy(strategy: str) -> Union[IndependentStrategy, AncestralStrategy]:
     strategy = strategy.lower()
 
     if strategy == "independent":
         return IndependentStrategy()
     elif strategy == "ancestral":
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/figures.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/figures.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/key_highlight.js` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/key_highlight.js`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.css` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_privacy_protection.css` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_privacy_protection.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_synthetic_quality.css` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_synthetic_quality.css`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/report/report_template.html` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/report/report_template.html`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/sdk_extras.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/sdk_extras.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/ancestral.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/ancestral.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,41 +15,42 @@
 
 
 class AncestralStrategy:
     @property
     def name(self) -> str:
         return "ancestral"
 
+    # TODO: remove when `gretel_model` param is removed
     @property
-    def default_model(self) -> str:
-        return "amplify"
+    def supported_gretel_models(self) -> list[str]:
+        return ["amplify"]
 
     @property
-    def supported_models(self) -> list[str]:
+    def supported_model_keys(self) -> list[str]:
         return ["amplify"]
 
     def label_encode_keys(
         self, rel_data: RelationalData, tables: dict[str, pd.DataFrame]
     ) -> dict[str, pd.DataFrame]:
         return common.label_encode_keys(rel_data, tables)
 
     def prepare_training_data(
-        self, rel_data: RelationalData, tables: list[str]
-    ) -> dict[str, pd.DataFrame]:
+        self, rel_data: RelationalData, table_paths: dict[str, Path]
+    ) -> dict[str, Path]:
         """
-        Returns tables with:
+        Writes tables' training data to provided paths.
+        Training data has:
         - all safe-for-seed ancestor fields added
         - columns in multigenerational format
         - all keys translated to contiguous integers
         - artificial min/max seed records added
         """
         all_tables = rel_data.list_all_tables()
-        omitted_tables = [t for t in all_tables if t not in tables]
+        omitted_tables = [t for t in all_tables if t not in table_paths]
         altered_tableset = {}
-        training_data = {}
 
         # Create a new table set identical to source data
         for table_name in all_tables:
             altered_tableset[table_name] = rel_data.get_table_data(table_name).copy()
 
         # Translate all keys to a contiguous list of integers
         altered_tableset = common.label_encode_keys(
@@ -58,24 +59,24 @@
 
         # Add artificial rows to support seeding
         altered_tableset = _add_artifical_rows_for_seeding(
             rel_data, altered_tableset, omitted_tables
         )
 
         # Collect all data in multigenerational format
-        for table_name in tables:
+        for table, path in table_paths.items():
             data = ancestry.get_table_data_with_ancestors(
                 rel_data=rel_data,
-                table=table_name,
+                table=table,
                 tableset=altered_tableset,
                 ancestral_seeding=True,
             )
-            training_data[table_name] = data
+            data.to_csv(path, index=False)
 
-        return training_data
+        return table_paths
 
     def tables_to_retrain(
         self, tables: list[str], rel_data: RelationalData
     ) -> list[str]:
         """
         Given a set of tables requested to retrain, returns those tables with all their
         descendants, because those descendant tables were trained with data from their
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/common.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/common.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/strategies/independent.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/strategies/independent.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,47 +16,49 @@
 
 
 class IndependentStrategy:
     @property
     def name(self) -> str:
         return "independent"
 
+    # TODO: remove when `gretel_model` param is removed
     @property
-    def default_model(self) -> str:
-        return "amplify"
+    def supported_gretel_models(self) -> list[str]:
+        return ["amplify", "actgan", "lstm", "tabular-dp"]
 
     @property
-    def supported_models(self) -> list[str]:
-        return ["amplify", "actgan", "lstm", "tabular-dp"]
+    def supported_model_keys(self) -> list[str]:
+        return ["amplify", "actgan", "synthetics", "tabular_dp"]
 
     def label_encode_keys(
         self, rel_data: RelationalData, tables: dict[str, pd.DataFrame]
     ) -> dict[str, pd.DataFrame]:
         return common.label_encode_keys(rel_data, tables)
 
     def prepare_training_data(
-        self, rel_data: RelationalData, tables: list[str]
-    ) -> dict[str, pd.DataFrame]:
+        self, rel_data: RelationalData, table_paths: dict[str, Path]
+    ) -> dict[str, Path]:
         """
-        Returns source tables with primary and foreign keys removed
+        Writes tables' training data to provided paths.
+        Training data has primary and foreign key columns removed.
         """
-        training_data = {}
-
-        for table_name in tables:
-            columns_to_drop = []
-            columns_to_drop.extend(rel_data.get_primary_key(table_name))
-            for foreign_key in rel_data.get_foreign_keys(table_name):
-                columns_to_drop.extend(foreign_key.columns)
-
-            data = rel_data.get_table_data(table_name)
-            data = data.drop(columns=columns_to_drop)
-
-            training_data[table_name] = data
+        for table, path in table_paths.items():
+            columns_to_drop = set()
+            columns_to_drop.update(rel_data.get_primary_key(table))
+            for foreign_key in rel_data.get_foreign_keys(table):
+                columns_to_drop.update(foreign_key.columns)
+
+            all_columns = rel_data.get_table_columns(table)
+            use_columns = [col for col in all_columns if col not in columns_to_drop]
+
+            rel_data.get_table_data(table, usecols=use_columns).to_csv(
+                path, index=False
+            )
 
-        return training_data
+        return table_paths
 
     def tables_to_retrain(
         self, tables: list[str], rel_data: RelationalData
     ) -> list[str]:
         """
         Returns the provided tables requested to retrain, unaltered.
         """
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/table_evaluation.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/table_evaluation.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/task_runner.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/task_runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/classify.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/classify.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         self.multitable = multitable
         self.out_dir = out_dir
         self.classify_record_handlers: dict[str, RecordHandler] = {}
         self.completed_models = []
         self.failed_models = []
         self.completed_record_handlers = []
         self.failed_record_handlers = []
-        self.result_filepaths: dict[str, Path] = {}
+        self.result_filepaths: list[Path] = []
 
     def action(self, job: Job) -> str:
         if self.all_rows:
             if isinstance(job, Model):
                 return "classify training"
             else:
                 return "classification (all rows)"
@@ -149,8 +149,8 @@
 
         destpath = self.out_dir / filename
 
         with smart_open.open(
             job.get_artifact_link(artifact_name), "rb"
         ) as src, smart_open.open(str(destpath), "wb") as dest:
             shutil.copyfileobj(src, dest)
-        self.result_filepaths[filename] = destpath
+        self.result_filepaths.append(destpath)
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/common.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/common.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_evaluate.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_evaluate.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_run.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_run.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/synthetics_train.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/synthetics_train.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_run.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_run.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/tasks/transforms_train.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/tasks/transforms_train.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/relational/workflow_state.py` & `gretel-trainer-0.9.0/src/gretel_trainer/relational/workflow_state.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/runner.py` & `gretel-trainer-0.9.0/src/gretel_trainer/runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/strategy.py` & `gretel-trainer-0.9.0/src/gretel_trainer/strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer/trainer.py` & `gretel-trainer-0.9.0/src/gretel_trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer.egg-info/PKG-INFO` & `gretel-trainer-0.9.0/src/gretel_trainer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gretel-trainer
-Version: 0.8.2
+Version: 0.9.0
 Summary: Synthetic Data Generation with optional Differential Privacy
 Home-page: https://github.com/gretelai/gretel-trainer
 License: https://gretel.ai/license/source-available-license
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Free To Use But Restricted
 Classifier: Operating System :: POSIX :: Linux
@@ -12,11 +12,12 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Python: >=3.9
 Provides-Extra: connectors
 Provides-Extra: mysql
 Provides-Extra: postgres
 Provides-Extra: snowflake
+Provides-Extra: bigquery
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `gretel-trainer-0.8.2/src/gretel_trainer.egg-info/SOURCES.txt` & `gretel-trainer-0.9.0/src/gretel_trainer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,24 +12,26 @@
 data/mitre-synthea-health.csv
 docs/Makefile
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/models.rst
 docs/quickstart.rst
+docs/relational.rst
 docs/requirements.txt
 docs/trainer.rst
 docs/img/gretel-logo.png
 docs/img/gretel_logo_white.png
 notebooks/benchmark.ipynb
 notebooks/conditional-generation.py
 notebooks/custom-example.py
 notebooks/relational.ipynb
 notebooks/simple-conditional-generation.ipynb
 notebooks/simple-example.py
+notebooks/table_extraction_with_subsetting.ipynb
 notebooks/trainer-examples.ipynb
 src/gretel_trainer/__init__.py
 src/gretel_trainer/models.py
 src/gretel_trainer/runner.py
 src/gretel_trainer/strategy.py
 src/gretel_trainer/trainer.py
 src/gretel_trainer.egg-info/PKG-INFO
@@ -53,14 +55,15 @@
 src/gretel_trainer/relational/__init__.py
 src/gretel_trainer/relational/ancestry.py
 src/gretel_trainer/relational/artifacts.py
 src/gretel_trainer/relational/backup.py
 src/gretel_trainer/relational/connectors.py
 src/gretel_trainer/relational/core.py
 src/gretel_trainer/relational/drawing.py
+src/gretel_trainer/relational/extractor.py
 src/gretel_trainer/relational/json.py
 src/gretel_trainer/relational/log.py
 src/gretel_trainer/relational/model_config.py
 src/gretel_trainer/relational/multi_table.py
 src/gretel_trainer/relational/sdk_extras.py
 src/gretel_trainer/relational/table_evaluation.py
 src/gretel_trainer/relational/task_runner.py
@@ -93,14 +96,15 @@
 tests/relational/conftest.py
 tests/relational/test_ancestral_strategy.py
 tests/relational/test_ancestry.py
 tests/relational/test_artifacts.py
 tests/relational/test_backup.py
 tests/relational/test_common_strategy.py
 tests/relational/test_connectors.py
+tests/relational/test_extractor.py
 tests/relational/test_independent_strategy.py
 tests/relational/test_model_config.py
 tests/relational/test_multi_table_config_options.py
 tests/relational/test_multi_table_restore.py
 tests/relational/test_relational_data.py
 tests/relational/test_relational_data_with_json.py
 tests/relational/test_report.py
```

### Comparing `gretel-trainer-0.8.2/tests/data/core-221-train.csv` & `gretel-trainer-0.9.0/tests/data/core-221-train.csv`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/mocks.py` & `gretel-trainer-0.9.0/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/conftest.py` & `gretel-trainer-0.9.0/tests/relational/conftest.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -92,16 +92,16 @@
 def trips() -> RelationalData:
     rel_data = rel_data_from_example_db("trips")
     rel_data.update_table_data(
         table="trips",
         data=pd.DataFrame(
             data={
                 "id": list(range(100)),
-                "vehicle_type_id": [1] * 60 + [2] * 30 + [3] * 5 + [4] * 5,
                 "purpose": ["work"] * 100,
+                "vehicle_type_id": [1] * 60 + [2] * 30 + [3] * 5 + [4] * 5,
             }
         ),
     )
     return rel_data
 
 
 @pytest.fixture()
```

### Comparing `gretel-trainer-0.8.2/tests/relational/example_dbs/art.sql` & `gretel-trainer-0.9.0/tests/relational/example_dbs/art.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/example_dbs/documents.sql` & `gretel-trainer-0.9.0/tests/relational/example_dbs/documents.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/example_dbs/ecom.sql` & `gretel-trainer-0.9.0/tests/relational/example_dbs/ecom.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/example_dbs/mutagenesis.sql` & `gretel-trainer-0.9.0/tests/relational/example_dbs/mutagenesis.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/example_dbs/pets.sql` & `gretel-trainer-0.9.0/tests/relational/example_dbs/pets.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/example_dbs/tpch.sql` & `gretel-trainer-0.9.0/tests/relational/example_dbs/tpch.sql`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_ancestral_strategy.py` & `gretel-trainer-0.9.0/tests/relational/test_ancestral_strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,53 +10,64 @@
 
 import gretel_trainer.relational.ancestry as ancestry
 from gretel_trainer.relational.core import MultiTableException
 from gretel_trainer.relational.strategies.ancestral import AncestralStrategy
 from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 
-def test_preparing_training_data_does_not_mutate_source_data(pets, art):
-    for rel_data in [pets, art]:
-        original_tables = {
-            table: rel_data.get_table_data(table).copy()
-            for table in rel_data.list_all_tables()
-        }
-
-        strategy = AncestralStrategy()
-        strategy.prepare_training_data(rel_data, rel_data.list_all_tables())
-
-        for table in rel_data.list_all_tables():
-            pdtest.assert_frame_equal(
-                original_tables[table], rel_data.get_table_data(table)
-            )
+def test_preparing_training_data_does_not_mutate_source_data(pets):
+    original_tables = {
+        table: pets.get_table_data(table).copy() for table in pets.list_all_tables()
+    }
+
+    strategy = AncestralStrategy()
+
+    with tempfile.NamedTemporaryFile() as pets_dest, tempfile.NamedTemporaryFile() as humans_dest:
+        strategy.prepare_training_data(
+            pets, {"pets": Path(pets_dest.name), "humans": Path(humans_dest.name)}
+        )
+
+    for table in pets.list_all_tables():
+        pdtest.assert_frame_equal(original_tables[table], pets.get_table_data(table))
 
 
 def test_prepare_training_data_subset_of_tables(pets):
     strategy = AncestralStrategy()
 
-    # We aren't synthesizing the "humans" table, so it is not in this list argument...
-    training_data = strategy.prepare_training_data(pets, ["pets"])
-    # ...nor do we create training data for it
-    assert set(training_data.keys()) == {"pets"}
+    with tempfile.NamedTemporaryFile() as pets_dest, tempfile.NamedTemporaryFile() as humans_dest:
+        # We aren't synthesizing the "humans" table, so it is not in this list argument...
+        training_data = strategy.prepare_training_data(
+            pets, {"pets": Path(pets_dest.name)}
+        )
+
+        train_pets = pd.read_csv(training_data["pets"])
+
+        # ...nor do we create training data for it
+        assert not train_pets.empty
+        assert os.stat(humans_dest.name).st_size == 0
 
     # Since the humans table is omitted from synthetics, we leave the FK values alone; specifically:
     # - they are not label-encoded (which would effectively zero-index them)
     # - we do not add artificial min/max values
-    assert set(training_data["pets"]["self|human_id"].values) == {1, 2, 3, 4, 5}
+    assert set(train_pets["self|human_id"].values) == {1, 2, 3, 4, 5}
     # We do add the artificial max PK row, though, since this table is being synthesized
-    assert len(training_data["pets"]) == 6
+    assert len(train_pets) == 6
 
 
 def test_prepare_training_data_returns_multigenerational_data(pets):
     strategy = AncestralStrategy()
 
-    training_data = strategy.prepare_training_data(pets, pets.list_all_tables())
+    with tempfile.NamedTemporaryFile() as pets_dest, tempfile.NamedTemporaryFile() as humans_dest:
+        training_data = strategy.prepare_training_data(
+            pets, {"pets": Path(pets_dest.name), "humans": Path(humans_dest.name)}
+        )
+        train_pets = pd.read_csv(training_data["pets"])
 
     for expected_column in ["self|id", "self|name", "self.human_id|id"]:
-        assert expected_column in training_data["pets"]
+        assert expected_column in train_pets
 
 
 def test_prepare_training_data_drops_highly_unique_categorical_ancestor_fields(art):
     art.update_table_data(
         table="artists",
         data=pd.DataFrame(
             data={
@@ -73,18 +84,27 @@
                 "artist_id": [f"A{i}" for i in range(100)],
                 "name": [str(i) for i in range(100)],
             }
         ),
     )
 
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(art, art.list_all_tables())
+
+    with tempfile.NamedTemporaryFile() as artists_dest, tempfile.NamedTemporaryFile() as paintings_dest:
+        training_data = strategy.prepare_training_data(
+            art,
+            {
+                "artists": Path(artists_dest.name),
+                "paintings": Path(paintings_dest.name),
+            },
+        )
+        train_paintings = pd.read_csv(training_data["paintings"])
 
     # Does not contain `self.artist_id|name` because it is highly unique categorical
-    assert set(training_data["paintings"].columns) == {
+    assert set(train_paintings.columns) == {
         "self|id",
         "self|name",
         "self|artist_id",
         "self.artist_id|id",
     }
 
 
@@ -112,65 +132,95 @@
                 "artist_id": [f"A{i}" for i in range(100)],
                 "name": [str(i) for i in range(100)],
             }
         ),
     )
 
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(art, art.list_all_tables())
+
+    with tempfile.NamedTemporaryFile() as artists_dest, tempfile.NamedTemporaryFile() as paintings_dest:
+        training_data = strategy.prepare_training_data(
+            art,
+            {
+                "artists": Path(artists_dest.name),
+                "paintings": Path(paintings_dest.name),
+            },
+        )
+        train_paintings = pd.read_csv(training_data["paintings"])
 
     # Does not contain `self.artist_id|name` because it is highly NaN
-    assert set(training_data["paintings"].columns) == {
+    assert set(train_paintings.columns) == {
         "self|id",
         "self|name",
         "self|artist_id",
         "self.artist_id|id",
     }
 
 
 def test_prepare_training_data_translates_alphanumeric_keys_and_adds_min_max_records(
     art,
 ):
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(art, art.list_all_tables())
+
+    with tempfile.NamedTemporaryFile() as artists_dest, tempfile.NamedTemporaryFile() as paintings_dest:
+        training_data = strategy.prepare_training_data(
+            art,
+            {
+                "artists": Path(artists_dest.name),
+                "paintings": Path(paintings_dest.name),
+            },
+        )
+        train_artists = pd.read_csv(training_data["artists"])
+        train_paintings = pd.read_csv(training_data["paintings"])
 
     # Artists, a parent table, should have 1 additional row
-    assert len(training_data["artists"]) == len(art.get_table_data("artists")) + 1
+    assert len(train_artists) == len(art.get_table_data("artists")) + 1
     # The last record has the artifical max PK
-    assert training_data["artists"]["self|id"].to_list() == [0, 1, 2, 3, 200]
+    assert train_artists["self|id"].to_list() == [0, 1, 2, 3, 200]
     # We do not assert on the value of "self|name" because the artificial max PK record is
     # randomly sampled from source and so the exact value is not deterministic
 
     # Paintings, as a child table, should have 3 additional rows
     # - artificial max PK
     # - artificial min FKs
     # - artificial max FKs
-    assert len(training_data["paintings"]) == len(art.get_table_data("paintings")) + 3
+    assert len(train_paintings) == len(art.get_table_data("paintings")) + 3
 
-    last_three = training_data["paintings"].tail(3)
+    last_three = train_paintings.tail(3)
     last_two = last_three.tail(2)
 
     # PKs are max, +1, +2
     assert last_three["self|id"].to_list() == [350, 351, 352]
     # FKs on last two rows (artifical FKs) are min, max
     assert last_two["self|artist_id"].to_list() == [0, 200]
     assert last_two["self.artist_id|id"].to_list() == [0, 200]
 
 
 def test_prepare_training_data_with_composite_keys(tpch):
     strategy = AncestralStrategy()
-    training_data = strategy.prepare_training_data(tpch, tpch.list_all_tables())
+    with tempfile.NamedTemporaryFile() as supplier_dest, tempfile.NamedTemporaryFile() as part_dest, tempfile.NamedTemporaryFile() as partsupp_dest, tempfile.NamedTemporaryFile() as lineitem_dest:
+        training_data = strategy.prepare_training_data(
+            tpch,
+            {
+                "supplier": Path(supplier_dest.name),
+                "part": Path(part_dest.name),
+                "partsupp": Path(partsupp_dest.name),
+                "lineitem": Path(lineitem_dest.name),
+            },
+        )
+
+        train_partsupp = pd.read_csv(training_data["partsupp"])
+        train_lineitem = pd.read_csv(training_data["lineitem"])
 
     l_max = len(tpch.get_table_data("lineitem")) * 50
     ps_max = len(tpch.get_table_data("partsupp")) * 50
     p_max = len(tpch.get_table_data("part")) * 50
     s_max = len(tpch.get_table_data("supplier")) * 50
 
     # partsupp table, composite PK
-    train_partsupp = training_data["partsupp"]
     assert set(train_partsupp.columns) == {
         "self|ps_partkey",
         "self|ps_suppkey",
         "self|ps_availqty",
         "self.ps_partkey|p_partkey",
         "self.ps_suppkey|s_suppkey",
     }
@@ -185,15 +235,14 @@
                 "self|ps_partkey": [ps_max, 0, p_max],
                 "self|ps_suppkey": [ps_max, 0, s_max],
             }
         ),
     )
 
     # lineitem table, composite FK to partsupp
-    train_lineitem = training_data["lineitem"]
     assert set(train_lineitem.columns) == {
         "self|l_partkey",
         "self|l_suppkey",
         "self|l_quantity",
         "self.l_partkey+l_suppkey|ps_partkey",
         "self.l_partkey+l_suppkey|ps_suppkey",
         "self.l_partkey+l_suppkey|ps_availqty",
```

### Comparing `gretel-trainer-0.8.2/tests/relational/test_ancestry.py` & `gretel-trainer-0.9.0/tests/relational/test_ancestry.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_backup.py` & `gretel-trainer-0.9.0/tests/relational/test_backup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,16 +13,20 @@
     BackupTransformsTrain,
 )
 
 
 def test_backup_relational_data(trips):
     expected = BackupRelationalData(
         tables={
-            "vehicle_types": BackupRelationalDataTable(primary_key=["id"]),
-            "trips": BackupRelationalDataTable(primary_key=["id"]),
+            "vehicle_types": BackupRelationalDataTable(
+                primary_key=["id"],
+            ),
+            "trips": BackupRelationalDataTable(
+                primary_key=["id"],
+            ),
         },
         foreign_keys=[
             BackupForeignKey(
                 table="trips",
                 constrained_columns=["vehicle_type_id"],
                 referred_table="vehicle_types",
                 referred_columns=["id"],
```

### Comparing `gretel-trainer-0.8.2/tests/relational/test_common_strategy.py` & `gretel-trainer-0.9.0/tests/relational/test_common_strategy.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_connectors.py` & `gretel-trainer-0.9.0/tests/relational/test_connectors.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_independent_strategy.py` & `gretel-trainer-0.9.0/tests/relational/test_independent_strategy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,58 @@
 import json
+import os
 import tempfile
 from collections import defaultdict
 from pathlib import Path
 from unittest.mock import Mock, patch
 
 import pandas as pd
 import pandas.testing as pdtest
 
 from gretel_trainer.relational.strategies.independent import IndependentStrategy
 from gretel_trainer.relational.table_evaluation import TableEvaluation
 
 
-def test_preparing_training_data_does_not_mutate_source_data(pets, art):
-    for rel_data in [pets, art]:
-        original_tables = {
-            table: rel_data.get_table_data(table).copy()
-            for table in rel_data.list_all_tables()
-        }
-
-        strategy = IndependentStrategy()
-        strategy.prepare_training_data(rel_data, rel_data.list_all_tables())
-
-        for table in rel_data.list_all_tables():
-            pdtest.assert_frame_equal(
-                original_tables[table], rel_data.get_table_data(table)
-            )
+def test_preparing_training_data_does_not_mutate_source_data(pets):
+    original_tables = {
+        table: pets.get_table_data(table).copy() for table in pets.list_all_tables()
+    }
+
+    strategy = IndependentStrategy()
+
+    with tempfile.NamedTemporaryFile() as pets_dest, tempfile.NamedTemporaryFile() as humans_dest:
+        strategy.prepare_training_data(
+            pets, {"pets": Path(pets_dest.name), "humans": Path(humans_dest.name)}
+        )
+
+    for table in pets.list_all_tables():
+        pdtest.assert_frame_equal(original_tables[table], pets.get_table_data(table))
 
 
 def test_prepare_training_data_removes_primary_and_foreign_keys(pets):
     strategy = IndependentStrategy()
 
-    training_data = strategy.prepare_training_data(pets, pets.list_all_tables())
+    with tempfile.NamedTemporaryFile() as pets_dest, tempfile.NamedTemporaryFile() as humans_dest:
+        training_data = strategy.prepare_training_data(
+            pets, {"pets": Path(pets_dest.name), "humans": Path(humans_dest.name)}
+        )
+        train_pets = pd.read_csv(training_data["pets"])
 
-    assert set(training_data["pets"].columns) == {"name", "age"}
+    assert set(train_pets.columns) == {"name", "age"}
 
 
 def test_prepare_training_data_subset_of_tables(pets):
     strategy = IndependentStrategy()
 
-    training_data = strategy.prepare_training_data(pets, ["humans"])
-
-    assert set(training_data.keys()) == {"humans"}
+    with tempfile.NamedTemporaryFile() as pets_dest, tempfile.NamedTemporaryFile() as humans_dest:
+        training_data = strategy.prepare_training_data(
+            pets, {"humans": Path(humans_dest.name)}
+        )
+        assert not pd.read_csv(training_data["humans"]).empty
+        assert os.stat(pets_dest.name).st_size == 0
 
 
 def test_retraining_a_set_of_tables_only_retrains_those_tables(ecom):
     strategy = IndependentStrategy()
     assert set(strategy.tables_to_retrain(["users"], ecom)) == {"users"}
     assert set(strategy.tables_to_retrain(["users", "events"], ecom)) == {
         "users",
```

### Comparing `gretel-trainer-0.8.2/tests/relational/test_multi_table_config_options.py` & `gretel-trainer-0.9.0/tests/relational/test_multi_table_config_options.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_multi_table_restore.py` & `gretel-trainer-0.9.0/tests/relational/test_multi_table_restore.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,33 +273,53 @@
         local_file(setup_path, "synthetics_training_archive"), "w:gz"
     ) as tar:
         for table in rel_data.list_all_tables():
             table_path = setup_path / f"synthetics_train_{table}.csv"
             rel_data.get_table_data(table).to_csv(table_path, index=False)
             tar.add(table_path, arcname=f"synthetics_train_{table}.csv")
 
+    # Reports
+    for table in rel_data.list_all_tables():
+        for kind in ["individual", "cross_table"]:
+            html_filename = f"synthetics_{kind}_evaluation_{table}.html"
+            html_path = setup_path / html_filename
+            with open(html_path, "w") as f:
+                f.write("<html></html>")
+            json_filename = f"synthetics_{kind}_evaluation_{table}.json"
+            json_path = setup_path / json_filename
+            with open(json_path, "w") as f:
+                json.dump(_report_json_dict, f)
+
     # Synthetics output archive
-    with tarfile.open(
-        local_file(setup_path, "synthetics_outputs_archive"), "w:gz"
-    ) as tar:
-        for table in rel_data.list_all_tables():
-            table_path = setup_path / f"synth_{table}.csv"
-            rel_data.get_table_data(table).to_csv(table_path, index=False)
-            tar.add(table_path, arcname=f"run-id/synth_{table}.csv")
-            for kind in ["individual", "cross_table"]:
-                html_filename = f"synthetics_{kind}_evaluation_{table}.html"
-                html_path = setup_path / html_filename
-                with open(html_path, "w") as f:
-                    f.write("<html></html>")
-                tar.add(html_path, arcname=f"run-id/{html_filename}")
-                json_filename = f"synthetics_{kind}_evaluation_{table}.json"
-                json_path = setup_path / json_filename
-                with open(json_path, "w") as f:
-                    json.dump(_report_json_dict, f)
-                tar.add(json_path, arcname=f"run-id/{json_filename}")
+    # Create a subdirectory with the run outputs
+    setup_run_path = setup_path / "run-id"
+    os.makedirs(setup_run_path)
+    for table in rel_data.list_all_tables():
+        table_path = setup_run_path / f"synth_{table}.csv"
+        rel_data.get_table_data(table).to_csv(table_path, index=False)
+        for kind in ["individual", "cross_table"]:
+            html_filename = f"synthetics_{kind}_evaluation_{table}.html"
+            json_filename = f"synthetics_{kind}_evaluation_{table}.json"
+            shutil.copy(setup_path / html_filename, setup_run_path / html_filename)
+            shutil.copy(setup_path / json_filename, setup_run_path / json_filename)
+
+    with tempfile.TemporaryDirectory() as tmpdir:
+        runtar = Path(tmpdir) / "run-id"
+        # Create the archive for this run...
+        shutil.make_archive(
+            base_name=str(runtar),
+            format="gztar",
+            root_dir=setup_run_path,
+        )
+
+        # ...and add it to the outputs archive
+        with tarfile.open(
+            local_file(setup_path, "synthetics_outputs_archive"), "w:gz"
+        ) as tar:
+            tar.add(f"{runtar}.tar.gz", arcname="run-id.tar.gz")
 
 
 # For non-archive files, we patch Project#get_artifact_link to return paths to files
 # in the test setup dir in place of HTTPS links (smart_open can treat these identically).
 # For tar files, though, which require using requests, we patch the entire download_tar_artifact function
 def configure_mocks(
     project: Mock,
```

### Comparing `gretel-trainer-0.8.2/tests/relational/test_relational_data.py` & `gretel-trainer-0.9.0/tests/relational/test_relational_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     assert mutagenesis.get_primary_key("atom") == ["atom_id"]
 
     assert set(mutagenesis.get_all_key_columns("bond")) == {"atom1_id", "atom2_id"}
     assert set(mutagenesis.get_all_key_columns("atom")) == {"atom_id", "molecule_id"}
 
 
 def test_column_metadata(pets):
-    assert pets.get_table_columns("humans") == {"id", "name", "city"}
+    assert pets.get_table_columns("humans") == ["id", "name", "city"]
 
     # Name is a highly unique categorical field, so is excluded
     assert pets.get_safe_ancestral_seed_columns("humans") == {"id", "city"}
 
     # Update the table data such that:
     # - id is highly unique categorical, but still the PK
     # - name is no longer highly unique
@@ -198,15 +198,15 @@
     with pytest.raises(MultiTableException):
         ecom.set_primary_key(table="users", primary_key="not_a_column")
 
 
 def test_get_subset_of_data(pets):
     normal_length = len(pets.get_table_data("humans"))
     subset = pets.get_table_data("humans", ["name", "city"])
-    assert set(subset.columns) == {"name", "city"}
+    assert list(subset.columns) == ["name", "city"]
     assert len(subset) == normal_length
 
 
 def test_list_tables_parents_before_children(ecom):
     def in_order(col, t1, t2):
         return col.index(t1) < col.index(t2)
```

### Comparing `gretel-trainer-0.8.2/tests/relational/test_relational_data_with_json.py` & `gretel-trainer-0.9.0/tests/relational/test_relational_data_with_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 import pandas as pd
 import pandas.testing as pdtest
 import pytest
 
-from gretel_trainer.relational.core import (
-    ForeignKey,
-    MultiTableException,
-    RelationalData,
-    Scope,
-)
+from gretel_trainer.relational.core import ForeignKey, RelationalData, Scope
 from gretel_trainer.relational.json import get_json_columns
 
 
 @pytest.fixture
 def bball():
     bball_jsonl = """
     {"name": "LeBron James", "age": 38, "draft": {"year": 2003}, "teams": ["Cavaliers", "Heat", "Lakers"], "suspensions": []}
@@ -155,40 +150,40 @@
         "bball-teams-sfx",
     }
     assert set(bball.list_all_tables()) == {"bball-sfx", "bball-teams-sfx"}
 
 
 def test_invented_json_column_names(documents, bball):
     # The root invented table adds columns for dictionary properties lifted from nested JSON objects
-    assert set(documents.get_table_columns("purchases-sfx")) == {
+    assert documents.get_table_columns("purchases-sfx") == [
         "~PRIMARY_KEY_ID~",
         "id",
         "user_id",
         "data>item",
         "data>cost",
         "data>details>color",
-    }
+    ]
 
     # JSON lists lead to invented child tables. These tables store the original content,
     # a new primary key, a foreign key back to the parent, and the original array index
-    assert set(documents.get_table_columns("purchases-data-years-sfx")) == {
-        "content",
+    assert documents.get_table_columns("purchases-data-years-sfx") == [
         "~PRIMARY_KEY_ID~",
         "purchases~id",
+        "content",
         "array~order",
-    }
+    ]
 
     # If the source table does not have a primary key defined, one is created on the root invented table
-    assert set(bball.get_table_columns("bball-sfx")) == {
+    assert bball.get_table_columns("bball-sfx") == [
+        "~PRIMARY_KEY_ID~",
         "name",
         "age",
         "draft>year",
         "draft>college",
-        "~PRIMARY_KEY_ID~",
-    }
+    ]
 
 
 def test_primary_key(documents, bball):
     # The root invented table's primary key is a composite key that includes the source PK and an invented column
     assert documents.get_primary_key("purchases") == ["id"]
     assert documents.get_primary_key("purchases-sfx") == ["id", "~PRIMARY_KEY_ID~"]
 
@@ -667,43 +662,43 @@
         "demo-sfx",
         "demo-d-sfx",
         "demo-e-sfx",
         "demo-f-sfx",
         "demo-f-content-ff-sfx",
     }
 
-    assert rel_data.get_table_columns("demo-sfx") == {
+    assert rel_data.get_table_columns("demo-sfx") == [
+        "~PRIMARY_KEY_ID~",
         "a",
         "b>bb",
         "c>cc>ccc",
-        "~PRIMARY_KEY_ID~",
-    }
-    assert rel_data.get_table_columns("demo-d-sfx") == {
-        "content",
+    ]
+    assert rel_data.get_table_columns("demo-d-sfx") == [
         "~PRIMARY_KEY_ID~",
         "demo~id",
+        "content",
         "array~order",
-    }
-    assert rel_data.get_table_columns("demo-e-sfx") == {
-        "content>ee",
+    ]
+    assert rel_data.get_table_columns("demo-e-sfx") == [
         "~PRIMARY_KEY_ID~",
         "demo~id",
         "array~order",
-    }
-    assert rel_data.get_table_columns("demo-f-sfx") == {
+        "content>ee",
+    ]
+    assert rel_data.get_table_columns("demo-f-sfx") == [
         "~PRIMARY_KEY_ID~",
         "demo~id",
         "array~order",
-    }
-    assert rel_data.get_table_columns("demo-f-content-ff-sfx") == {
-        "content>fff",
+    ]
+    assert rel_data.get_table_columns("demo-f-content-ff-sfx") == [
         "~PRIMARY_KEY_ID~",
         "demo^f~id",
         "array~order",
-    }
+        "content>fff",
+    ]
 
     output_tables = {
         "demo-sfx": pd.DataFrame(
             data={
                 "a": [1, 2],
                 "b>bb": [3, 4],
                 "c>cc>ccc": [5, 6],
@@ -822,25 +817,25 @@
     )
     rel_data = RelationalData()
     rel_data.add_table(name="mix", primary_key=None, data=df)
     assert set(rel_data.list_all_tables()) == {
         "mix-sfx",
         "mix-lcol-sfx",
     }
-    assert set(rel_data.get_table_data("mix-sfx").columns) == {
-        "id",
+    assert rel_data.get_table_columns("mix-sfx") == [
         "~PRIMARY_KEY_ID~",
+        "id",
         "dcol>language",
-    }
-    assert set(rel_data.get_table_data("mix-lcol-sfx").columns) == {
+    ]
+    assert rel_data.get_table_columns("mix-lcol-sfx") == [
         "~PRIMARY_KEY_ID~",
+        "mix~id",
         "content",
         "array~order",
-        "mix~id",
-    }
+    ]
 
 
 def test_all_tables_are_present_in_debug_summary(documents):
     assert documents.debug_summary() == {
         "foreign_key_count": 4,
         "max_depth": 2,
         "public_table_count": 3,
```

### Comparing `gretel-trainer-0.8.2/tests/relational/test_report.py` & `gretel-trainer-0.9.0/tests/relational/test_report.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_synthetics_run_task.py` & `gretel-trainer-0.9.0/tests/relational/test_synthetics_run_task.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_task_runner.py` & `gretel-trainer-0.9.0/tests/relational/test_task_runner.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/relational/test_train_transforms.py` & `gretel-trainer-0.9.0/tests/relational/test_train_transforms.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/test_benchmark.py` & `gretel-trainer-0.9.0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `gretel-trainer-0.8.2/tests/test_strategy.py` & `gretel-trainer-0.9.0/tests/test_strategy.py`

 * *Files identical despite different names*

