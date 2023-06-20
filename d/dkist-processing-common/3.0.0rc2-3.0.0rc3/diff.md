# Comparing `tmp/dkist-processing-common-3.0.0rc2.tar.gz` & `tmp/dkist-processing-common-3.0.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist-processing-common-3.0.0rc2.tar", last modified: Tue Jun 13 17:25:13 2023, max compression
+gzip compressed data, was "dkist-processing-common-3.0.0rc3.tar", last modified: Tue Jun 20 16:49:37 2023, max compression
```

## Comparing `dkist-processing-common-3.0.0rc2.tar` & `dkist-processing-common-3.0.0rc3.tar`

### file list

```diff
@@ -1,125 +1,133 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.591911 dkist-processing-common-3.0.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-13 17:25:13.591911 dkist-processing-common-3.0.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.583911 dkist-processing-common-3.0.0rc2/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/changelog/140.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.583911 dkist-processing-common-3.0.0rc2/dkist_processing_common/
--rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.583911 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/config.py
--rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.583911 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/bytes.py
--rw-rw-rw-   0 root         (0) root         (0)      546 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/bytesio.py
--rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/fits.py
--rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/json.py
--rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/path.py
--rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/str.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.583911 dkist-processing-common-3.0.0rc2/dkist_processing_common/fonts/
--rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/fonts/Lato-Regular.ttf
--rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/fonts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/manual.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.587911 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/
--rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/graphql.py
--rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/message.py
--rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/quality_json_encoders.py
--rw-rw-rw-   0 root         (0) root         (0)     7365 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/tags.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/models/wavelength.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.587911 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/dsps_repeat.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/experiment_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/l1_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/proposal_id_bud.py
--rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/quality.py
--rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/single_value_single_key_flower.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/time.py
--rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/unique_bud.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.587911 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     9049 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/base.py
--rw-rw-rw-   0 root         (0) root         (0)    10675 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/l1_output_data.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.587911 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1930 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/fits.py
--rw-rw-rw-   0 root         (0) root         (0)     6718 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/globus.py
--rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/interservice_bus.py
--rw-rw-rw-   0 root         (0) root         (0)    13164 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/metadata_store.py
--rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/object_store.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.587911 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/quality/
--rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/quality/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/quality/_base.py
--rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.591911 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_base.py
--rw-rw-rw-   0 root         (0) root         (0)     7126 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_codecs.py
--rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_constants.py
--rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_cs_step.py
--rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_dkist_location.py
--rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_fits_flowers.py
--rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_flower_pot.py
--rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_input_dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     1331 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_l1_output_data_base.py
--rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_parse_l0_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_publish_catalog_messages.py
--rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_quality.py
--rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_quality_mixin.py
--rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_scratch.py
--rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_tags.py
--rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_teardown.py
--rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_transfer_input_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py
--rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_workflow_task_base.py
--rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.583911 dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-13 17:25:13.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4548 2023-06-13 17:25:13.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-13 17:25:13.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-13 17:25:13.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-13 17:25:13.000000 dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.591911 dkist-processing-common-3.0.0rc2/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/docs/requirements.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-13 17:25:13.591911 dkist-processing-common-3.0.0rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-13 17:25:13.591911 dkist-processing-common-3.0.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-13 17:25:07.000000 dkist-processing-common-3.0.0rc2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.456444 dkist-processing-common-3.0.0rc3/
+-rw-rw-rw-   0 root         (0) root         (0)     2481 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      844 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      429 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13348 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-20 16:49:37.456444 dkist-processing-common-3.0.0rc3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3732 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2433 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.424443 dkist-processing-common-3.0.0rc3/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/changelog/.gitempty
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/changelog/139.feature.2.rst
+-rw-rw-rw-   0 root         (0) root         (0)       85 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/changelog/139.feature.rst
+-rw-rw-rw-   0 root         (0) root         (0)      342 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/changelog/140.feature.rst
+-rwxrwxrwx   0 root         (0) root         (0)      642 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.424443 dkist-processing-common-3.0.0rc3/dkist_processing_common/
+-rw-rw-rw-   0 root         (0) root         (0)      317 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.428444 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     2409 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1178 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1580 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     8215 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     5641 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.432444 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/bytes.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)      900 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/iobase.py
+-rw-rw-rw-   0 root         (0) root         (0)      939 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/json.py
+-rw-rw-rw-   0 root         (0) root         (0)      197 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/path.py
+-rw-rw-rw-   0 root         (0) root         (0)      679 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/str.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.432444 dkist-processing-common-3.0.0rc3/dkist_processing_common/fonts/
+-rw-rw-rw-   0 root         (0) root         (0)   656568 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/fonts/Lato-Regular.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      101 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/fonts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6987 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/manual.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.436444 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/
+-rw-rw-rw-   0 root         (0) root         (0)       74 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4766 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     3453 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     4176 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)     3514 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/graphql.py
+-rw-rw-rw-   0 root         (0) root         (0)     1109 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     3408 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1096 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/quality_json_encoders.py
+-rw-rw-rw-   0 root         (0) root         (0)     7510 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/tags.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/models/wavelength.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.440444 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       67 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6381 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     1827 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/dsps_repeat.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/experiment_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1767 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)      921 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     2451 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/l1_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      677 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/proposal_id_bud.py
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     1230 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/single_value_single_key_flower.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/time.py
+-rw-rw-rw-   0 root         (0) root         (0)     1669 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/unique_bud.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.444444 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      504 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11470 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     9049 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8689 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/l1_output_data.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.444444 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3243 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2033 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     6887 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/globus.py
+-rw-rw-rw-   0 root         (0) root         (0)     6813 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     2421 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/interservice_bus.py
+-rw-rw-rw-   0 root         (0) root         (0)    13164 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/metadata_store.py
+-rw-rw-rw-   0 root         (0) root         (0)     3612 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/object_store.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.448444 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/quality/
+-rw-rw-rw-   0 root         (0) root         (0)      383 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/quality/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8287 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/quality/_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    47886 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/quality/_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     3153 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     8329 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     8859 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     1374 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     4863 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     7974 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    18550 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.456444 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    24490 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     3023 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     7501 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_codecs.py
+-rw-rw-rw-   0 root         (0) root         (0)     4203 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     2291 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_cs_step.py
+-rw-rw-rw-   0 root         (0) root         (0)     4097 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_debug_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)      513 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_dkist_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     4682 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_fits.py
+-rw-rw-rw-   0 root         (0) root         (0)     8808 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)    12959 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_fits_flowers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2258 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_flower_pot.py
+-rw-rw-rw-   0 root         (0) root         (0)    19450 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_input_dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3159 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_output_data_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     6276 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)    10476 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_parse_l0_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_publish_catalog_messages.py
+-rw-rw-rw-   0 root         (0) root         (0)     9168 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)    36336 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_quality_mixin.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_scratch.py
+-rw-rw-rw-   0 root         (0) root         (0)     4569 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     5745 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_teardown.py
+-rw-rw-rw-   0 root         (0) root         (0)     6666 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_transfer_input_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2270 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_transfer_l1_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    13218 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_trial_output_data.py
+-rw-rw-rw-   0 root         (0) root         (0)    10527 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_workflow_task_base.py
+-rw-rw-rw-   0 root         (0) root         (0)    14952 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.428444 dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     4327 2023-06-20 16:49:37.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4899 2023-06-20 16:49:37.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-20 16:49:37.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      603 2023-06-20 16:49:37.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       24 2023-06-20 16:49:37.000000 dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.456444 dkist-processing-common-3.0.0rc3/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      120 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1890 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      113 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/docs/requirements.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-20 16:49:37.456444 dkist-processing-common-3.0.0rc3/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      780 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1690 2023-06-20 16:49:37.460444 dkist-processing-common-3.0.0rc3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2023-06-20 16:49:28.000000 dkist-processing-common-3.0.0rc3/setup.py
```

### Comparing `dkist-processing-common-3.0.0rc2/.gitignore` & `dkist-processing-common-3.0.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/.pre-commit-config.yaml` & `dkist-processing-common-3.0.0rc3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/CHANGELOG.rst` & `dkist-processing-common-3.0.0rc3/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/PKG-INFO` & `dkist-processing-common-3.0.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc2/README.rst` & `dkist-processing-common-3.0.0rc3/README.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/bitbucket-pipelines.yml` & `dkist-processing-common-3.0.0rc3/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/check_changelog_updated.sh` & `dkist-processing-common-3.0.0rc3/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/config.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/config.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/constants.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/dkist_location.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/graphql.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/scratch.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/_util/tags.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/_util/tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/fits.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/fits.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 from typing import Type
 
 import numpy as np
 from astropy.io import fits
 from astropy.io.fits import Header
 
