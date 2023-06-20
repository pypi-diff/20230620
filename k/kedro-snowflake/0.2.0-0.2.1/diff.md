# Comparing `tmp/kedro_snowflake-0.2.0.tar.gz` & `tmp/kedro_snowflake-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_snowflake-0.2.0.tar", max compression
+gzip compressed data, was "kedro_snowflake-0.2.1.tar", max compression
```

## Comparing `kedro_snowflake-0.2.0.tar` & `kedro_snowflake-0.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
--rw-r--r--   0        0        0    11338 2023-06-20 14:50:08.660277 kedro_snowflake-0.2.0/LICENSE
--rw-r--r--   0        0        0     4805 2023-06-20 14:50:08.660277 kedro_snowflake-0.2.0/README.md
--rw-r--r--   0        0        0       22 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/__init__.py
--rw-r--r--   0        0        0     4523 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/cli.py
--rw-r--r--   0        0        0     2282 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/cli_functions.py
--rw-r--r--   0        0        0     5479 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/config.py
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/datasets/__init__.py
--rw-r--r--   0        0        0     5483 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/datasets/internal.py
--rw-r--r--   0        0        0     5660 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/datasets/native.py
--rw-r--r--   0        0        0    18339 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/generator.py
--rw-r--r--   0        0        0      119 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/misc.py
--rw-r--r--   0        0        0     3504 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/pipeline.py
--rw-r--r--   0        0        0     1526 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/runner.py
--rw-r--r--   0        0        0     1612 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/README.md
--rw-r--r--   0        0        0      595 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/cookiecutter.json
--rw-r--r--   0        0        0   162747 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
--rw-r--r--   0        0        0   162747 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
--rw-r--r--   0        0        0     2339 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/prompts.yml
--rw-r--r--   0        0        0     1785 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0        0        0     3958 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
--rw-r--r--   0        0        0     1083 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
--rw-r--r--   0        0        0     2778 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0        0        0      901 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
--rw-r--r--   0        0        0      232 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
--rw-r--r--   0        0        0     4375 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0        0        0      431 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.672277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
--rw-r--r--   0        0        0  1810602 2023-06-20 14:50:08.684277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
--rw-r--r--   0        0        0  2937144 2023-06-20 14:50:08.700277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
--rw-r--r--   0        0        0  4195290 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
--rw-r--r--   0        0        0     6967 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0        0        0      459 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.732277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0        0        0      446 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0        0        0       47 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
--rw-r--r--   0        0        0      552 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0        0        0     1198 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
--rw-r--r--   0        0        0     1109 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
--rw-r--r--   0        0        0       60 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0        0        0     1527 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0        0        0      967 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/hooks.py
--rw-r--r--   0        0        0      423 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
--rw-r--r--   0        0        0        0 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rwxr-xr-x   0        0        0      117 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
--rwxr-xr-x   0        0        0     2607 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
--rwxr-xr-x   0        0        0     1192 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
--rwxr-xr-x   0        0        0      114 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
--rwxr-xr-x   0        0        0     2368 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
--rwxr-xr-x   0        0        0      866 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
--rw-r--r--   0        0        0     3737 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/mlflow_helpers.py
--rw-r--r--   0        0        0     1370 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0        0        0      263 2023-06-20 14:50:08.668277 kedro_snowflake-0.2.0/kedro_snowflake/starters.py
--rw-r--r--   0        0        0     5272 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/kedro_snowflake/utils.py
--rw-r--r--   0        0        0     1803 2023-06-20 14:50:08.736277 kedro_snowflake-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 kedro_snowflake-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-06-20 15:56:04.398609 kedro_snowflake-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4995 2023-06-20 15:56:04.398609 kedro_snowflake-0.2.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/__init__.py
+-rw-r--r--   0        0        0     4523 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/cli.py
+-rw-r--r--   0        0        0     2282 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/cli_functions.py
+-rw-r--r--   0        0        0     5479 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/config.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/datasets/__init__.py
+-rw-r--r--   0        0        0     5483 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/datasets/internal.py
+-rw-r--r--   0        0        0     5660 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/datasets/native.py
+-rw-r--r--   0        0        0    18339 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/generator.py
+-rw-r--r--   0        0        0      119 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/misc.py
+-rw-r--r--   0        0        0     3504 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/pipeline.py
+-rw-r--r--   0        0        0     1526 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/runner.py
+-rw-r--r--   0        0        0     1612 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/README.md
+-rw-r--r--   0        0        0      595 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/cookiecutter.json
+-rw-r--r--   0        0        0   162747 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0   162747 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0     2339 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/prompts.yml
+-rw-r--r--   0        0        0     1785 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0        0        0     3958 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
+-rw-r--r--   0        0        0     1083 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
+-rw-r--r--   0        0        0     2778 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0        0        0      901 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
+-rw-r--r--   0        0        0      232 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+-rw-r--r--   0        0        0     4375 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0        0        0      431 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.410609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+-rw-r--r--   0        0        0  1810602 2023-06-20 15:56:04.418609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
+-rw-r--r--   0        0        0  2937144 2023-06-20 15:56:04.430609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
+-rw-r--r--   0        0        0  4195290 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+-rw-r--r--   0        0        0     6967 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0        0        0      459 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0        0        0      446 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
+-rw-r--r--   0        0        0      552 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0        0        0     1198 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0        0        0     1109 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+-rw-r--r--   0        0        0       60 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0        0        0     1527 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0        0        0      967 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/hooks.py
+-rw-r--r--   0        0        0      423 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rwxr-xr-x   0        0        0      117 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
+-rwxr-xr-x   0        0        0     1192 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
+-rwxr-xr-x   0        0        0      114 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
+-rwxr-xr-x   0        0        0     2368 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
+-rwxr-xr-x   0        0        0      866 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
+-rw-r--r--   0        0        0     3737 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/mlflow_helpers.py
+-rw-r--r--   0        0        0     1370 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0        0        0      263 2023-06-20 15:56:04.406609 kedro_snowflake-0.2.1/kedro_snowflake/starters.py
+-rw-r--r--   0        0        0     5272 2023-06-20 15:56:04.462609 kedro_snowflake-0.2.1/kedro_snowflake/utils.py
+-rw-r--r--   0        0        0     1803 2023-06-20 15:56:04.466609 kedro_snowflake-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6250 1970-01-01 00:00:00.000000 kedro_snowflake-0.2.1/PKG-INFO
```

### Comparing `kedro_snowflake-0.2.0/LICENSE` & `kedro_snowflake-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/README.md` & `kedro_snowflake-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 This plugin allows to run full Kedro pipelines in Snowflake. Right now it supports
 * Kedro starter, to get you up to speed fast
 * automatically creating Snowflake Stored Procedures from Kedro nodes (using Snowpark SDK)
 * translating Kedro pipeline into Snowflake tasks graph
 * running Kedro pipeline fully within Snowflake, without external system
 * using Kedro's official `SnowparkTableDataSet`
 * automatically storing intermediate data as Transient Tables (if Snowpark's DataFrames are used)
+* <span style="color:yellow;float:left;margin: 0px 7px 0px 0px">**(New!)</span>** [MLflow](https://mlflow.org/) integration with Snowflake with example usage in _Snowflights_ Kedro starter
+
 
 ## Documentation
 For detailed documentation refer to https://kedro-snowflake.readthedocs.io/
 
 ## Usage
 ### With starter
 1. Install the plugin
```

#### html2text {}

```diff
@@ -18,25 +18,27 @@
             **** We help companies turn their data into assets ****
 ## About This plugin allows to run full Kedro pipelines in Snowflake. Right now
 it supports * Kedro starter, to get you up to speed fast * automatically
 creating Snowflake Stored Procedures from Kedro nodes (using Snowpark SDK) *
 translating Kedro pipeline into Snowflake tasks graph * running Kedro pipeline
 fully within Snowflake, without external system * using Kedro's official
 `SnowparkTableDataSet` * automatically storing intermediate data as Transient
-Tables (if Snowpark's DataFrames are used) ## Documentation For detailed
-documentation refer to https://kedro-snowflake.readthedocs.io/ ## Usage ###
-With starter 1. Install the plugin ```bash pip install "kedro-snowflake>=0.1.0"
-``` 2. Create new project with our Kedro starter âï¸ _Snowflights_ ð:
-```bash kedro new --starter=snowflights --checkout=master ```  And answer the
-interactive prompts â¬ï¸ (click to expand)  ``` Project Name ============
-Please enter a human readable name for your new project. Spaces, hyphens, and
-underscores are allowed. [Snowflights]: Snowflake Account =================
-Please enter the name of your Snowflake account. This is the part of the URL
-before .snowflakecomputing.com []: abc-123 Snowflake User ============== Please
-enter the name of your Snowflake user. []: user2137 Snowflake Warehouse
+Tables (if Snowpark's DataFrames are used) * **(New!)** [MLflow](https://
+mlflow.org/) integration with Snowflake with example usage in _Snowflights_
+Kedro starter ## Documentation For detailed documentation refer to https://
+kedro-snowflake.readthedocs.io/ ## Usage ### With starter 1. Install the plugin
+```bash pip install "kedro-snowflake>=0.1.0" ``` 2. Create new project with our
+Kedro starter âï¸ _Snowflights_ ð: ```bash kedro new --
+starter=snowflights --checkout=master ```  And answer the interactive prompts
+â¬ï¸ (click to expand)  ``` Project Name ============ Please enter a human
+readable name for your new project. Spaces, hyphens, and underscores are
+allowed. [Snowflights]: Snowflake Account ================= Please enter the
+name of your Snowflake account. This is the part of the URL before
+.snowflakecomputing.com []: abc-123 Snowflake User ============== Please enter
+the name of your Snowflake user. []: user2137 Snowflake Warehouse
 =================== Please enter the name of your Snowflake warehouse. []:
 compute-wh Snowflake Database ================== Please enter the name of your
 Snowflake database. [DEMO]: Snowflake Schema ================ Please enter the
 name of your Snowflake schema. [DEMO]: Snowflake Password Environment Variable
 ======================================= Please enter the name of the
 environment variable that contains your Snowflake password. Alternatively, you
 can re-configure the plugin later to use Kedros credentials.yml
```

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/cli.py` & `kedro_snowflake-0.2.1/kedro_snowflake/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/cli_functions.py` & `kedro_snowflake-0.2.1/kedro_snowflake/cli_functions.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/config.py` & `kedro_snowflake-0.2.1/kedro_snowflake/config.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/datasets/internal.py` & `kedro_snowflake-0.2.1/kedro_snowflake/datasets/internal.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/datasets/native.py` & `kedro_snowflake-0.2.1/kedro_snowflake/datasets/native.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/generator.py` & `kedro_snowflake-0.2.1/kedro_snowflake/generator.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/pipeline.py` & `kedro_snowflake-0.2.1/kedro_snowflake/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/runner.py` & `kedro_snowflake-0.2.1/kedro_snowflake/runner.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/README.md` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/cookiecutter.json` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/prompts.yml` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/prompts.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/hooks.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/hooks.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/mlflow_helpers.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/mlflow_helpers.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro_snowflake-0.2.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/kedro_snowflake/utils.py` & `kedro_snowflake-0.2.1/kedro_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.2.0/pyproject.toml` & `kedro_snowflake-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-snowflake"
-version = "0.2.0"
+version = "0.2.1"
 description = "Kedro plugin with Snowflake / Snowpark support"
 readme = "README.md"
 authors = ['GetInData MLOPS <mlops@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-snowflake"
 repository = "https://github.com/getindata/kedro-snowflake"
 documentation = "https://kedro-snowflake.readthedocs.io/"
```

### Comparing `kedro_snowflake-0.2.0/PKG-INFO` & `kedro_snowflake-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-snowflake
-Version: 0.2.0
+Version: 0.2.1
 Summary: Kedro plugin with Snowflake / Snowpark support
 Home-page: https://github.com/getindata/kedro-snowflake
 License: Apache-2.0
 Keywords: kedro,snowflake,snowpark,mlops
 Author: GetInData MLOPS
 Author-email: mlops@getindata.com
 Maintainer: GetInData MLOPS
@@ -48,14 +48,16 @@
 This plugin allows to run full Kedro pipelines in Snowflake. Right now it supports
 * Kedro starter, to get you up to speed fast
 * automatically creating Snowflake Stored Procedures from Kedro nodes (using Snowpark SDK)
 * translating Kedro pipeline into Snowflake tasks graph
 * running Kedro pipeline fully within Snowflake, without external system
 * using Kedro's official `SnowparkTableDataSet`
 * automatically storing intermediate data as Transient Tables (if Snowpark's DataFrames are used)
+* <span style="color:yellow;float:left;margin: 0px 7px 0px 0px">**(New!)</span>** [MLflow](https://mlflow.org/) integration with Snowflake with example usage in _Snowflights_ Kedro starter
+
 
 ## Documentation
 For detailed documentation refer to https://kedro-snowflake.readthedocs.io/
 
 ## Usage
 ### With starter
 1. Install the plugin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kedro-snowflake Version: 0.2.0 Summary: Kedro
+Metadata-Version: 2.1 Name: kedro-snowflake Version: 0.2.1 Summary: Kedro
 plugin with Snowflake / Snowpark support Home-page: https://github.com/
 getindata/kedro-snowflake License: Apache-2.0 Keywords:
 kedro,snowflake,snowpark,mlops Author: GetInData MLOPS Author-email:
 mlops@getindata.com Maintainer: GetInData MLOPS Maintainer-email:
 mlops@getindata.com Requires-Python: >=3.8,<3.9 Classifier: Development Status
 :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
@@ -35,25 +35,27 @@
             **** We help companies turn their data into assets ****
 ## About This plugin allows to run full Kedro pipelines in Snowflake. Right now
 it supports * Kedro starter, to get you up to speed fast * automatically
 creating Snowflake Stored Procedures from Kedro nodes (using Snowpark SDK) *
 translating Kedro pipeline into Snowflake tasks graph * running Kedro pipeline
 fully within Snowflake, without external system * using Kedro's official
 `SnowparkTableDataSet` * automatically storing intermediate data as Transient
-Tables (if Snowpark's DataFrames are used) ## Documentation For detailed
-documentation refer to https://kedro-snowflake.readthedocs.io/ ## Usage ###
-With starter 1. Install the plugin ```bash pip install "kedro-snowflake>=0.1.0"
-``` 2. Create new project with our Kedro starter âï¸ _Snowflights_ ð:
-```bash kedro new --starter=snowflights --checkout=master ```  And answer the
-interactive prompts â¬ï¸ (click to expand)  ``` Project Name ============
-Please enter a human readable name for your new project. Spaces, hyphens, and
-underscores are allowed. [Snowflights]: Snowflake Account =================
-Please enter the name of your Snowflake account. This is the part of the URL
-before .snowflakecomputing.com []: abc-123 Snowflake User ============== Please
-enter the name of your Snowflake user. []: user2137 Snowflake Warehouse
+Tables (if Snowpark's DataFrames are used) * **(New!)** [MLflow](https://
+mlflow.org/) integration with Snowflake with example usage in _Snowflights_
+Kedro starter ## Documentation For detailed documentation refer to https://
+kedro-snowflake.readthedocs.io/ ## Usage ### With starter 1. Install the plugin
+```bash pip install "kedro-snowflake>=0.1.0" ``` 2. Create new project with our
+Kedro starter âï¸ _Snowflights_ ð: ```bash kedro new --
+starter=snowflights --checkout=master ```  And answer the interactive prompts
+â¬ï¸ (click to expand)  ``` Project Name ============ Please enter a human
+readable name for your new project. Spaces, hyphens, and underscores are
+allowed. [Snowflights]: Snowflake Account ================= Please enter the
+name of your Snowflake account. This is the part of the URL before
+.snowflakecomputing.com []: abc-123 Snowflake User ============== Please enter
+the name of your Snowflake user. []: user2137 Snowflake Warehouse
 =================== Please enter the name of your Snowflake warehouse. []:
 compute-wh Snowflake Database ================== Please enter the name of your
 Snowflake database. [DEMO]: Snowflake Schema ================ Please enter the
 name of your Snowflake schema. [DEMO]: Snowflake Password Environment Variable
 ======================================= Please enter the name of the
 environment variable that contains your Snowflake password. Alternatively, you
 can re-configure the plugin later to use Kedros credentials.yml
```

