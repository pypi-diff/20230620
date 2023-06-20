# Comparing `tmp/timeseriesflattener-1.0.0.tar.gz` & `tmp/timeseriesflattener-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeseriesflattener-1.0.0.tar", last modified: Thu Jun 15 09:31:15 2023, max compression
+gzip compressed data, was "timeseriesflattener-1.2.0.tar", last modified: Tue Jun 20 08:04:35 2023, max compression
```

## Comparing `timeseriesflattener-1.0.0.tar` & `timeseriesflattener-1.2.0.tar`

### file list

```diff
@@ -1,133 +1,133 @@
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.464397 timeseriesflattener-1.0.0/
--rw-r--r--   0 au484925 (903520038) staff       (20)      489 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.cookiecutter.json
--rw-r--r--   0 au484925 (903520038) staff       (20)      738 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.cruft.json
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.410705 timeseriesflattener-1.0.0/.github/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.403811 timeseriesflattener-1.0.0/.github/actions/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.410959 timeseriesflattener-1.0.0/.github/actions/test/
--rw-r--r--   0 au484925 (903520038) staff       (20)      892 2023-06-14 14:06:50.000000 timeseriesflattener-1.0.0/.github/actions/test/action.yml
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.411219 timeseriesflattener-1.0.0/.github/actions/test_tutorials/
--rw-r--r--   0 au484925 (903520038) staff       (20)      948 2023-06-15 08:56:38.000000 timeseriesflattener-1.0.0/.github/actions/test_tutorials/action.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      529 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/dependabot.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      252 2023-03-01 09:46:41.000000 timeseriesflattener-1.0.0/.github/pull_request_template.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     1689 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/recommended_repo_setup.md
--rw-r--r--   0 au484925 (903520038) staff       (20)      465 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/.github/setup_ci.md
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.413184 timeseriesflattener-1.0.0/.github/workflows/
--rw-r--r--   0 au484925 (903520038) staff       (20)      720 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/check_for_rej.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2083 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/cruft.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      849 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/.github/workflows/dependabot_automerge.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      868 2023-06-07 11:02:56.000000 timeseriesflattener-1.0.0/.github/workflows/documentation.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)      727 2023-03-23 07:54:31.000000 timeseriesflattener-1.0.0/.github/workflows/generate_paper_pdf.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2446 2023-03-23 07:59:10.000000 timeseriesflattener-1.0.0/.github/workflows/main_test_and_release.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2891 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/pre-commit.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     1132 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.github/workflows/stalebot.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     3056 2023-06-14 14:23:53.000000 timeseriesflattener-1.0.0/.github/workflows/static_type_checks.yml
--rw-r--r--   0 au484925 (903520038) staff       (20)     2871 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.gitignore
--rw-r--r--   0 au484925 (903520038) staff       (20)      644 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 au484925 (903520038) staff       (20)     1286 2023-03-31 09:12:14.000000 timeseriesflattener-1.0.0/.zenodo.json
--rw-r--r--   0 au484925 (903520038) staff       (20)    55767 2023-06-15 09:31:08.000000 timeseriesflattener-1.0.0/CHANGELOG.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     5238 2023-03-01 10:46:04.000000 timeseriesflattener-1.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     4474 2023-03-01 11:40:47.000000 timeseriesflattener-1.0.0/CONTRIBUTING.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     1087 2022-12-06 14:15:36.000000 timeseriesflattener-1.0.0/LICENSE
--rw-r--r--   0 au484925 (903520038) staff       (20)      262 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/Makefile
--rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-15 09:31:15.463864 timeseriesflattener-1.0.0/PKG-INFO
--rw-r--r--   0 au484925 (903520038) staff       (20)     9122 2023-06-15 08:47:22.000000 timeseriesflattener-1.0.0/README.md
--rw-r--r--   0 au484925 (903520038) staff       (20)      658 2022-12-06 09:57:22.000000 timeseriesflattener-1.0.0/citation.cff
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.415040 timeseriesflattener-1.0.0/docs/
--rw-r--r--   0 au484925 (903520038) staff       (20)      633 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/docs/Makefile
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.416482 timeseriesflattener-1.0.0/docs/_static/
--rw-r--r--   0 au484925 (903520038) staff       (20)    15406 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/favicon.ico
--rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/icon.png
--rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/icon_dark.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   811066 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/_static/terminology_figure.png
--rw-r--r--   0 au484925 (903520038) staff       (20)     4211 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/docs/conf.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2097 2023-04-19 11:55:26.000000 timeseriesflattener-1.0.0/docs/faq.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)      332 2023-06-14 14:10:35.000000 timeseriesflattener-1.0.0/docs/feature_specifications.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)     5280 2023-01-25 13:20:02.000000 timeseriesflattener-1.0.0/docs/index.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)      299 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/installation.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)      312 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/timeseriesflattener.rst
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.421322 timeseriesflattener-1.0.0/docs/tutorials/
--rw-r--r--   0 au484925 (903520038) staff       (20)   118804 2023-06-15 08:47:23.000000 timeseriesflattener-1.0.0/docs/tutorials/01_basic.ipynb
--rw-r--r--   0 au484925 (903520038) staff       (20)    50220 2023-06-15 08:47:22.000000 timeseriesflattener-1.0.0/docs/tutorials/02_advanced.ipynb
--rw-r--r--   0 au484925 (903520038) staff       (20)    72388 2023-06-15 08:34:08.000000 timeseriesflattener-1.0.0/docs/tutorials/03_text.ipynb
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.424123 timeseriesflattener-1.0.0/docs/tutorials/img/
--rw-r--r--   0 au484925 (903520038) staff       (20)    78953 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_a.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   109486 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_b.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   107613 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_c.png
--rw-r--r--   0 au484925 (903520038) staff       (20)   250306 2022-12-12 11:53:58.000000 timeseriesflattener-1.0.0/docs/tutorials/img/term_d.png
--rw-r--r--   0 au484925 (903520038) staff       (20)      370 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/docs/tutorials.rst
--rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.0.0/icon.png
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.425267 timeseriesflattener-1.0.0/paper/
--rw-r--r--   0 au484925 (903520038) staff       (20)    14392 2023-03-31 09:12:14.000000 timeseriesflattener-1.0.0/paper/paper.bib
--rw-r--r--   0 au484925 (903520038) staff       (20)     9344 2023-03-31 09:12:14.000000 timeseriesflattener-1.0.0/paper/paper.md
--rw-r--r--   0 au484925 (903520038) staff       (20)     4327 2023-06-15 09:31:08.000000 timeseriesflattener-1.0.0/pyproject.toml
--rw-r--r--   0 au484925 (903520038) staff       (20)       38 2023-06-15 09:31:15.464448 timeseriesflattener-1.0.0/setup.cfg
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.425526 timeseriesflattener-1.0.0/src/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1996 2023-06-14 14:28:54.000000 timeseriesflattener-1.0.0/src/conftest.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.427953 timeseriesflattener-1.0.0/src/timeseriesflattener/
--rw-r--r--   0 au484925 (903520038) staff       (20)      309 2023-06-14 08:57:30.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     4834 2023-06-15 08:30:34.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/aggregation_fns.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     5559 2023-06-14 12:58:48.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/column_handler.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.429076 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-12-06 12:02:05.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     1977 2023-06-14 09:34:12.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     6308 2023-06-15 08:28:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.429592 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/
--rw-r--r--   0 au484925 (903520038) staff       (20)     7344 2023-06-15 08:34:18.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/group_specs.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     8428 2023-06-15 08:34:18.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/single_specs.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    36395 2023-06-15 08:30:40.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_dataset.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2271 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_ds_validator.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2239 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/logger.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     7704 2023-06-14 11:44:29.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/misc_utils.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.430337 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/
--rw-r--r--   0 au484925 (903520038) staff       (20)     3008 2023-06-14 12:20:04.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/load_synth_data.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.405297 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.405021 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.430851 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1477 2023-03-20 10:36:42.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
--rw-r--r--   0 au484925 (903520038) staff       (20)   864795 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.433308 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1869 2023-04-20 07:25:41.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    25543 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
--rw-r--r--   0 au484925 (903520038) staff       (20)     1015 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.453628 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/
--rw-r--r--   0 au484925 (903520038) staff       (20)      784 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     1003 2023-03-20 10:36:42.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
--rw-r--r--   0 au484925 (903520038) staff       (20)      980 2023-06-14 09:07:20.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
--rw-r--r--   0 au484925 (903520038) staff       (20)      816 2023-03-20 10:36:42.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
--rw-r--r--   0 au484925 (903520038) staff       (20)   248865 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)   268962 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)   268904 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)  4316151 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)  4315816 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)    68900 2022-12-12 11:53:56.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)    84570 2023-02-23 15:25:24.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
--rw-r--r--   0 au484925 (903520038) staff       (20)     1392 2023-06-14 12:15:52.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/text_embedding_functions.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     5179 2023-06-14 13:28:04.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/testing/utils_for_testing.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.454465 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/__init__.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.454563 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_feature_cache/
--rw-r--r--   0 au484925 (903520038) staff       (20)     3425 2023-06-15 08:34:08.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.455393 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    16237 2023-06-15 08:34:01.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     1452 2023-06-14 10:33:38.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2305 2023-06-15 08:34:09.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.462878 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
--rw-r--r--   0 au484925 (903520038) staff       (20)        0 2023-02-07 08:39:43.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
--rw-r--r--   0 au484925 (903520038) staff       (20)    18309 2023-06-15 08:34:09.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2688 2023-06-15 08:34:11.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2328 2023-06-14 10:33:38.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2319 2023-06-15 08:34:18.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     8190 2023-06-15 08:34:19.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2397 2023-06-14 11:20:11.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
--rw-r--r--   0 au484925 (903520038) staff       (20)     2342 2023-06-14 12:24:11.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/text_embedding_functions.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.463210 timeseriesflattener-1.0.0/src/timeseriesflattener/utils/
--rw-r--r--   0 au484925 (903520038) staff       (20)     1065 2023-06-14 13:05:30.000000 timeseriesflattener-1.0.0/src/timeseriesflattener/utils/pydantic_basemodel.py
-drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-15 09:31:15.428600 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/
--rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/PKG-INFO
--rw-r--r--   0 au484925 (903520038) staff       (20)     4668 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/SOURCES.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)        1 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/dependency_links.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)      739 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/requires.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)       29 2023-06-15 09:31:15.000000 timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/top_level.txt
--rw-r--r--   0 au484925 (903520038) staff       (20)     9396 2023-06-15 08:57:16.000000 timeseriesflattener-1.0.0/tasks.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.165711 timeseriesflattener-1.2.0/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      489 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.cookiecutter.json
+-rw-r--r--   0 au484925 (903520038) staff       (20)      738 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.cruft.json
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.119565 timeseriesflattener-1.2.0/.github/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.112944 timeseriesflattener-1.2.0/.github/actions/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.119814 timeseriesflattener-1.2.0/.github/actions/test/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      892 2023-06-14 14:06:50.000000 timeseriesflattener-1.2.0/.github/actions/test/action.yml
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.120056 timeseriesflattener-1.2.0/.github/actions/test_tutorials/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      948 2023-06-15 08:56:38.000000 timeseriesflattener-1.2.0/.github/actions/test_tutorials/action.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      529 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.github/dependabot.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      252 2023-03-01 09:46:41.000000 timeseriesflattener-1.2.0/.github/pull_request_template.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1689 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.github/recommended_repo_setup.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)      465 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/.github/setup_ci.md
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.121788 timeseriesflattener-1.2.0/.github/workflows/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      720 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.github/workflows/check_for_rej.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2083 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.github/workflows/cruft.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      849 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/.github/workflows/dependabot_automerge.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      868 2023-06-07 11:02:56.000000 timeseriesflattener-1.2.0/.github/workflows/documentation.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)      727 2023-03-23 07:54:31.000000 timeseriesflattener-1.2.0/.github/workflows/generate_paper_pdf.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2446 2023-06-20 08:04:16.000000 timeseriesflattener-1.2.0/.github/workflows/main_test_and_release.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2891 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1132 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.github/workflows/stalebot.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     3056 2023-06-14 14:23:53.000000 timeseriesflattener-1.2.0/.github/workflows/static_type_checks.yml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2871 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.gitignore
+-rw-r--r--   0 au484925 (903520038) staff       (20)      644 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1286 2023-03-31 09:12:14.000000 timeseriesflattener-1.2.0/.zenodo.json
+-rw-r--r--   0 au484925 (903520038) staff       (20)    55819 2023-06-20 08:04:27.000000 timeseriesflattener-1.2.0/CHANGELOG.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5238 2023-03-01 10:46:04.000000 timeseriesflattener-1.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4474 2023-03-01 11:40:47.000000 timeseriesflattener-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1087 2022-12-06 14:15:36.000000 timeseriesflattener-1.2.0/LICENSE
+-rw-r--r--   0 au484925 (903520038) staff       (20)      262 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/Makefile
+-rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-20 08:04:35.165186 timeseriesflattener-1.2.0/PKG-INFO
+-rw-r--r--   0 au484925 (903520038) staff       (20)     9122 2023-06-15 08:47:22.000000 timeseriesflattener-1.2.0/README.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)      658 2022-12-06 09:57:22.000000 timeseriesflattener-1.2.0/citation.cff
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.123715 timeseriesflattener-1.2.0/docs/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      633 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/docs/Makefile
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.125475 timeseriesflattener-1.2.0/docs/_static/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    15406 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.0/docs/_static/favicon.ico
+-rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.0/docs/_static/icon.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.0/docs/_static/icon_dark.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   811066 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.0/docs/_static/terminology_figure.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4211 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.0/docs/conf.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2097 2023-04-19 11:55:26.000000 timeseriesflattener-1.2.0/docs/faq.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)      332 2023-06-14 14:10:35.000000 timeseriesflattener-1.2.0/docs/feature_specifications.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5280 2023-01-25 13:20:02.000000 timeseriesflattener-1.2.0/docs/index.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)      299 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.0/docs/installation.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)      312 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.0/docs/timeseriesflattener.rst
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.130555 timeseriesflattener-1.2.0/docs/tutorials/
+-rw-r--r--   0 au484925 (903520038) staff       (20)   118804 2023-06-15 08:47:23.000000 timeseriesflattener-1.2.0/docs/tutorials/01_basic.ipynb
+-rw-r--r--   0 au484925 (903520038) staff       (20)    50220 2023-06-15 08:47:22.000000 timeseriesflattener-1.2.0/docs/tutorials/02_advanced.ipynb
+-rw-r--r--   0 au484925 (903520038) staff       (20)    72388 2023-06-15 08:34:08.000000 timeseriesflattener-1.2.0/docs/tutorials/03_text.ipynb
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.133154 timeseriesflattener-1.2.0/docs/tutorials/img/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    78953 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.0/docs/tutorials/img/term_a.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   109486 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.0/docs/tutorials/img/term_b.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   107613 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.0/docs/tutorials/img/term_c.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)   250306 2022-12-12 11:53:58.000000 timeseriesflattener-1.2.0/docs/tutorials/img/term_d.png
+-rw-r--r--   0 au484925 (903520038) staff       (20)      370 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.0/docs/tutorials.rst
+-rw-r--r--   0 au484925 (903520038) staff       (20)    49714 2022-12-15 07:52:34.000000 timeseriesflattener-1.2.0/icon.png
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.134309 timeseriesflattener-1.2.0/paper/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    14392 2023-03-31 09:12:14.000000 timeseriesflattener-1.2.0/paper/paper.bib
+-rw-r--r--   0 au484925 (903520038) staff       (20)     9344 2023-03-31 09:12:14.000000 timeseriesflattener-1.2.0/paper/paper.md
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4318 2023-06-20 08:04:27.000000 timeseriesflattener-1.2.0/pyproject.toml
+-rw-r--r--   0 au484925 (903520038) staff       (20)       38 2023-06-20 08:04:35.165763 timeseriesflattener-1.2.0/setup.cfg
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.134619 timeseriesflattener-1.2.0/src/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1996 2023-06-14 14:28:54.000000 timeseriesflattener-1.2.0/src/conftest.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.137115 timeseriesflattener-1.2.0/src/timeseriesflattener/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      309 2023-06-14 08:57:30.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4834 2023-06-15 08:30:34.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/aggregation_fns.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5559 2023-06-14 12:58:48.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/column_handler.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.138371 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_cache/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-12-06 12:02:05.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_cache/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1977 2023-06-14 09:34:12.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     6308 2023-06-15 08:28:24.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_cache/cache_to_disk.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.138864 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_specs/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     7344 2023-06-15 08:34:18.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_specs/group_specs.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     8428 2023-06-15 08:34:18.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/feature_specs/single_specs.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    36395 2023-06-15 08:30:40.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/flattened_dataset.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2271 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/flattened_ds_validator.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2239 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/logger.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     7704 2023-06-14 11:44:29.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/misc_utils.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.139546 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     3008 2023-06-14 12:20:04.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/load_synth_data.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.114450 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.114254 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/flattened/
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.140031 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1477 2023-03-20 10:36:42.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)   864795 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.142577 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1869 2023-04-20 07:25:41.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    25543 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1015 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.160005 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/
+-rw-r--r--   0 au484925 (903520038) staff       (20)      784 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1003 2023-03-20 10:36:42.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)      980 2023-06-14 09:07:20.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)      816 2023-03-20 10:36:42.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_txt_data.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)   248865 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)   268962 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)   268904 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)  4316151 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)  4315816 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)    68900 2022-12-12 11:53:56.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)    84570 2023-02-23 15:25:24.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1392 2023-06-14 12:15:52.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/text_embedding_functions.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     5179 2023-06-14 13:28:04.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/testing/utils_for_testing.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.160895 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/__init__.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.161008 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_feature_cache/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     3425 2023-06-15 08:34:08.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.161803 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2022-11-30 10:22:16.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    16237 2023-06-15 08:34:01.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1452 2023-06-14 10:33:38.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2305 2023-06-15 08:34:09.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.164185 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/
+-rw-r--r--   0 au484925 (903520038) staff       (20)        0 2023-02-07 08:39:43.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/__init__.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)    18309 2023-06-15 08:34:09.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2688 2023-06-15 08:34:11.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2328 2023-06-14 10:33:38.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2319 2023-06-15 08:34:18.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     8190 2023-06-15 08:34:19.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2397 2023-06-14 11:20:11.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py
+-rw-r--r--   0 au484925 (903520038) staff       (20)     2342 2023-06-14 12:24:11.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/text_embedding_functions.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.164457 timeseriesflattener-1.2.0/src/timeseriesflattener/utils/
+-rw-r--r--   0 au484925 (903520038) staff       (20)     1065 2023-06-14 13:05:30.000000 timeseriesflattener-1.2.0/src/timeseriesflattener/utils/pydantic_basemodel.py
+drwxr-xr-x   0 au484925 (903520038) staff       (20)        0 2023-06-20 08:04:35.137855 timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/
+-rw-r--r--   0 au484925 (903520038) staff       (20)    11520 2023-06-20 08:04:35.000000 timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/PKG-INFO
+-rw-r--r--   0 au484925 (903520038) staff       (20)     4668 2023-06-20 08:04:35.000000 timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/SOURCES.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)        1 2023-06-20 08:04:35.000000 timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/dependency_links.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)      730 2023-06-20 08:04:35.000000 timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/requires.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)       29 2023-06-20 08:04:35.000000 timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/top_level.txt
+-rw-r--r--   0 au484925 (903520038) staff       (20)     9396 2023-06-15 08:57:16.000000 timeseriesflattener-1.2.0/tasks.py
```

### Comparing `timeseriesflattener-1.0.0/.cruft.json` & `timeseriesflattener-1.2.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/actions/test/action.yml` & `timeseriesflattener-1.2.0/.github/actions/test/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/actions/test_tutorials/action.yml` & `timeseriesflattener-1.2.0/.github/actions/test_tutorials/action.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/dependabot.yml` & `timeseriesflattener-1.2.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/recommended_repo_setup.md` & `timeseriesflattener-1.2.0/.github/recommended_repo_setup.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/check_for_rej.yml` & `timeseriesflattener-1.2.0/.github/workflows/check_for_rej.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/cruft.yml` & `timeseriesflattener-1.2.0/.github/workflows/cruft.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/dependabot_automerge.yml` & `timeseriesflattener-1.2.0/.github/workflows/dependabot_automerge.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/documentation.yml` & `timeseriesflattener-1.2.0/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/generate_paper_pdf.yml` & `timeseriesflattener-1.2.0/.github/workflows/generate_paper_pdf.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/main_test_and_release.yml` & `timeseriesflattener-1.2.0/.github/workflows/main_test_and_release.yml`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
       # Checkout action is required for token to persist
       - uses: actions/checkout@v2
         with:
           fetch-depth: 0
           token: ${{ secrets.RELEASE_BOT }}
 
       - name: Python Semantic Release
-        uses: relekang/python-semantic-release@v7.33.1
+        uses: relekang/python-semantic-release@v7.34.4
         with:
           github_token: ${{ secrets.RELEASE_BOT }}
           # Remember to copy the tool.semantic_release section from pyproject.toml
           # as well
           # To enable pypi,
           # 1) Set upload_to_pypi to true in pyproject.toml and
           # 2) Set the pypi_token in the repo
```