-from dkist_processing_common.codecs.bytesio import bytesio_encoder
+from dkist_processing_common.codecs.iobase import iobase_encoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 
 
 def fits_array_encoder(data: np.ndarray, header: Header | None = None) -> bytes:
     """Convert an array to raw bytes representing a fits `HDUList`."""
     if not isinstance(data, np.ndarray):
         raise ValueError(f"Input type {type(data)} is not np.ndarray")
@@ -22,15 +22,15 @@
 def fits_hdulist_encoder(hdu_list: fits.HDUList) -> bytes:
     """Convert an `HDUList` to raw bytes for writing to a file."""
     if not isinstance(hdu_list, fits.HDUList):
         raise ValueError(f"Input type {type(hdu_list)} is not fits.HDUList")
     file_obj = BytesIO()
     hdu_list.writeto(file_obj, checksum=True)
     file_obj.seek(0)
-    return bytesio_encoder(file_obj)
+    return iobase_encoder(file_obj)
 
 
 def fits_hdu_decoder(path: Path) -> fits.PrimaryHDU | fits.CompImageHDU:
     """Read a Path with `fits` to produce an `HDUList`."""
     hdu_list = fits.open(path)
     return _extract_hdu(hdu_list)
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/json.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/json.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/codecs/str.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/codecs/str.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/fonts/Lato-Regular.ttf` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/fonts/Lato-Regular.ttf`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/manual.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/manual.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/constants.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/fits_access.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/flower_pot.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/graphql.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/graphql.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/message.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/message.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/parameters.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/quality.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/quality_json_encoders.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/quality_json_encoders.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/tags.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/tags.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     modstate = "MODSTATE"
     dsps_repeat = "DSPS_REPEAT"
     calibrated = "CALIBRATED"  # A flag to indicate the data has been calibrated but not yet output
     quality = "QUALITY"
     exposure_time = "EXP_TIME"
     quality_task = "QUALITY_TASK"
     parameter = "PARAMETER"
