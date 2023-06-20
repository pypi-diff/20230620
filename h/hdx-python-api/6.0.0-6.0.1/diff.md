# Comparing `tmp/hdx-python-api-6.0.0.tar.gz` & `tmp/hdx-python-api-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hdx-python-api-6.0.0.tar", last modified: Thu Apr 13 04:41:06 2023, max compression
+gzip compressed data, was "hdx-python-api-6.0.1.tar", last modified: Tue Jun 20 01:23:01 2023, max compression
```

## Comparing `hdx-python-api-6.0.0.tar` & `hdx-python-api-6.0.1.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.916793 hdx-python-api-6.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.github/workflows/run-python-tests.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/.readthedocs.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/doc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    42394 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/doc/main.md
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.916793 hdx-python-api-6.0.0/src/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.924793 hdx-python-api-6.0.0/src/hdx/api/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx/api/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24827 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/hdx_base_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/api/locations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.924793 hdx-python-api-6.0.0/src/hdx/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   111856 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9457 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/dataset_title_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/date_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/filestore_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/hdx_datasource_topline.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    28494 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/hdxobject.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/indicator_resource_view_template.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    11097 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/organization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24274 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4532 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/resource_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7678 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/resource_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15004 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/showcase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9685 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21984 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/data/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.928794 hdx-python-api-6.0.0/src/hdx/facades/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3863 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/infer_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/keyword_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/src/hdx/facades/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.928794 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-13 04:41:06.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:41:05.000000 hdx-python-api-6.0.0/src/hdx_python_api.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.920793 hdx-python-api-6.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.928794 hdx-python-api-6.0.0/tests/fixtures/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/Accepted_Tags.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)   169312 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/Tag_Mapping.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/Tag_Mapping_ChainRuleError.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/config/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/empty.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      449 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_base_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_base_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_datasource_topline.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_datasource_topline.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_email_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_email_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_missing_site_config.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_organization_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_organization_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      147 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_view_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_view_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_showcase_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_showcase_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_user_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_user_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_vocabulary_static.json
--rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/hdx_vocabulary_static.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/project_configuration.json
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/project_configuration.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config2.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config3.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/config/user_agent_config_wrong.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    25870 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/dataset_search_results.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/datastore/
--rwxr-xr-x   0 runner    (1001) docker     (123)    23724 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/empty.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/gen_resource/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      920 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/test_data_no_data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/gen_resource/test_data_no_years.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)    13842 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/organization_show_results.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.936794 hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/resource_formats.json
--rwxr-xr-x   0 runner    (1001) docker     (123)    14465 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/showcase_all_search_results.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/test_data.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/test_data.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.940794 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/
--rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   319924 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    92805 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   290790 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   230593 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   216041 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)   842238 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
--rw-r--r--   0 runner    (1001) docker     (123)    48523 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_dataset.json
--rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.940794 hdx-python-api-6.0.0/tests/fixtures/update_logic/
--rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources.yml
--rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources_new.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.944794 hdx-python-api-6.0.0/tests/hdx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.944794 hdx-python-api-6.0.0/tests/hdx/api/
--rwxr-xr-x   0 runner    (1001) docker     (123)    34779 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/api/test_configuration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3009 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/api/test_locations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    44943 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/tests/hdx/data/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9940 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49148 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_dataset_core.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    75019 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_dataset_noncore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_dataset_title_helper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19570 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_organization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45966 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_resource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19114 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_resource_view.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23053 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_showcase.py
--rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_update_dataset_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    63707 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_update_logic.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21174 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   116056 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/data/test_vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/tests/hdx/facades/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/test_infer_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5957 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/test_keyword_arguments.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5651 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/tests/hdx/facades/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:41:06.948794 hdx-python-api-6.0.0/workingexample/
--rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/my_code.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/my_resource.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/my_resource.xlsx
--rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-04-13 04:40:44.000000 hdx-python-api-6.0.0/workingexample/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.624457 hdx-python-api-6.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.604457 hdx-python-api-6.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.608457 hdx-python-api-6.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/.github/workflows/run-python-tests.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1148 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/.readthedocs.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1079 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 01:23:01.624457 hdx-python-api-6.0.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1294 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.608457 hdx-python-api-6.0.1/doc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42389 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/doc/main.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      165 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1460 2023-06-20 01:23:01.624457 hdx-python-api-6.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.604457 hdx-python-api-6.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.604457 hdx-python-api-6.0.1/src/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.608457 hdx-python-api-6.0.1/src/hdx/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-20 01:23:01.000000 hdx-python-api-6.0.1/src/hdx/api/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24827 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/api/configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2023 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/api/hdx_base_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4541 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/api/locations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.608457 hdx-python-api-6.0.1/src/hdx/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   111856 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9457 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/dataset_title_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5798 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/date_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3545 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/filestore_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      366 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/hdx_datasource_topline.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28494 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/hdxobject.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2915 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/indicator_resource_view_template.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11097 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/organization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24274 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4532 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/resource_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7678 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/resource_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15004 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/showcase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9685 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22127 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/data/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.608457 hdx-python-api-6.0.1/src/hdx/facades/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/facades/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3863 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/facades/infer_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1113 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/facades/keyword_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1057 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/src/hdx/facades/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.612457 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-20 01:23:01.000000 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-06-20 01:23:01.000000 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:23:01.000000 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-20 01:23:01.000000 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-20 01:23:01.000000 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 01:23:00.000000 hdx-python-api-6.0.1/src/hdx_python_api.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)       64 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.604457 hdx-python-api-6.0.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.612457 hdx-python-api-6.0.1/tests/fixtures/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6147 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/Accepted_Tags.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)   169312 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/Tag_Mapping.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      234 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/Tag_Mapping_ChainRuleError.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.616457 hdx-python-api-6.0.1/tests/fixtures/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/empty.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      449 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_base_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      373 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_base_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       55 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_dataset_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      975 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_dataset_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_datasource_topline.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      367 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_datasource_topline.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      172 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_email_configuration.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      135 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_email_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       75 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_missing_site_config.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      134 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_organization_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       72 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_organization_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      182 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_resource_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      147 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_resource_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       87 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_resource_view_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_resource_view_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      221 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_showcase_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      188 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_showcase_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      161 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_user_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_user_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_vocabulary_static.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)       39 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/hdx_vocabulary_static.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/project_configuration.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/project_configuration.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       32 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/user_agent_config.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       23 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/user_agent_config2.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       73 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/user_agent_config3.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/config/user_agent_config_wrong.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25870 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/dataset_search_results.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.616457 hdx-python-api-6.0.1/tests/fixtures/datastore/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23724 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/empty.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.616457 hdx-python-api-6.0.1/tests/fixtures/gen_resource/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/gen_resource/conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/gen_resource/min_qc_conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      920 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/gen_resource/qc_conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/gen_resource/test_data_no_data.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1534 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/gen_resource/test_data_no_years.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13842 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/organization_show_results.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.616457 hdx-python-api-6.0.1/tests/fixtures/qc_from_rows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)       42 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/qc_from_rows/qc_conflict_data_alg_one_col.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/resource_formats.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14465 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/showcase_all_search_results.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1549 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/test_data.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      830 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/test_data.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.620457 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    50900 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/dem_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   319924 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/opri_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    92805 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   290790 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   230593 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   216041 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   842238 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    48523 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/unesco_dataset.json
+-rw-r--r--   0 runner    (1001) docker     (123)    38434 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/unesco_update_dataset.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.620457 hdx-python-api-6.0.1/tests/fixtures/update_logic/
+-rw-r--r--   0 runner    (1001) docker     (123)    24658 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_logic/update_logic_resources.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16486 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/fixtures/update_logic/update_logic_resources_new.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.620457 hdx-python-api-6.0.1/tests/hdx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.620457 hdx-python-api-6.0.1/tests/hdx/api/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34779 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/api/test_configuration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3009 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/api/test_locations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44943 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.620457 hdx-python-api-6.0.1/tests/hdx/data/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9940 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49148 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_dataset_core.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    75350 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_dataset_noncore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_dataset_title_helper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19570 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_organization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45966 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_resource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19114 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_resource_view.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23053 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_showcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10124 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_update_dataset_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63707 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_update_logic.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21174 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   116056 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/data/test_vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.620457 hdx-python-api-6.0.1/tests/hdx/facades/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1489 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/facades/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3184 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/facades/test_infer_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5957 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/facades/test_keyword_arguments.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5651 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/tests/hdx/facades/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 01:23:01.624457 hdx-python-api-6.0.1/workingexample/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      174 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/workingexample/my_code.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       12 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/workingexample/my_resource.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/workingexample/my_resource.xlsx
+-rwxr-xr-x   0 runner    (1001) docker     (123)      393 2023-06-20 01:22:41.000000 hdx-python-api-6.0.1/workingexample/run.py
```

### Comparing `hdx-python-api-6.0.0/.github/workflows/publish.yml` & `hdx-python-api-6.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/.github/workflows/run-python-tests.yml` & `hdx-python-api-6.0.1/.github/workflows/run-python-tests.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/.gitignore` & `hdx-python-api-6.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/LICENSE` & `hdx-python-api-6.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/PKG-INFO` & `hdx-python-api-6.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.0
+Version: 6.0.1
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Home-page: https://github.com/OCHA-DAP/hdx-python-api
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,API,library,CKAN
 Platform: any
