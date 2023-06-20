# Comparing `tmp/kedro_snowflake-0.1.2.tar.gz` & `tmp/kedro_snowflake-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_snowflake-0.1.2.tar", max compression
+gzip compressed data, was "kedro_snowflake-0.2.0.tar", max compression
```

## Comparing `kedro_snowflake-0.1.2.tar` & `kedro_snowflake-0.2.0.tar`

### file list

```diff
@@ -1,66 +1,68 @@
--rw-r--r--   0        0        0    11338 2023-05-05 10:45:27.909912 kedro_snowflake-0.1.2/LICENSE
--rw-r--r--   0        0        0     4510 2023-05-05 10:45:27.909912 kedro_snowflake-0.1.2/README.md
--rw-r--r--   0        0        0       22 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/__init__.py
--rw-r--r--   0        0        0     4523 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/cli.py
--rw-r--r--   0        0        0     2282 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/cli_functions.py
--rw-r--r--   0        0        0     4444 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/config.py
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/datasets/__init__.py
--rw-r--r--   0        0        0     5483 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/datasets/internal.py
--rw-r--r--   0        0        0     5660 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/datasets/native.py
--rw-r--r--   0        0        0    14301 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/generator.py
--rw-r--r--   0        0        0      119 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/misc.py
--rw-r--r--   0        0        0     3504 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/pipeline.py
--rw-r--r--   0        0        0     1526 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/runner.py
--rw-r--r--   0        0        0     1612 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/README.md
--rw-r--r--   0        0        0      524 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/cookiecutter.json
--rw-r--r--   0        0        0   162747 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
--rw-r--r--   0        0        0   162747 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
--rw-r--r--   0        0        0     1927 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/prompts.yml
--rw-r--r--   0        0        0     1785 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0        0        0     3958 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
--rw-r--r--   0        0        0     1083 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
--rw-r--r--   0        0        0     2778 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0        0        0      901 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
--rw-r--r--   0        0        0      232 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
--rw-r--r--   0        0        0     2073 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0        0        0      431 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
--rw-r--r--   0        0        0  1810602 2023-05-05 10:45:27.925912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
--rw-r--r--   0        0        0  2937144 2023-05-05 10:45:27.937912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
--rw-r--r--   0        0        0  4195290 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
--rw-r--r--   0        0        0     6967 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0        0        0      459 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0        0        0      446 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
--rw-r--r--   0        0        0      433 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0        0        0     1198 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
--rw-r--r--   0        0        0     1109 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
--rw-r--r--   0        0        0       60 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0        0        0     1527 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0        0        0      423 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
--rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rwxr-xr-x   0        0        0      117 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
--rwxr-xr-x   0        0        0     2607 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
--rwxr-xr-x   0        0        0     1192 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
--rwxr-xr-x   0        0        0      114 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
--rwxr-xr-x   0        0        0     1712 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
--rwxr-xr-x   0        0        0      866 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
--rw-r--r--   0        0        0     1363 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0        0        0      263 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters.py
--rw-r--r--   0        0        0     5272 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/utils.py
--rw-r--r--   0        0        0     1712 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5762 1970-01-01 00:00:00.000000 kedro_snowflake-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-06-20 14:50:08.660277 kedro_snowflake-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4805 2023-06-20 14:50:08.660277 kedro_snowflake-0.2.0/README.md
+-rw-r--r--   0        0        0       22 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/__init__.py
+-rw-r--r--   0        0        0     4523 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/cli.py
+-rw-r--r--   0        0        0     2282 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/cli_functions.py
+-rw-r--r--   0        0        0     5479 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/datasets/__init__.py
+-rw-r--r--   0        0        0     5483 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/datasets/internal.py
+-rw-r--r--   0        0        0     5660 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/datasets/native.py
+-rw-r--r--   0        0        0    18339 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/generator.py
+-rw-r--r--   0        0        0      119 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/misc.py
+-rw-r--r--   0        0        0     3504 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/pipeline.py
+-rw-r--r--   0        0        0     1526 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/runner.py
+-rw-r--r--   0        0        0     1612 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/README.md
+-rw-r--r--   0        0        0      595 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/cookiecutter.json
+-rw-r--r--   0        0        0   162747 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0   162747 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0     2339 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/prompts.yml
+-rw-r--r--   0        0        0     1785 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0        0        0     3958 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
+-rw-r--r--   0        0        0     1083 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
+-rw-r--r--   0        0        0     2778 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0        0        0      901 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
+-rw-r--r--   0        0        0      232 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+-rw-r--r--   0        0        0     4375 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0        0        0      431 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+-rw-r--r--   0        0        0  1810602 2023-06-20 14:50:08.684277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
+-rw-r--r--   0        0        0  2937144 2023-06-20 14:50:08.700277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
+-rw-r--r--   0        0        0  4195290 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+-rw-r--r--   0        0        0     6967 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0        0        0      459 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0        0        0      446 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
+-rw-r--r--   0        0        0      552 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0        0        0     1198 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+-rw-r--r--   0        0        0       60 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0        0        0     1527 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0        0        0      967 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/hooks.py
+-rw-r--r--   0        0        0      423 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+-rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rwxr-xr-x   0        0        0      117 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
+-rwxr-xr-x   0        0        0     1192 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
+-rwxr-xr-x   0        0        0      114 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
+-rwxr-xr-x   0        0        0     2368 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
+-rwxr-xr-x   0        0        0      866 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
+-rw-r--r--   0        0        0     3737 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/mlflow_helpers.py
+-rw-r--r--   0        0        0     1370 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0        0        0      263 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/starters.py
+-rw-r--r--   0        0        0     5272 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/utils.py
+-rw-r--r--   0        0        0     1803 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 kedro_snowflake-0.2.0/PKG-INFO
```

### Comparing `kedro_snowflake-0.1.2/LICENSE` & `kedro_snowflake-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/README.md` & `kedro_snowflake-0.2.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 2. Create new project with our Kedro starter ❄️ _Snowflights_ 🚀:
     ```bash
     kedro new --starter=snowflights --checkout=master
     ```
     <details>
         <summary>And answer the interactive prompts ⬇️ (click to expand) </summary>
     