+    debug = "DEBUG"
 
 
 class Tag:
     """Controlled methods for creating tags from stems + optional suffixes."""
 
     @staticmethod
     def format_tag(stem: StemName | str, *parts):
@@ -157,14 +158,19 @@
 
         Returns
         -------
         A movie tag
         """
         return cls.format_tag(StemName.movie)
 
+    @classmethod
+    def debug(cls) -> str:
+        """Return a debug tag."""
+        return cls.format_tag(StemName.debug)
+
     # Dynamic Tags
     @classmethod
     def task(cls, ip_task_type: str):
         """
         Return a task tag for the given task type.
 
         Parameters
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/models/wavelength.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/models/wavelength.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/cs_step.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/dsps_repeat.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/dsps_repeat.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/experiment_id_bud.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/experiment_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/id_bud.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/l0_fits_access.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/l1_fits_access.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/proposal_id_bud.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/proposal_id_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/quality.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/single_value_single_key_flower.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/single_value_single_key_flower.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/time.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/time.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/parsers/unique_bud.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/parsers/unique_bud.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/assemble_movie.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/base.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/l1_output_data.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/l1_output_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,65 @@
-"""Task(s) for the transfer out of data from a processing pipeline."""
+"""Task(s) for the transfer and publishing of L1 data from a production run of a processing pipeline."""
 import logging
-from abc import ABC
-from functools import cached_property
 from pathlib import Path
 from typing import Iterable
 
 from dkist_processing_common.models.message import CatalogFrameMessage
 from dkist_processing_common.models.message import CatalogObjectMessage
 from dkist_processing_common.models.message import CreateQualityReportMessage
 from dkist_processing_common.models.tags import Tag
-from dkist_processing_common.tasks import WorkflowTaskBase
 from dkist_processing_common.tasks.mixin.globus import GlobusMixin