### Comparing `timeseriesflattener-1.0.0/.github/workflows/pre-commit.yml` & `timeseriesflattener-1.2.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/stalebot.yml` & `timeseriesflattener-1.2.0/.github/workflows/stalebot.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.github/workflows/static_type_checks.yml` & `timeseriesflattener-1.2.0/.github/workflows/static_type_checks.yml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.gitignore` & `timeseriesflattener-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.pre-commit-config.yaml` & `timeseriesflattener-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/.zenodo.json` & `timeseriesflattener-1.2.0/.zenodo.json`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/CHANGELOG.md` & `timeseriesflattener-1.2.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v1.2.0 (2023-06-20)
+
+
+
+## v1.1.0 (2023-06-20)
+
+
+
 ## v1.0.0 (2023-06-15)
 
 ### Feature
 
 * Specs should be pydantic basemodels ([`04781f6`](https://github.com/Aarhus-Psychiatry-Research/timeseriesflattener/commit/04781f6ace79d8abbddaa92ac57a4877be5f9398))
 
 ### Fix
```

### Comparing `timeseriesflattener-1.0.0/CODE_OF_CONDUCT.md` & `timeseriesflattener-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/CONTRIBUTING.md` & `timeseriesflattener-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/LICENSE` & `timeseriesflattener-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/PKG-INFO` & `timeseriesflattener-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.0.0
+Version: 1.2.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.2.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.0.0/README.md` & `timeseriesflattener-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/citation.cff` & `timeseriesflattener-1.2.0/citation.cff`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/Makefile` & `timeseriesflattener-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/_static/favicon.ico` & `timeseriesflattener-1.2.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/_static/icon.png` & `timeseriesflattener-1.2.0/docs/_static/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/_static/icon_dark.png` & `timeseriesflattener-1.2.0/docs/_static/icon_dark.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/_static/terminology_figure.png` & `timeseriesflattener-1.2.0/docs/_static/terminology_figure.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/conf.py` & `timeseriesflattener-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/faq.rst` & `timeseriesflattener-1.2.0/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/index.rst` & `timeseriesflattener-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/01_basic.ipynb` & `timeseriesflattener-1.2.0/docs/tutorials/01_basic.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/02_advanced.ipynb` & `timeseriesflattener-1.2.0/docs/tutorials/02_advanced.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/03_text.ipynb` & `timeseriesflattener-1.2.0/docs/tutorials/03_text.ipynb`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/img/term_a.png` & `timeseriesflattener-1.2.0/docs/tutorials/img/term_a.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/img/term_b.png` & `timeseriesflattener-1.2.0/docs/tutorials/img/term_b.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/img/term_c.png` & `timeseriesflattener-1.2.0/docs/tutorials/img/term_c.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/docs/tutorials/img/term_d.png` & `timeseriesflattener-1.2.0/docs/tutorials/img/term_d.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/icon.png` & `timeseriesflattener-1.2.0/icon.png`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/paper/paper.bib` & `timeseriesflattener-1.2.0/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/paper/paper.md` & `timeseriesflattener-1.2.0/paper/paper.md`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/pyproject.toml` & `timeseriesflattener-1.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel", "setuptools_scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "timeseriesflattener"
-version = "1.0.0"
+version = "1.2.0"
 authors = [{name = "Lasse Hansen", email = "lasseh0310@gmail.com"}, {name = "Jakob Grøhn Damgaard", email = "bokajgd@gmail.com"}, {name = "Kenneth Enevoldsen"}, {name = "Martin Bernstorff", email = "martinbernstorff@gmail.com"}]
 description = "A package for converting time series data from e.g. electronic health records into wide format data."
 classifiers = [
   "Operating System :: POSIX :: Linux",
   "Operating System :: MacOS :: MacOS X",
   "Operating System :: Microsoft :: Windows",
   "Programming Language :: Python :: 3.8",
@@ -20,29 +20,29 @@
 dependencies = [
     "scipy>=1.8.0",
     "scikit-learn>=1.1.2",
     "pydantic>=1.9.0",
     "pandas>=1.4.0",
     "catalogue>=2.0.0",
     "numpy>=1.23.3",
-    "pyarrow>=9.0.0",
-    "protobuf<=4.22.3", # Other versions give errors with pytest, super weird!
+    "pyarrow>=8.0.0",
+    "protobuf<=4.23.3", # Other versions give errors with pytest, super weird!
     "frozendict>=2.3.4",
     "coloredlogs>14.0.0",
     "psycopmlutils>=0.5.0",
 ]
 
 [project.license]
 file = "LICENSE"
 name = "MIT"
 [project.optional-dependencies]
 dev = [
   "cruft",
   "pyright==1.1.305",  
-  "pre-commit==2.20.0,<2.21.0",
+  "pre-commit==3.3.3",
   "ruff==0.0.272", # important that these match the pre-commit hooks
   "black[jupyter]==22.8.0", # important that these match the pre-commit hooks
   "pandas-stubs", # type stubs for pandas
   "invoke==2.1.1",
   "tox",
 ]
 test = [
```

### Comparing `timeseriesflattener-1.0.0/src/conftest.py` & `timeseriesflattener-1.2.0/src/conftest.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/aggregation_fns.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/column_handler.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/column_handler.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/feature_cache/abstract_feature_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/feature_cache/cache_to_disk.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/feature_cache/cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/group_specs.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/feature_specs/group_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/feature_specs/single_specs.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/feature_specs/single_specs.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_dataset.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/flattened_ds_validator.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/flattened_ds_validator.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/logger.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/logger.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/misc_utils.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/misc_utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/load_synth_data.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/load_synth_data.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/create_synth_flattened_with_outcome.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/flattened/generated_with_outcome/synth_flattened_with_outcome.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/create_bow_and_pca_model.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/synth_bow_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/models/synth_pca_model.pkl`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_prediction_times.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_binary.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_raw_float.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/create_synth_sex.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_prediction_times.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_binary_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_1.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_raw_float_2.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_sex.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/test_data/raw/synth_text_data.csv`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/text_embedding_functions.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/testing/utils_for_testing.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/testing/utils_for_testing.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_feature_cache/test_cache_to_disk.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_aggregation_fns.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_feature_spec_objects.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_add_values.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_cache.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_concatenation.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_errors.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/test_flattened_dataset.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/tests/test_timeseriesflattener/test_flattened_dataset/utils.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/text_embedding_functions.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/text_embedding_functions.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener/utils/pydantic_basemodel.py` & `timeseriesflattener-1.2.0/src/timeseriesflattener/utils/pydantic_basemodel.py`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/PKG-INFO` & `timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeseriesflattener
-Version: 1.0.0
+Version: 1.2.0
 Summary: A package for converting time series data from e.g. electronic health records into wide format data.
 Author: Kenneth Enevoldsen
 Author-email: Lasse Hansen <lasseh0310@gmail.com>, Jakob Grøhn Damgaard <bokajgd@gmail.com>, Martin Bernstorff <martinbernstorff@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 PSYCOP Group, Aarhus University
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.0.0 Summary: A
+Metadata-Version: 2.1 Name: timeseriesflattener Version: 1.2.0 Summary: A
 package for converting time series data from e.g. electronic health records
 into wide format data. Author: Kenneth Enevoldsen Author-email: Lasse Hansen
 gmail.com>, Jakob GrÃ¸hn Damgaard
 gmail.com>, Martin Bernstorff
 gmail.com> License: MIT License Copyright (c) 2022 PSYCOP Group, Aarhus
 University Permission is hereby granted, free of charge, to any person
 obtaining a copy of this software and associated documentation files (the
```

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/SOURCES.txt` & `timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `timeseriesflattener-1.0.0/src/timeseriesflattener.egg-info/requires.txt` & `timeseriesflattener-1.2.0/src/timeseriesflattener.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 scipy>=1.8.0
 scikit-learn>=1.1.2
 pydantic>=1.9.0
 pandas>=1.4.0
 catalogue>=2.0.0
 numpy>=1.23.3
-pyarrow>=9.0.0
-protobuf<=4.22.3
+pyarrow>=8.0.0
+protobuf<=4.23.3
 frozendict>=2.3.4
 coloredlogs>14.0.0
 psycopmlutils>=0.5.0
 
 [dev]
 cruft
 pyright==1.1.305
-pre-commit<2.21.0,==2.20.0
+pre-commit==3.3.3
 ruff==0.0.272
 black[jupyter]==22.8.0
 pandas-stubs
 invoke==2.1.1
 tox
 
 [docs]
```

### Comparing `timeseriesflattener-1.0.0/tasks.py` & `timeseriesflattener-1.2.0/tasks.py`

 * *Files identical despite different names*