-    ```bash
+    ```
     Project Name
     ============
     Please enter a human readable name for your new project.
     Spaces, hyphens, and underscores are allowed.
      [Snowflights]: 
     
     Snowflake Account
@@ -62,30 +62,40 @@
     ===================
     Please enter the name of your Snowflake warehouse.
      []: compute-wh
     
     Snowflake Database
     ==================
     Please enter the name of your Snowflake database.
-     [KEDRO]: 
+     [DEMO]: 
     
     Snowflake Schema
     ================
     Please enter the name of your Snowflake schema.
-     [PUBLIC]: 
+     [DEMO]: 
     
     Snowflake Password Environment Variable
     =======================================
     Please enter the name of the environment variable that contains your Snowflake password.
-    Alternatively, you can re-configure the plugin later to use Kedro's credentials.yml
+    Alternatively, you can re-configure the plugin later to use Kedros credentials.yml
      [SNOWFLAKE_PASSWORD]:       
     
+    Pipeline Name Used As A Snowflake Task Prefix
+    =============================================
+
+     [default]:
+
+    Enable Mlflow Integration (See Documentation For The Configuration Instructions)
+    ================================================================================
+
+     [False]: 
+
     The project name 'Snowflights' has been applied to: 
-    - The project title in /tmp/snowflights/README.md 
-    - The folder created for your project in /tmp/snowflights 
+    - The project title in /tmp/snowflights/README.md
+    - The folder created for your project in /tmp/snowflights
     - The project's python package in /tmp/snowflights/src/snowflights
     ```
     </details>
 
 3. Run the project
     ```bash
     cd snowflights