-from dkist_processing_common.tasks.mixin.globus import GlobusTransferItem
 from dkist_processing_common.tasks.mixin.interservice_bus import InterserviceBusMixin
-from dkist_processing_common.tasks.mixin.object_store import ObjectStoreMixin
 
 
 __all__ = [
     "AddDatasetReceiptAccount",
     "PublishCatalogAndQualityMessages",
     "TransferL1Data",
     "L1OutputDataBase",
     "SubmitQuality",
 ]
 
 from dkist_processing_common.tasks.mixin.quality import QualityMixin
+from dkist_processing_common.tasks.output_data_base import OutputDataBase, TransferDataBase
 
 logger = logging.getLogger(__name__)
 
 
-class L1OutputDataBase(WorkflowTaskBase, QualityMixin, ABC):
-    """Subclass of WorkflowTaskBase which encapsulates common level 1 output data methods."""
-
-    @cached_property
-    def destination_bucket(self) -> str:
-        """Get the destination bucket."""
-        return self.metadata_store_recipe_run_configuration().get("destination_bucket", "data")
-
-    def format_object_key(self, path: Path) -> str:
-        """
-        Convert output paths into object store keys.
-
-        Parameters
-        ----------
-        path: the Path to convert
-
-        Returns
-        -------
-        formatted path in the object store
-        """
-        object_key = self.destination_folder / Path(path.name)
-        return str(object_key)
-
-    @property
-    def destination_folder(self) -> Path:
-        """Format the destination folder."""
-        return self.destination_root_folder / Path(self.constants.dataset_id)
-
-    @property
-    def destination_root_folder(self) -> Path:
-        """Format the destination root folder."""
-        return Path(self.constants.proposal_id)
+class L1OutputDataBase(OutputDataBase, QualityMixin):
+    """Subclass of OutputDataBase which encapsulates common level 1 output data methods."""
 
     @property
     def dataset_has_quality_report(self) -> bool:
         """Return True if a quality report has been submitted to the metadata-store."""
         return self.metadata_store_quality_report_exists(dataset_id=self.constants.dataset_id)
 
 
-class TransferL1Data(L1OutputDataBase, GlobusMixin, ObjectStoreMixin):
+class TransferL1Data(TransferDataBase, GlobusMixin):
     """Task class for transferring Level 1 processed data to the object store."""
 
+    def transfer_objects(self):
+        """Transfer movie and L1 output frames."""
+        with self.apm_task_step("Upload movie"):
+            # Movie needs to be transferred separately as the movie headers need to go with it
+            self.transfer_movie()
+
+        with self.apm_task_step("Upload science frames"):
+            self.transfer_output_frames()
+
     def transfer_output_frames(self):
         """Create a Globus transfer for all output data."""
-        science_frame_paths: list[Path] = list(self.read(tags=[Tag.output(), Tag.frame()]))
-        transfer_items = []
-        for p in science_frame_paths:
-            object_key = self.format_object_key(p)
-            destination_path = Path(self.destination_bucket, object_key)
-            item = GlobusTransferItem(
-                source_path=p,
-                destination_path=destination_path,
-            )
-            transfer_items.append(item)
+        transfer_items = self.build_output_frame_transfer_list()
+
         logger.info(
             f"Preparing globus transfer {len(transfer_items)} items: "
             f"recipe_run_id={self.recipe_run_id}. "
             f"transfer_items={transfer_items[:3]}..."
         )
-        # Send transfer
+
         self.globus_transfer_scratch_to_object_store(
             transfer_items=transfer_items,
             label=f"Transfer science frames for recipe_run_id {self.recipe_run_id}",
         )
 
     def transfer_movie(self):
         """Transfer the movie to the object store."""
@@ -115,33 +82,14 @@
         self.object_store_upload_movie(
             movie=movie,
             bucket=self.destination_bucket,
             object_key=movie_object_key,
             content_type="video/mp4",
         )
 