```

### Comparing `hdx-python-api-6.0.0/README.md` & `hdx-python-api-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/doc/main.md` & `hdx-python-api-6.0.1/doc/main.md`

 * *Files 1% similar despite different names*

```diff
@@ -214,55 +214,55 @@
 
         Configuration.create(hdx_site="stage", user_agent="A_Quick_Example")
 
 10. Read this dataset 
 [Novel Coronavirus (COVID-19) Cases Data](https://data.humdata.org/dataset/novel-coronavirus-2019-ncov-cases)
      from HDX and view the date of the dataset:
 
-         dataset = Dataset.read_from_hdx("novel-coronavirus-2019-ncov-cases")
-         print(dataset.get_reference_period())
+        dataset = Dataset.read_from_hdx("novel-coronavirus-2019-ncov-cases")
+        print(dataset.get_reference_period())
 
 11. You can search for datasets on HDX and get their resources:
 
-         datasets = Dataset.search_in_hdx("thailand subnational boundaries", rows=10)
-         print(datasets)
-         resources = Dataset.get_all_resources(datasets)
-         print(resources)
+        datasets = Dataset.search_in_hdx("thailand subnational boundaries", rows=10)
+        print(datasets)
+        resources = Dataset.get_all_resources(datasets)
+        print(resources)
 
 12. You can download a resource in the dataset:
 
-         url, path = resources[0].download()
-         print("Resource URL %s downloaded to %s" % (url, path))
+        url, path = resources[0].download()
+        print("Resource URL %s downloaded to %s" % (url, path))
 
 13. If you have an API key, you can write to HDX. You can try it out on a test 
     server. With a dataset to which you have permissions, change the dataset date:
 
-         dataset = Dataset.read_from_hdx("ID OR NAME OF DATASET")
-         print(dataset.get_reference_period())  # record this
-         dataset.set_reference_period("2015-07-26")
-         print(dataset.get_reference_period())
-         dataset.update_in_hdx()
+        dataset = Dataset.read_from_hdx("ID OR NAME OF DATASET")
+        print(dataset.get_reference_period())  # record this
+        dataset.set_reference_period("2015-07-26")
+        print(dataset.get_reference_period())
+        dataset.update_in_hdx()
 
 14. You can view it on HDX before changing it back (if you have an API key):
 
-         dataset.set_reference_period("PREVIOUS DATE")
-         dataset.update_in_hdx()
+        dataset.set_reference_period("PREVIOUS DATE")
+        dataset.update_in_hdx()
 
 15. Exit and remove virtualenv:
 
-         exit()
-         deactivate
+        exit()
+        deactivate
 
      On Windows:
 
-         rd /s /q test
+        rd /s /q test
 
      On other OSs:
 
-         rm -rf test
+        rm -rf test
 
 # Building a Project
 
 ## Default Configuration for Facades
 
 The easiest way to get started is to use the facades and configuration defaults. The 
 facades set up both logging and HDX configuration.
@@ -688,15 +688,15 @@
 
     dataset.add_other_location("LOCATION")
 
 ### Tags
 
 HDX datasets can have tags which help people to find them eg. "common operational 
 dataset - cod", "refugees". These tags come from a predefined set of 
-[approved tags](https://docs.google.com/spreadsheets/d/e/2PACX-1vRjeajloIuQl8mfTSHU71ZgbHSgYYUgHrLqyjHSuQJ-zMqS3SVM9hJqMs72L-84LQ/pub?gid=1739051517&single=true&output=csv).
+[approved tags](https://docs.google.com/spreadsheets/d/e/2PACX-1vQD3ba751XbWS5GVwdJmzOF9mc7dnm56hE2U8di12JnpYkdseILmjfGSn1W7UVQzmHKSd6p8FWaXdFL/pub?gid=1768359211&single=true&output=csv).
 If you add tags that are not in the approved list, the library attempts to map them to
 approved tags based on a spreadsheet of tag mappings.
 
 
 If you wish to get the current tags, you can use this method:
 
     tags = dataset.get_tags()
```

### Comparing `hdx-python-api-6.0.0/pyproject.toml` & `hdx-python-api-6.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/setup.cfg` & `hdx-python-api-6.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/api/configuration.py` & `hdx-python-api-6.0.1/src/hdx/api/configuration.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/api/hdx_base_configuration.yml` & `hdx-python-api-6.0.1/src/hdx/api/hdx_base_configuration.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/api/locations.py` & `hdx-python-api-6.0.1/src/hdx/api/locations.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/dataset.py` & `hdx-python-api-6.0.1/src/hdx/data/dataset.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/dataset_title_helper.py` & `hdx-python-api-6.0.1/src/hdx/data/dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/date_helper.py` & `hdx-python-api-6.0.1/src/hdx/data/date_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/filestore_helper.py` & `hdx-python-api-6.0.1/src/hdx/data/filestore_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/hdxobject.py` & `hdx-python-api-6.0.1/src/hdx/data/hdxobject.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/indicator_resource_view_template.yml` & `hdx-python-api-6.0.1/src/hdx/data/indicator_resource_view_template.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/organization.py` & `hdx-python-api-6.0.1/src/hdx/data/organization.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/resource.py` & `hdx-python-api-6.0.1/src/hdx/data/resource.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/resource_matcher.py` & `hdx-python-api-6.0.1/src/hdx/data/resource_matcher.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/resource_view.py` & `hdx-python-api-6.0.1/src/hdx/data/resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/showcase.py` & `hdx-python-api-6.0.1/src/hdx/data/showcase.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/user.py` & `hdx-python-api-6.0.1/src/hdx/data/user.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/data/vocabulary.py` & `hdx-python-api-6.0.1/src/hdx/data/vocabulary.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,28 +476,32 @@
         """
         if configuration is None:
             configuration = Configuration.read()
         tag = tag.lower()
         tags_dict = cls.read_tags_mappings(configuration=configuration)
         tags = list()
         deleted_tags = list()
-        if cls.is_approved(tag):
-            tags.append(tag)
-        elif tag not in tags_dict.keys():
-            logger.error(
-                f"Unapproved tag {tag} not in tag mapping! For a list of approved tags see: {configuration['tags_list_url']}"
-            )
-            deleted_tags.append(tag)
+        whattodo = tags_dict.get(tag)
+        if whattodo is None:
+            if cls.is_approved(tag):
+                tags.append(tag)
+            else:
+                logger.error(
+                    f"Unapproved tag {tag} not in tags mappings! For a list of approved tags see: {configuration['tags_list_url']}"
+                )
+                deleted_tags.append(tag)
         else:
-            whattodo = tags_dict[tag]
             action = whattodo["Action to Take"]
             if action == "ok":
-                logger.error(
-                    f"Tag {tag} is not in CKAN approved tags but is in tags mappings! For a list of approved tags see: {configuration['tags_list_url']}"
-                )
+                if cls.is_approved(tag):
+                    tags.append(tag)
+                else:
+                    logger.error(
+                        f"Tag {tag} is not in CKAN approved tags but is in tags mappings! For a list of approved tags see: {configuration['tags_list_url']}"
+                    )
             elif action == "delete":
                 if log_deleted:
                     logger.info(
                         f"Tag {tag} is invalid and won't be added! For a list of approved tags see: {configuration['tags_list_url']}"
                     )
                 deleted_tags.append(tag)
             elif action == "merge":
```

### Comparing `hdx-python-api-6.0.0/src/hdx/facades/infer_arguments.py` & `hdx-python-api-6.0.1/src/hdx/facades/infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/facades/keyword_arguments.py` & `hdx-python-api-6.0.1/src/hdx/facades/keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx/facades/simple.py` & `hdx-python-api-6.0.1/src/hdx/facades/simple.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/src/hdx_python_api.egg-info/PKG-INFO` & `hdx-python-api-6.0.1/src/hdx_python_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hdx-python-api
-Version: 6.0.0
+Version: 6.0.1
 Summary: HDX Python API for interacting with the Humanitarian Data Exchange
 Home-page: https://github.com/OCHA-DAP/hdx-python-api
 Author: Michael Rans
 Author-email: rans@email.com
 License: MIT
 Keywords: HDX,API,library,CKAN
 Platform: any
```

### Comparing `hdx-python-api-6.0.0/src/hdx_python_api.egg-info/SOURCES.txt` & `hdx-python-api-6.0.1/src/hdx_python_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/Accepted_Tags.csv` & `hdx-python-api-6.0.1/tests/fixtures/Accepted_Tags.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/Tag_Mapping.csv` & `hdx-python-api-6.0.1/tests/fixtures/Tag_Mapping.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.json` & `hdx-python-api-6.0.1/tests/fixtures/config/hdx_dataset_static.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/config/hdx_dataset_static.yml` & `hdx-python-api-6.0.1/tests/fixtures/config/hdx_dataset_static.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/config/hdx_datasource_topline.json` & `hdx-python-api-6.0.1/tests/fixtures/config/hdx_datasource_topline.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/config/hdx_resource_view_static.yml` & `hdx-python-api-6.0.1/tests/fixtures/config/hdx_resource_view_static.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/dataset_search_results.yml` & `hdx-python-api-6.0.1/tests/fixtures/dataset_search_results.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx` & `hdx-python-api-6.0.1/tests/fixtures/datastore/ACLED-All-Africa-File_20170101-to-20170708.xlsx`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/gen_resource/conflict_data_alg.csv` & `hdx-python-api-6.0.1/tests/fixtures/gen_resource/conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/gen_resource/qc_conflict_data_alg.csv` & `hdx-python-api-6.0.1/tests/fixtures/gen_resource/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/gen_resource/test_data_no_years.csv` & `hdx-python-api-6.0.1/tests/fixtures/gen_resource/test_data_no_years.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/organization_show_results.yml` & `hdx-python-api-6.0.1/tests/fixtures/organization_show_results.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv` & `hdx-python-api-6.0.1/tests/fixtures/qc_from_rows/qc_conflict_data_alg.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/resource_formats.json` & `hdx-python-api-6.0.1/tests/fixtures/resource_formats.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/showcase_all_search_results.yml` & `hdx-python-api-6.0.1/tests/fixtures/showcase_all_search_results.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/test_data.csv` & `hdx-python-api-6.0.1/tests/fixtures/test_data.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/test_data.zip` & `hdx-python-api-6.0.1/tests/fixtures/test_data.zip`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_data_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/dem_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/dem_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_data_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/opri_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/opri_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/opri_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/qc_sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/sdg_data_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/sdg_indicatorlist_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/sdg_metadata_zwe.csv`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_dataset.json` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/unesco_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_dataset_resources/unesco_update_dataset.json` & `hdx-python-api-6.0.1/tests/fixtures/update_dataset_resources/unesco_update_dataset.json`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources.yml` & `hdx-python-api-6.0.1/tests/fixtures/update_logic/update_logic_resources.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/fixtures/update_logic/update_logic_resources_new.yml` & `hdx-python-api-6.0.1/tests/fixtures/update_logic/update_logic_resources_new.yml`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/api/test_configuration.py` & `hdx-python-api-6.0.1/tests/hdx/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/api/test_locations.py` & `hdx-python-api-6.0.1/tests/hdx/api/test_locations.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/conftest.py` & `hdx-python-api-6.0.1/tests/hdx/conftest.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/__init__.py` & `hdx-python-api-6.0.1/tests/hdx/data/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_dataset_core.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_dataset_core.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_dataset_noncore.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_dataset_noncore.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,19 +447,35 @@
             "fatalities - deaths",
         ]
         dataset.add_tag("cholera")
         assert dataset.get_tags() == [
             "violence and conflict",
             "fatalities - deaths",
             "cholera",
+            "disease",
         ]
         dataset.remove_tag("violence and conflict")
-        assert dataset.get_tags() == ["fatalities - deaths", "cholera"]
+        assert dataset.get_tags() == [
+            "fatalities - deaths",
+            "cholera",
+            "disease",
+        ]
         dataset.add_tag("cholera")
-        assert dataset.get_tags() == ["fatalities - deaths", "cholera"]
+        assert dataset.get_tags() == [
+            "fatalities - deaths",
+            "cholera",
+            "disease",
+        ]
+        dataset.add_tag("cbi")
+        assert dataset.get_tags() == [
+            "fatalities - deaths",
+            "cholera",
+            "disease",
+            "cash assistance",
+        ]
 
     def test_add_clean_tags(self, configuration, vocabulary_read):
         Vocabulary.set_tagsdict(None)
         Vocabulary.read_tags_mappings(failchained=False)
         datasetdata = copy.deepcopy(dataset_data)
         dataset = Dataset(datasetdata)
         assert dataset.get_tags() == ["conflict", "political violence"]
```

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_dataset_title_helper.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_dataset_title_helper.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_organization.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_organization.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_resource.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_resource.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_resource_view.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_resource_view.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_showcase.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_showcase.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_update_dataset_resources.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_update_dataset_resources.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_update_logic.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_update_logic.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_user.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_user.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/data/test_vocabulary.py` & `hdx-python-api-6.0.1/tests/hdx/data/test_vocabulary.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/facades/__init__.py` & `hdx-python-api-6.0.1/tests/hdx/facades/__init__.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/facades/test_infer_arguments.py` & `hdx-python-api-6.0.1/tests/hdx/facades/test_infer_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/facades/test_keyword_arguments.py` & `hdx-python-api-6.0.1/tests/hdx/facades/test_keyword_arguments.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/tests/hdx/facades/test_simple.py` & `hdx-python-api-6.0.1/tests/hdx/facades/test_simple.py`

 * *Files identical despite different names*

### Comparing `hdx-python-api-6.0.0/workingexample/my_resource.xlsx` & `hdx-python-api-6.0.1/workingexample/my_resource.xlsx`

 * *Files identical despite different names*