```

#### html2text {}

```diff
@@ -23,29 +23,33 @@
 fully within Snowflake, without external system * using Kedro's official
 `SnowparkTableDataSet` * automatically storing intermediate data as Transient
 Tables (if Snowpark's DataFrames are used) ## Documentation For detailed
 documentation refer to https://kedro-snowflake.readthedocs.io/ ## Usage ###
 With starter 1. Install the plugin ```bash pip install "kedro-snowflake>=0.1.0"
 ``` 2. Create new project with our Kedro starter âï¸ _Snowflights_ ð:
 ```bash kedro new --starter=snowflights --checkout=master ```  And answer the
-interactive prompts â¬ï¸ (click to expand)  ```bash Project Name ============
+interactive prompts â¬ï¸ (click to expand)  ``` Project Name ============
 Please enter a human readable name for your new project. Spaces, hyphens, and
 underscores are allowed. [Snowflights]: Snowflake Account =================
 Please enter the name of your Snowflake account. This is the part of the URL
 before .snowflakecomputing.com []: abc-123 Snowflake User ============== Please
 enter the name of your Snowflake user. []: user2137 Snowflake Warehouse
 =================== Please enter the name of your Snowflake warehouse. []:
 compute-wh Snowflake Database ================== Please enter the name of your
-Snowflake database. [KEDRO]: Snowflake Schema ================ Please enter the
-name of your Snowflake schema. [PUBLIC]: Snowflake Password Environment
-Variable ======================================= Please enter the name of the
+Snowflake database. [DEMO]: Snowflake Schema ================ Please enter the
+name of your Snowflake schema. [DEMO]: Snowflake Password Environment Variable
+======================================= Please enter the name of the
 environment variable that contains your Snowflake password. Alternatively, you
-can re-configure the plugin later to use Kedro's credentials.yml
-[SNOWFLAKE_PASSWORD]: The project name 'Snowflights' has been applied to: - The
-project title in /tmp/snowflights/README.md - The folder created for your
-project in /tmp/snowflights - The project's python package in /tmp/snowflights/
-src/snowflights ```  3. Run the project ```bash cd snowflights kedro snowflake
-run --wait-for-completion ``` ### In existing Kedro project 1. Install the
-plugin ```bash pip install "kedro-snowflake>=0.1.0" ``` 2. Initialize the
-plugin ```bash kedro snowflake init       ``` 3. Run the project ```bash kedro
+can re-configure the plugin later to use Kedros credentials.yml
+[SNOWFLAKE_PASSWORD]: Pipeline Name Used As A Snowflake Task Prefix
+============================================= [default]: Enable Mlflow
+Integration (See Documentation For The Configuration Instructions)
+================================================================================
+[False]: The project name 'Snowflights' has been applied to: - The project
+title in /tmp/snowflights/README.md - The folder created for your project in /
+tmp/snowflights - The project's python package in /tmp/snowflights/src/
+snowflights ```  3. Run the project ```bash cd snowflights kedro snowflake run
+--wait-for-completion ``` ### In existing Kedro project 1. Install the plugin
+```bash pip install "kedro-snowflake>=0.1.0" ``` 2. Initialize the plugin
+```bash kedro snowflake init       ``` 3. Run the project ```bash kedro
 snowflake run --wait-for-completion ``` ### Kedro pipeline in Snowflake Tasks
 [Kedro Snowflake Plugin] Execution: [Kedro Snowflake Plugin CLI]
```

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/cli.py` & `kedro_snowflake-0.2.0/kedro_snowflake/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/cli_functions.py` & `kedro_snowflake-0.2.0/kedro_snowflake/cli_functions.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/config.py` & `kedro_snowflake-0.2.0/kedro_snowflake/config.py`

 * *Files 22% similar despite different names*

```diff
@@ -39,14 +39,15 @@
             )
         return values
 
 
 class DependenciesConfig(BaseModel):
     packages: List[str] = [
         "snowflake-snowpark-python",
+        "mlflow",
         "cachetools",
         "pluggy",
         "PyYAML==6.0",
         "jmespath",
         "click",
         "importlib_resources",
         "toml",
@@ -76,17 +77,33 @@
     stage: str = "@KEDRO_SNOWFLAKE_STAGE"
     temporary_stage: str = "@KEDRO_SNOWFLAKE_TEMP_DATA_STAGE"
     schedule: str = "11520 minute"
     stored_procedure_name_suffix: Optional[str] = ""
     pipeline_name_mapping: Optional[Dict[str, str]] = {"__default__": "default"}
 
 
+class MLflowFunctionsConfig(BaseModel):
+    experiment_get_by_name: str = "mlflow_experiment_get_by_name"
+    run_create: str = "mlflow_run_create"
+    run_update: str = "mlflow_run_update"
+    run_log_metric: str = "mlflow_run_log_metric"
+    run_log_parameter: str = "mlflow_run_log_parameter"
+
+
+class SnowflakeMLflowConfig(BaseModel):
+    experiment_name: Optional[str]
+    functions: MLflowFunctionsConfig
+    run_id: Optional[str]
+    stage: Optional[str]
+
+
 class SnowflakeConfig(BaseModel):
     connection: SnowflakeConnectionConfig
     runtime: SnowflakeRuntimeConfig
+    mlflow: Optional[SnowflakeMLflowConfig]
 
 
 class KedroSnowflakeConfig(BaseModel):
     snowflake: SnowflakeConfig
 
 
 CONFIG_TEMPLATE_YAML = """
@@ -132,14 +149,15 @@
       - antlr4
       - dynaconf
       - anyconfig
       # packages use official Snowflake's Conda Channel
       # https://repo.anaconda.com/pkgs/snowflake/
       packages:
       - snowflake-snowpark-python
+      - mlflow
       - cachetools
       - pluggy
       - PyYAML==6.0
       - jmespath
       - click
       - importlib_resources
       - toml
@@ -148,14 +166,27 @@
       - fsspec
       - scikit-learn
       - pandas
       - zstandard
       - more-itertools
       - openpyxl
       - backoff
+      - pydantic
     # Optionally provide mapping for user-friendly pipeline names
     pipeline_name_mapping:
      __default__: default
+  # EXPERIMENTAL: Either MLflow experiment name to enable MLflow tracking
+  # or leave empty
+#   mlflow:
+#     experiment_name: ~
+#     stage: ~
+    # Snowflake external functions needed for calling MLflow instance
+#     functions:
+#         experiment_get_by_name: mlflow_experiment_get_by_name
+#         run_create: mlflow_run_create
+#         run_update: mlflow_run_update
+#         run_log_metric: mlflow_run_log_metric
+#         run_log_parameter: mlflow_run_log_parameter
 """.strip()
 
 # This auto-validates the template above during import
 _CONFIG_TEMPLATE = KedroSnowflakeConfig.parse_obj(yaml.safe_load(CONFIG_TEMPLATE_YAML))
```

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/datasets/internal.py` & `kedro_snowflake-0.2.0/kedro_snowflake/datasets/internal.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/datasets/native.py` & `kedro_snowflake-0.2.0/kedro_snowflake/datasets/native.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/generator.py` & `kedro_snowflake-0.2.0/kedro_snowflake/generator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import os
 import re
 import tempfile
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Dict, List, Optional
@@ -55,14 +56,20 @@
         self.kedro_environment = kedro_environment
 
         self.extra_params = extra_params
         self.kedro_params = kedro_params
         self.config = config
         self.pipeline_name = pipeline_name
         self.extra_env = extra_env
+        self.mlflow_enabled = (
+            True
+            if self.config.snowflake.mlflow
+            and self.config.snowflake.mlflow.experiment_name
+            else False
+        )
 
     def _get_pipeline_name_for_snowflake(self):
         return (self.config.snowflake.runtime.pipeline_name_mapping or {}).get(
             self.pipeline_name, self.pipeline_name
         )
 
     def _generate_task_sql(
@@ -74,15 +81,17 @@
         extra_params: Optional[str] = None,
     ):
         return self.TASK_TEMPLATE.format(
             task_name=task_name,
             warehouse=self.connection_parameters["warehouse"],
             after_tasks=",".join(after_tasks),
             task_body=self.TASK_BODY_TEMPLATE.format(
-                root_task_name=self._root_task_name,
+                root_task_name=self._root_task_name
+                if not self.mlflow_enabled
+                else self._mlflow_root_task_name,
                 environment=self.kedro_environment,
                 sproc_name=self.SPROC_NAME,
                 pipeline_name=pipeline_name,
                 nodes_to_run=",".join(f"'{n}'" for n in nodes_to_run),
                 extra_params=extra_params or "",
             ),
         )
@@ -97,58 +106,109 @@
 """.strip().format(
             task_name=self._root_task_name,
             warehouse=self.connection_parameters["warehouse"],
             root_sproc=self._root_sproc_name,
             schedule=self.config.snowflake.runtime.schedule,
         )
 
-    def _sanitize_node_name(self, node_name: str) -> str:
-        return re.sub(r"\W", "_", node_name)
+    def _generate_root_task_suspend_sql(self):
+        return """
+alter task {task_name} suspend;
+        """.strip().format(
+            task_name=self._root_task_name
+        )
+
+    def _generate_mlflow_drop_task_sql(self):
+        return """
+drop task if exists {task_name};
+        """.strip().format(
+            task_name=self._mlflow_root_task_name
+        )
+
+    def _generate_mlflow_root_task_sql(self):
+        return """
+create or replace task {task_name}
+warehouse = '{warehouse}'
+after {after_task}
+as
+call {root_sproc}();
+""".strip().format(
+            task_name=self._mlflow_root_task_name,
+            warehouse=self.connection_parameters["warehouse"],
+            root_sproc=self._mlflow_root_sproc_name,
+            after_task=self._root_task_name,
+        )
+
+    def _standardize_node_name(self, node_name: str) -> str:
+        sanity_node_name = re.sub(r"\W", "_", node_name)
+        return f"kedro_{self._get_pipeline_name_for_snowflake()}_{sanity_node_name}"
 
     def _generate_snowflake_tasks_sql(
         self,
         pipeline: Pipeline,
     ) -> List[str]:
-        sql_statements = [self._generate_root_task_sql()]
+        sql_statements = [
+            self._generate_root_task_sql(),
+            self._generate_root_task_suspend_sql(),
+        ]
+        if self.mlflow_enabled:
+            sql_statements.append(self._generate_mlflow_root_task_sql())
+        else:
+            sql_statements.append(self._generate_mlflow_drop_task_sql())
 
         node_dependencies = (
             pipeline.node_dependencies
         )  # <-- this one is not topological
         for node in pipeline.nodes:  # <-- this one is topological
             after_tasks = [self._root_task_name] + [
-                self._sanitize_node_name(n.name) for n in node_dependencies[node]
+                f"{self._standardize_node_name(n.name)}"
+                for n in node_dependencies[node]
             ]
+            if self.mlflow_enabled:
+                after_tasks.append(self._mlflow_root_task_name)
             sql_statements.append(
                 self._generate_task_sql(
-                    self._sanitize_node_name(node.name),
+                    self._standardize_node_name(node.name),
                     after_tasks,
                     self.pipeline_name,
                     [node.name],
                     self.extra_params,
                 )
             )
+
         return sql_statements
 
     def _generate_task_execute_sql(self):
         return [
             f"call SYSTEM$TASK_DEPENDENTS_ENABLE( '{self._root_task_name}' );",
             f"alter task {self._root_task_name} resume;",
             f"execute task {self._root_task_name};",
         ]
 
     @property
     def _root_task_name(self):
-        root_task_name = f"kedro_snowflake_start_{self._get_pipeline_name_for_snowflake()}_task".upper()
+        root_task_name = (
+            f"kedro_{self._get_pipeline_name_for_snowflake()}_start_task".upper()
+        )
         return root_task_name
 
     @property
-    def _root_sproc_name(self):
-        return (
-            f"kedro_snowflake_start_{self._get_pipeline_name_for_snowflake()}".upper()
+    def _mlflow_root_task_name(self):
+        mlflow_root_task_name = (
+            f"kedro_{self._get_pipeline_name_for_snowflake()}_mlflow_start_task".upper()
         )
+        return mlflow_root_task_name
+
+    @property
+    def _root_sproc_name(self):
+        return f"kedro_{self._get_pipeline_name_for_snowflake()}_start".upper()
+
+    @property
+    def _mlflow_root_sproc_name(self):
+        return f"kedro_{self._get_pipeline_name_for_snowflake()}_start_mlflow".upper()
 
     def generate(self) -> KedroSnowflakePipeline:
         """Generate a SnowflakePipeline object from a Kedro pipeline.
         It can be used to run the pipeline or just to get the SQL statements.
         Note that the pipeline is not executed, it is just translated to SQL statements,
         but the stored procedures ARE created.
         """
@@ -198,14 +258,21 @@
             )
 
             logger.info("Creating Kedro Snowflake root sproc")
             root_sproc = self._construct_kedro_snowflake_root_sproc(  # noqa: F841
                 snowflake_stage_name
             )
 
+            if self.mlflow_enabled:
+                mlflow_root_sproc = (  # noqa: F841
+                    self._construct_kedro_snowflake_mlflow_root_sproc(
+                        snowflake_stage_name
+                    )
+                )
+
             logger.info("Creating Kedro Snowflake Sproc")
             snowflake_sproc = self._construct_kedro_snowflake_sproc(
                 imports=self._generate_imports_for_sproc(
                     dependencies_dir, snowflake_stage_name
                 ),
                 packages=self.config.snowflake.runtime.dependencies.packages,
                 stage_location=snowflake_stage_name,
@@ -215,15 +282,15 @@
             logger.debug(snowflake_sproc)
             pipeline_sql_statements = self._generate_snowflake_tasks_sql(pipeline)
             return KedroSnowflakePipeline(
                 session,
                 pipeline_sql_statements,
                 self._generate_task_execute_sql(),
                 self._root_task_name,
-                [self._sanitize_node_name(n.name) for n in pipeline.nodes],
+                [self._standardize_node_name(n.name) for n in pipeline.nodes],
             )
 
     def _generate_imports_for_sproc(self, dependencies_dir, snowflake_stage_name):
         imports_for_sproc = [
             f"{snowflake_stage_name}/{f.name}"
             for f in dependencies_dir.glob("*")
             if f.is_file()
@@ -266,14 +333,51 @@
             ).collect()
             self.snowflake_session.sql(f"create stage {s.lstrip('@')};").collect()
 
     @cached_property
     def snowflake_session(self):
         return Session.builder.configs(self.connection_parameters).create()
 
+    def _construct_kedro_snowflake_mlflow_root_sproc(self, stage_location: str):
+        experiment_name = self.config.snowflake.mlflow.experiment_name
+        experiment_get_by_name_func = (
+            self.config.snowflake.mlflow.functions.experiment_get_by_name
+        )
+        run_create_func = self.config.snowflake.mlflow.functions.run_create
+        experiment_id = (
+            self.snowflake_session.sql(
+                f"SELECT {experiment_get_by_name_func}('{experiment_name}'):body.experiments[0].experiment_id"
+            ).collect()[0][0]
+        ).strip(" \"'\t\r\n")
+        mlflow_config = self.config.snowflake.mlflow.dict()
+
+        def mlflow_start_run(session: Session) -> str:
+            run_id = (
+                session.sql(
+                    f"SELECT {run_create_func}({experiment_id}):body.run.info.run_id"
+                ).collect()[0][0]
+            ).strip(" \"'\t\r\n")
+            mlflow_config["run_id"] = run_id
+            mlflow_config_json = json.dumps(mlflow_config)
+            session.sql(
+                f"call system$set_return_value('{mlflow_config_json}');"
+            ).collect()
+            return run_id
+
+        return sproc(
+            func=mlflow_start_run,
+            name=self._mlflow_root_sproc_name,
+            is_permanent=True,
+            replace=True,
+            stage_location=stage_location,
+            packages=["snowflake-snowpark-python"],
+            execute_as="caller",
+            session=self.snowflake_session,
+        )
+
     def _construct_kedro_snowflake_root_sproc(self, stage_location: str):
         def kedro_start_run(session: Session) -> str:
             from uuid import uuid4
 
             run_id = uuid4().hex
             session.sql(f"call system$set_return_value('{run_id}');").collect()
             return run_id
@@ -296,14 +400,16 @@
         stage_location: str,
         temp_data_stage: str,
     ):
         # create a Snowpark Stored Procedure from Kedro node (node arg)
         # and return it
 
         project_name = Path.cwd().name
+        mlflow_task_name = self._mlflow_root_task_name
+        is_mlflow_enabled = self.mlflow_enabled
 
         def kedro_sproc_executor(
             session: Session,
             environment: str,
             run_id: str,
             pipeline_name: str,
             node_names: Optional[List[str]],
@@ -325,14 +431,20 @@
                 "environment": environment,
                 "run_id": run_id,
                 "pipeline_name": pipeline_name,
                 "node_names": node_names,
                 "extra_params_json": extra_params_json,
             }
 
+            if is_mlflow_enabled:
+                mlflow_config = session.sql(
+                    f"call system$get_predecessor_return_value('{mlflow_task_name}')"
+                ).collect()[0][0]
+                os.environ["SNOWFLAKE_MLFLOW_CONFIG"] = mlflow_config
+
             def extract_tar_zstd(input_path, output_path):
                 with zstd.open(input_path, "rb") as archive:
                     tarfile.open(fileobj=archive, mode="r|").extractall(output_path)
 
             # Extract project and special dependencies
             extract_start_ts = monotonic()
             project_file_list = [
```

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/pipeline.py` & `kedro_snowflake-0.2.0/kedro_snowflake/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/runner.py` & `kedro_snowflake-0.2.0/kedro_snowflake/runner.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/README.md` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/prompts.yml` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/prompts.yml`

 * *Files 18% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     be at least 2 characters long.
 
 snowflake_account:
   title: "Snowflake Account"
   text: |
     Please enter the name of your Snowflake account.
     This is the part of the URL before .snowflakecomputing.com
-  regex_validator: "^[A-Za-z0-9-]{2,}$"
+  regex_validator: "^[A-Za-z0-9-.]{2,}$"
   error_message: |
     It must contain only alphanumeric symbols and hyphens and
     be at least 2 characters long.
 
 snowflake_user:
   title: "Snowflake User"
   text: |
@@ -53,8 +53,20 @@
 snowflake_password_env_variable:
   title: "Snowflake Password Environment Variable"
   text: |
     Please enter the name of the environment variable that contains your Snowflake password.
     Alternatively, you can re-configure the plugin later to use Kedro's credentials.yml
   regex_validator: "^[A-Za-z0-9\\_]+$"
   error_message: |
-    It must contain only alphanumeric symbols and underscores
+    It must contain only alphanumeric symbols and underscores
+
+pipeline_name:
+  title: "Pipeline name used as a Snowflake task prefix"
+  regex_validator: "^[\\w-]+$"
+  error_message: |
+    It must contain only alphanumeric symbols and hyphens
+
+enable_mlflow_integration:
+  title: "Enable MLflow integration (see documentation for the configuration instructions)"
+  regex_validator: "^([Tt]rue|[Ff]alse|[Yy](es))"
+  error_message: |
+    Please type either 'true' or 'false'
```

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     shuttles["d_check_complete"] = _is_true(shuttles["d_check_complete"])
     shuttles["moon_clearance_complete"] = _is_true(shuttles["moon_clearance_complete"])
     shuttles["price"] = _parse_money(shuttles["price"])
     return shuttles
 
 
 def create_model_input_table(
-    shuttles: pd.DataFrame, companies: pd.DataFrame, reviews: pd.DataFrame
+    shuttles: pd.DataFrame, companies: sp.DataFrame, reviews: pd.DataFrame
 ) -> pd.DataFrame:
     """Combines all data to create a model input table.
 
     Args:
         shuttles: Preprocessed data for shuttles.
         companies: Preprocessed data for companies.
         reviews: Raw data for reviews.
```

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Project settings. There is no need to edit this file unless you want to change values
 from the Kedro defaults. For further information, including these default values, see
 https://kedro.readthedocs.io/en/stable/kedro_project_setup/settings.html."""
+from .hooks import SnowflakeHook
 
 # Instantiated project hooks.
-# from {{cookiecutter.python_package}}.hooks import ProjectHooks
-# HOOKS = (ProjectHooks(),)
+# from snowflake_mlops_demo.hooks import ProjectHooks
+HOOKS = (SnowflakeHook(),)
 
 # Installed plugins for which to disable hook auto-registration.
 # DISABLE_HOOKS_FOR_PLUGINS = ("kedro-viz",)
 
 # Class that manages storing KedroSession data.
 # from kedro.framework.session.shelvestore import ShelveStore
 # SESSION_STORE_CLASS = ShelveStore
@@ -26,15 +27,13 @@
 
 # Class that manages how configuration is loaded.
 from kedro.config import OmegaConfigLoader
 
 CONFIG_LOADER_CLASS = OmegaConfigLoader
 # Keyword arguments to pass to the `CONFIG_LOADER_CLASS` constructor.
 CONFIG_LOADER_ARGS = {
-    "config_patterns": {
-        "snowflake": ["snowflake*"],
-    },
+    "config_patterns": {"snowflake": ["snowflake*"],},
 }
 
 # Class that manages the Data Catalog.
 # from kedro.io import DataCatalog
 # DATA_CATALOG_CLASS = DataCatalog
```

### Comparing `kedro_snowflake-0.1.2/kedro_snowflake/utils.py` & `kedro_snowflake-0.2.0/kedro_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.2/pyproject.toml` & `kedro_snowflake-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-snowflake"
-version = "0.1.2"
+version = "0.2.0"
 description = "Kedro plugin with Snowflake / Snowpark support"
 readme = "README.md"
 authors = ['GetInData MLOPS <mlops@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-snowflake"
 repository = "https://github.com/getindata/kedro-snowflake"
 documentation = "https://kedro-snowflake.readthedocs.io/"
@@ -29,15 +29,16 @@
 ]
 
 [tool.isort]
 known_third_party = ["pydantic","semver","setuptools"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
-kedro = ">=0.18.7,<0.19"
+# Fixing kedro version because of problems in the snowflake datasets at kedro >= 0.18.9
+kedro = ">=0.18.7,<=0.18.8"
 snowflake-snowpark-python = {version = ">=1.0.0,<1.1.0", extras = ["pandas"]}
 backoff = "^2.2.1"
 cloudpickle = ">=1.6.0,<=2.0.0"
 zstandard = "^0.20.0"
 pydantic = "^1.10.7"
 tabulate = "^0.9.0"
 kedro-datasets = {version = ">=1.1.0", extras = ["pandas-csvdataset", "pandas-exceldataset", "pandas-parquetdataset", "snowflake-snowparktabledataset"]}
```

### Comparing `kedro_snowflake-0.1.2/PKG-INFO` & `kedro_snowflake-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-snowflake
-Version: 0.1.2
+Version: 0.2.0
 Summary: Kedro plugin with Snowflake / Snowpark support
 Home-page: https://github.com/getindata/kedro-snowflake
 License: Apache-2.0
 Keywords: kedro,snowflake,snowpark,mlops
 Author: GetInData MLOPS
 Author-email: mlops@getindata.com
 Maintainer: GetInData MLOPS
@@ -12,15 +12,15 @@
 Requires-Python: >=3.8,<3.9
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cloudpickle (>=1.6.0,<=2.0.0)
-Requires-Dist: kedro (>=0.18.7,<0.19)
+Requires-Dist: kedro (>=0.18.7,<=0.18.8)
 Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-exceldataset,pandas-parquetdataset,snowflake-snowparktabledataset] (>=1.1.0)
 Requires-Dist: pandas (>=1.3,<3.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: snowflake-snowpark-python[pandas] (>=1.0.0,<1.1.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: zstandard (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://kedro-snowflake.readthedocs.io/
@@ -65,15 +65,15 @@
 2. Create new project with our Kedro starter ❄️ _Snowflights_ 🚀:
     ```bash
     kedro new --starter=snowflights --checkout=master
     ```
     <details>
         <summary>And answer the interactive prompts ⬇️ (click to expand) </summary>
     
-    ```bash
+    ```
     Project Name
     ============
     Please enter a human readable name for your new project.
     Spaces, hyphens, and underscores are allowed.
      [Snowflights]: 
     
     Snowflake Account
@@ -91,30 +91,40 @@
     ===================
     Please enter the name of your Snowflake warehouse.
      []: compute-wh
     
     Snowflake Database
     ==================
     Please enter the name of your Snowflake database.
-     [KEDRO]: 
+     [DEMO]: 
     
     Snowflake Schema
     ================
     Please enter the name of your Snowflake schema.
-     [PUBLIC]: 
+     [DEMO]: 
     
     Snowflake Password Environment Variable
     =======================================
     Please enter the name of the environment variable that contains your Snowflake password.
-    Alternatively, you can re-configure the plugin later to use Kedro's credentials.yml
+    Alternatively, you can re-configure the plugin later to use Kedros credentials.yml
      [SNOWFLAKE_PASSWORD]:       
     
+    Pipeline Name Used As A Snowflake Task Prefix
+    =============================================
+
+     [default]:
+
+    Enable Mlflow Integration (See Documentation For The Configuration Instructions)
+    ================================================================================
+
+     [False]: 
+
     The project name 'Snowflights' has been applied to: 
-    - The project title in /tmp/snowflights/README.md 
-    - The folder created for your project in /tmp/snowflights 
+    - The project title in /tmp/snowflights/README.md
+    - The folder created for your project in /tmp/snowflights
     - The project's python package in /tmp/snowflights/src/snowflights
     ```
     </details>
 
 3. Run the project
     ```bash
     cd snowflights
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: kedro-snowflake Version: 0.1.2 Summary: Kedro
+Metadata-Version: 2.1 Name: kedro-snowflake Version: 0.2.0 Summary: Kedro
 plugin with Snowflake / Snowpark support Home-page: https://github.com/
 getindata/kedro-snowflake License: Apache-2.0 Keywords:
 kedro,snowflake,snowpark,mlops Author: GetInData MLOPS Author-email:
 mlops@getindata.com Maintainer: GetInData MLOPS Maintainer-email:
 mlops@getindata.com Requires-Python: >=3.8,<3.9 Classifier: Development Status
 :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Requires-Dist: backoff (>=2.2.1,<3.0.0) Requires-
-Dist: cloudpickle (>=1.6.0,<=2.0.0) Requires-Dist: kedro (>=0.18.7,<0.19)
+Dist: cloudpickle (>=1.6.0,<=2.0.0) Requires-Dist: kedro (>=0.18.7,<=0.18.8)
 Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-exceldataset,pandas-
 parquetdataset,snowflake-snowparktabledataset] (>=1.1.0) Requires-Dist: pandas
 (>=1.3,<3.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-Dist:
 snowflake-snowpark-python[pandas] (>=1.0.0,<1.1.0) Requires-Dist: tabulate
 (>=0.9.0,<0.10.0) Requires-Dist: zstandard (>=0.20.0,<0.21.0) Project-URL:
 Documentation, https://kedro-snowflake.readthedocs.io/ Project-URL: Repository,
 https://github.com/getindata/kedro-snowflake Description-Content-Type: text/
@@ -40,29 +40,33 @@
 fully within Snowflake, without external system * using Kedro's official
 `SnowparkTableDataSet` * automatically storing intermediate data as Transient
 Tables (if Snowpark's DataFrames are used) ## Documentation For detailed
 documentation refer to https://kedro-snowflake.readthedocs.io/ ## Usage ###
 With starter 1. Install the plugin ```bash pip install "kedro-snowflake>=0.1.0"
 ``` 2. Create new project with our Kedro starter âï¸ _Snowflights_ ð:
 ```bash kedro new --starter=snowflights --checkout=master ```  And answer the
-interactive prompts â¬ï¸ (click to expand)  ```bash Project Name ============
+interactive prompts â¬ï¸ (click to expand)  ``` Project Name ============
 Please enter a human readable name for your new project. Spaces, hyphens, and
 underscores are allowed. [Snowflights]: Snowflake Account =================
 Please enter the name of your Snowflake account. This is the part of the URL
 before .snowflakecomputing.com []: abc-123 Snowflake User ============== Please
 enter the name of your Snowflake user. []: user2137 Snowflake Warehouse
 =================== Please enter the name of your Snowflake warehouse. []:
 compute-wh Snowflake Database ================== Please enter the name of your
-Snowflake database. [KEDRO]: Snowflake Schema ================ Please enter the
-name of your Snowflake schema. [PUBLIC]: Snowflake Password Environment
-Variable ======================================= Please enter the name of the
+Snowflake database. [DEMO]: Snowflake Schema ================ Please enter the
+name of your Snowflake schema. [DEMO]: Snowflake Password Environment Variable
+======================================= Please enter the name of the
 environment variable that contains your Snowflake password. Alternatively, you
-can re-configure the plugin later to use Kedro's credentials.yml
-[SNOWFLAKE_PASSWORD]: The project name 'Snowflights' has been applied to: - The
-project title in /tmp/snowflights/README.md - The folder created for your
-project in /tmp/snowflights - The project's python package in /tmp/snowflights/
-src/snowflights ```  3. Run the project ```bash cd snowflights kedro snowflake
-run --wait-for-completion ``` ### In existing Kedro project 1. Install the
-plugin ```bash pip install "kedro-snowflake>=0.1.0" ``` 2. Initialize the
-plugin ```bash kedro snowflake init       ``` 3. Run the project ```bash kedro
+can re-configure the plugin later to use Kedros credentials.yml
+[SNOWFLAKE_PASSWORD]: Pipeline Name Used As A Snowflake Task Prefix
+============================================= [default]: Enable Mlflow
+Integration (See Documentation For The Configuration Instructions)
+================================================================================
+[False]: The project name 'Snowflights' has been applied to: - The project
+title in /tmp/snowflights/README.md - The folder created for your project in /
+tmp/snowflights - The project's python package in /tmp/snowflights/src/
+snowflights ```  3. Run the project ```bash cd snowflights kedro snowflake run
+--wait-for-completion ``` ### In existing Kedro project 1. Install the plugin
+```bash pip install "kedro-snowflake>=0.1.0" ``` 2. Initialize the plugin
+```bash kedro snowflake init       ``` 3. Run the project ```bash kedro
 snowflake run --wait-for-completion ``` ### Kedro pipeline in Snowflake Tasks
 [Kedro Snowflake Plugin] Execution: [Kedro Snowflake Plugin CLI]
```