-    def remove_folder_objects(self):
-        """Remove folder objects that would have been added by the Globus transfer."""
-        removed_object_keys = self.object_store_remove_folder_objects(
-            bucket=self.destination_bucket, path=self.destination_root_folder
-        )
-        logger.info(
-            f"Removed folder objects in {self.destination_bucket} bucket. {removed_object_keys=}"
-        )
-
-    def run(self) -> None:
-        """Transfer the data."""
-        with self.apm_task_step("Upload movie"):
-            # Movie needs to be transferred separately as the movie headers need to go with it
-            self.transfer_movie()
-        with self.apm_task_step("Upload science frames"):
-            self.transfer_output_frames()
-        with self.apm_task_step("Remove folder objects"):
-            self.remove_folder_objects()
-
 
 class PublishCatalogAndQualityMessages(L1OutputDataBase, InterserviceBusMixin):
     """Task class for publishing Catalog and Quality Messages."""
 
     def frame_messages(self, paths: Iterable[Path]) -> list[CatalogFrameMessage]:
         """
         Create the frame messages.
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/fits.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/fits.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,12 +40,17 @@
         )
 
     def fits_data_write(
         self,
         hdu_list: fits.HDUList,
         tags: tag_type_hint,
         relative_path: Path | str | None = None,
+        overwrite: bool = False,
     ) -> Path:
         """Write the fits object to a file with the given path and tag with the given tags."""
         return self.write(
-            data=hdu_list, tags=tags, relative_path=relative_path, encoder=fits_hdulist_encoder
+            data=hdu_list,
+            tags=tags,
+            relative_path=relative_path,
+            encoder=fits_hdulist_encoder,
+            overwrite=overwrite,
         )
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/globus.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/globus.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 class GlobusTransferItem:
     """Dataclass used to support globus transfers."""
 
     source_path: str | Path
     destination_path: str | Path
     recursive: bool = False  # file
 
+    def __hash__(self) -> int:
+        """Hash so we can do set stuff on these items."""
+        return hash((self.source_path, self.destination_path, self.recursive))
+
 
 class GlobusMixin:
     """Mixin to add methods to a Task to support globus transfers."""
 
     @property
     def globus_transfer_client(self) -> TransferClient:
         """Get the globus transfer client, creating it if it doesn't exist."""
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/input_dataset.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/interservice_bus.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/interservice_bus.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/metadata_store.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/metadata_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/object_store.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/object_store.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/quality/_base.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/quality/_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/mixin/quality/_metrics.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/mixin/quality/_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/quality_metrics.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/teardown.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/transfer_input_data.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tasks/write_l1.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/conftest.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_assemble_movie.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_base.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_codecs.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_codecs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import json
 from io import BytesIO
+from io import StringIO
 from pathlib import Path
 from uuid import uuid4
 
 import numpy as np
 import pytest
 from astropy.io import fits
 from astropy.io.fits import CompImageHDU
 from astropy.io.fits import HDUList
 from astropy.io.fits import Header
 from astropy.io.fits import PrimaryHDU
 
 from dkist_processing_common.codecs.bytes import bytes_decoder
 from dkist_processing_common.codecs.bytes import bytes_encoder
-from dkist_processing_common.codecs.bytesio import bytesio_decoder
-from dkist_processing_common.codecs.bytesio import bytesio_encoder
 from dkist_processing_common.codecs.fits import fits_access_decoder
 from dkist_processing_common.codecs.fits import fits_array_decoder
 from dkist_processing_common.codecs.fits import fits_array_encoder
 from dkist_processing_common.codecs.fits import fits_hdu_decoder
 from dkist_processing_common.codecs.fits import fits_hdulist_encoder
+from dkist_processing_common.codecs.iobase import iobase_decoder
+from dkist_processing_common.codecs.iobase import iobase_encoder
 from dkist_processing_common.codecs.json import json_decoder
 from dkist_processing_common.codecs.json import json_encoder
 from dkist_processing_common.codecs.str import str_decoder
 from dkist_processing_common.codecs.str import str_encoder
 from dkist_processing_common.models.fits_access import FitsAccessBase
 
 
@@ -127,15 +128,15 @@
         self.foo = self.header["foo"]
 
 
 @pytest.mark.parametrize(
     "data_fixture_name, encoder_function",
     [
         pytest.param("bytes_object", bytes_encoder, id="bytes"),
-        pytest.param("bytesIO_object", bytesio_encoder, id="BytesIO"),
+        pytest.param("bytesIO_object", iobase_encoder, id="BytesIO"),
         pytest.param("ndarray_object", fits_array_encoder, id="fits ndarray"),
         pytest.param("primary_hdu_list", fits_hdulist_encoder, id="fits uncompressed HDUList"),
         pytest.param("compressed_hdu_list", fits_hdulist_encoder, id="fits compressed HDUList"),
         pytest.param("dictionary", json_encoder, id="json"),
         pytest.param("string", str_encoder, id="str"),
     ],
 )
@@ -145,14 +146,27 @@
     When: Encoding data with the correct codec
     Then: A `bytes` object is returned
     """
     data = request.getfixturevalue(data_fixture_name)
     assert type(encoder_function(data)) is bytes
 
 
+def test_non_bytes_IOBase_encoder():
+    """
+    Given: String data in a StringIO object
+    When: Trying to encode with the iobase_encoder
+    Then: An error is raised
+    """
+    io_obj = StringIO()
+    io_obj.write("foo")
+    io_obj.seek(0)
+    with pytest.raises(ValueError, match="produces str data"):
+        iobase_encoder(io_obj)
+
+
 @pytest.mark.parametrize(
     "data_fixture_name, path_fixture_name, decoder_function",
     [
         pytest.param("bytes_object", "path_to_bytes", bytes_decoder, id="bytes"),
         pytest.param("dictionary", "path_to_json", json_decoder, id="json"),
         pytest.param("string", "path_to_str", str_decoder, id="str"),
     ],
@@ -170,18 +184,18 @@
     decoded_value = decoder_function(file_path)
     assert expected == decoded_value
 
 
 def test_bytesio_decoder(bytesIO_object, path_to_bytesIO):
     """
     Given: Path to a file containing binary data
-    When: Decoding the file with the bytesio_decoder
+    When: Decoding the file with the iobase_decoder
     Then: The correct data and type are returned
     """
-    decoded_object = bytesio_decoder(path_to_bytesIO)
+    decoded_object = iobase_decoder(path_to_bytesIO, io_class=BytesIO)
 
     bytesIO_object.seek(0)
     assert decoded_object.read() == bytesIO_object.read()
 
 
 @pytest.mark.parametrize(
     "path_fixture_name",
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_constants.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_cs_step.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_cs_step.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_dkist_location.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_dkist_location.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_fits_access.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_fits_flowers.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_fits_flowers.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_flower_pot.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_flower_pot.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_input_dataset.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_input_dataset.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_parameters.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_parse_l0_input_data.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_parse_l0_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_publish_catalog_messages.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_publish_catalog_messages.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_quality.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_quality.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_quality_mixin.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_quality_mixin.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_scratch.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_scratch.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_tags.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_teardown.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_teardown.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_transfer_input_data.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_transfer_input_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_transfer_l1_output_data.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_transfer_l1_output_data.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_workflow_task_base.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_workflow_task_base.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common/tests/test_write_l1.py` & `dkist-processing-common-3.0.0rc3/dkist_processing_common/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/PKG-INFO` & `dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-common
-Version: 3.0.0rc2
+Version: 3.0.0rc3
 Summary: Common task classes used by the DKIST Science Data Processing pipelines to process DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-common/src/master/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/common
 Classifier: Programming Language :: Python
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/SOURCES.txt` & `dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 README.rst
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 changelog/.gitempty
+changelog/139.feature.2.rst
+changelog/139.feature.rst
 changelog/140.feature.rst
 dkist_processing_common/__init__.py
 dkist_processing_common/manual.py
 dkist_processing_common.egg-info/PKG-INFO
 dkist_processing_common.egg-info/SOURCES.txt
 dkist_processing_common.egg-info/dependency_links.txt
 dkist_processing_common.egg-info/requires.txt
@@ -22,16 +24,16 @@
 dkist_processing_common/_util/constants.py
 dkist_processing_common/_util/dkist_location.py
 dkist_processing_common/_util/graphql.py
 dkist_processing_common/_util/scratch.py
 dkist_processing_common/_util/tags.py
 dkist_processing_common/codecs/__init__.py
 dkist_processing_common/codecs/bytes.py
-dkist_processing_common/codecs/bytesio.py
 dkist_processing_common/codecs/fits.py
+dkist_processing_common/codecs/iobase.py
 dkist_processing_common/codecs/json.py
 dkist_processing_common/codecs/path.py
 dkist_processing_common/codecs/str.py
 dkist_processing_common/fonts/Lato-Regular.ttf
 dkist_processing_common/fonts/__init__.py
 dkist_processing_common/models/__init__.py
 dkist_processing_common/models/constants.py
@@ -56,20 +58,23 @@
 dkist_processing_common/parsers/single_value_single_key_flower.py
 dkist_processing_common/parsers/time.py
 dkist_processing_common/parsers/unique_bud.py
 dkist_processing_common/tasks/__init__.py
 dkist_processing_common/tasks/assemble_movie.py
 dkist_processing_common/tasks/base.py
 dkist_processing_common/tasks/l1_output_data.py
+dkist_processing_common/tasks/output_data_base.py
 dkist_processing_common/tasks/parse_l0_input_data.py
 dkist_processing_common/tasks/quality_metrics.py
 dkist_processing_common/tasks/teardown.py
 dkist_processing_common/tasks/transfer_input_data.py
+dkist_processing_common/tasks/trial_output_data.py
 dkist_processing_common/tasks/write_l1.py
 dkist_processing_common/tasks/mixin/__init__.py
+dkist_processing_common/tasks/mixin/debug_frame.py
 dkist_processing_common/tasks/mixin/fits.py
 dkist_processing_common/tasks/mixin/globus.py
 dkist_processing_common/tasks/mixin/input_dataset.py
 dkist_processing_common/tasks/mixin/interservice_bus.py
 dkist_processing_common/tasks/mixin/metadata_store.py
 dkist_processing_common/tasks/mixin/object_store.py
 dkist_processing_common/tasks/mixin/quality/__init__.py
@@ -78,30 +83,33 @@
 dkist_processing_common/tests/__init__.py
 dkist_processing_common/tests/conftest.py
 dkist_processing_common/tests/test_assemble_movie.py
 dkist_processing_common/tests/test_base.py
 dkist_processing_common/tests/test_codecs.py
 dkist_processing_common/tests/test_constants.py
 dkist_processing_common/tests/test_cs_step.py
+dkist_processing_common/tests/test_debug_frame.py
 dkist_processing_common/tests/test_dkist_location.py
+dkist_processing_common/tests/test_fits.py
 dkist_processing_common/tests/test_fits_access.py
 dkist_processing_common/tests/test_fits_flowers.py
 dkist_processing_common/tests/test_flower_pot.py
 dkist_processing_common/tests/test_input_dataset.py
-dkist_processing_common/tests/test_l1_output_data_base.py
+dkist_processing_common/tests/test_output_data_base.py
 dkist_processing_common/tests/test_parameters.py
 dkist_processing_common/tests/test_parse_l0_input_data.py
 dkist_processing_common/tests/test_publish_catalog_messages.py
 dkist_processing_common/tests/test_quality.py
 dkist_processing_common/tests/test_quality_mixin.py
 dkist_processing_common/tests/test_scratch.py
 dkist_processing_common/tests/test_tags.py
 dkist_processing_common/tests/test_teardown.py
 dkist_processing_common/tests/test_transfer_input_data.py
 dkist_processing_common/tests/test_transfer_l1_output_data.py
+dkist_processing_common/tests/test_trial_output_data.py
 dkist_processing_common/tests/test_workflow_task_base.py
 dkist_processing_common/tests/test_write_l1.py
 docs/Makefile
 docs/changelog.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
```

### Comparing `dkist-processing-common-3.0.0rc2/dkist_processing_common.egg-info/requires.txt` & `dkist-processing-common-3.0.0rc3/dkist_processing_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/docs/Makefile` & `dkist-processing-common-3.0.0rc3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/docs/conf.py` & `dkist-processing-common-3.0.0rc3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/docs/make.bat` & `dkist-processing-common-3.0.0rc3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/licenses/LICENSE.rst` & `dkist-processing-common-3.0.0rc3/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/pyproject.toml` & `dkist-processing-common-3.0.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist-processing-common-3.0.0rc2/setup.cfg` & `dkist-processing-common-3.0.0rc3/setup.cfg`

 * *Files identical despite different names*

