# Comparing `tmp/hedtools-0.2.0.tar.gz` & `tmp/hedtools-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\hedtools-0.2.0.tar", last modified: Tue Feb 14 21:42:44 2023, max compression
+gzip compressed data, was "dist\hedtools-0.3.0.tar", last modified: Tue Jun 20 20:41:22 2023, max compression
```

## Comparing `hedtools-0.2.0.tar` & `hedtools-0.3.0.tar`

### file list

```diff
@@ -1,140 +1,149 @@
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/
--rw-rw-rw-   0        0        0     1102 2022-02-04 21:37:41.000000 hedtools-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       70 2022-06-20 19:04:23.000000 hedtools-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5504 2023-02-14 21:42:44.000000 hedtools-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4866 2023-02-14 21:37:40.000000 hedtools-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/
--rw-rw-rw-   0        0        0      792 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/__init__.py
--rw-rw-rw-   0        0        0      518 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/_version.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/errors/
--rw-rw-rw-   0        0        0      321 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/errors/__init__.py
--rw-rw-rw-   0        0        0    15247 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/errors/error_messages.py
--rw-rw-rw-   0        0        0    21390 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/errors/error_reporter.py
--rw-rw-rw-   0        0        0     4435 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/errors/error_types.py
--rw-rw-rw-   0        0        0     4408 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/errors/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/models/
--rw-rw-rw-   0        0        0      712 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/__init__.py
--rw-rw-rw-   0        0        0    27105 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/base_input.py
--rw-rw-rw-   0        0        0    21515 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/column_mapper.py
--rw-rw-rw-   0        0        0     6908 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/column_metadata.py
--rw-rw-rw-   0        0        0    11343 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/def_mapper.py
--rw-rw-rw-   0        0        0     6525 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/definition_dict.py
--rw-rw-rw-   0        0        0     3573 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/definition_entry.py
--rw-rw-rw-   0        0        0    15753 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/expression_parser.py
--rw-rw-rw-   0        0        0    19210 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/hed_group.py
--rw-rw-rw-   0        0        0     9594 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/hed_ops.py
--rw-rw-rw-   0        0        0    13543 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/hed_string.py
--rw-rw-rw-   0        0        0     4555 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/hed_string_group.py
--rw-rw-rw-   0        0        0    19702 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/hed_tag.py
--rw-rw-rw-   0        0        0      627 2022-09-12 19:32:19.000000 hedtools-0.2.0/hed/models/model_constants.py
--rw-rw-rw-   0        0        0     4659 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/onset_mapper.py
--rw-rw-rw-   0        0        0     9994 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/sidecar.py
--rw-rw-rw-   0        0        0    11165 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/sidecar_base.py
--rw-rw-rw-   0        0        0     2516 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/spreadsheet_input.py
--rw-rw-rw-   0        0        0     4276 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/tabular_input.py
--rw-rw-rw-   0        0        0      942 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/models/timeseries_input.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/schema/
--rw-rw-rw-   0        0        0      590 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/__init__.py
--rw-rw-rw-   0        0        0    19001 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/hed_cache.py
--rw-rw-rw-   0        0        0    26152 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/hed_schema.py
--rw-rw-rw-   0        0        0     1861 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/schema/hed_schema_constants.py
--rw-rw-rw-   0        0        0    10273 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/hed_schema_entry.py
--rw-rw-rw-   0        0        0     6906 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/hed_schema_group.py
--rw-rw-rw-   0        0        0     7399 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/hed_schema_io.py
--rw-rw-rw-   0        0        0     6118 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/hed_schema_section.py
--rw-rw-rw-   0        0        0     8019 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_compliance.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/schema/schema_data/
--rw-rw-rw-   0        0        0   316118 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_data/HED8.0.0.xml
--rw-rw-rw-   0        0        0   335759 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_data/HED8.1.0.xml
--rw-rw-rw-   0        0        0   350310 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_data/HED_score_1.0.0.xml
--rw-rw-rw-   0        0        0   316637 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_data/HED_testlib_1.0.2.xml
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/schema/schema_io/
--rw-rw-rw-   0        0        0        0 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/schema/schema_io/__init__.py
--rw-rw-rw-   0        0        0     7951 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/schema/schema_io/schema2wiki.py
--rw-rw-rw-   0        0        0     7337 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/schema/schema_io/schema2xml.py
--rw-rw-rw-   0        0        0     3710 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_io/schema_util.py
--rw-rw-rw-   0        0        0    22025 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_io/wiki2schema.py
--rw-rw-rw-   0        0        0      933 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/schema/schema_io/wiki_constants.py
--rw-rw-rw-   0        0        0    13700 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_io/xml2schema.py
--rw-rw-rw-   0        0        0     2452 2022-06-20 19:04:23.000000 hedtools-0.2.0/hed/schema/schema_io/xml_constants.py
--rw-rw-rw-   0        0        0     2600 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/schema/schema_validation_util.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/
--rw-rw-rw-   0        0        0     3055 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/analysis/
--rw-rw-rw-   0        0        0       29 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/__init__.py
--rw-rw-rw-   0        0        0     5912 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/analysis_util.py
--rw-rw-rw-   0        0        0    15621 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/annotation_util.py
--rw-rw-rw-   0        0        0     1608 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/column_name_summary.py
--rw-rw-rw-   0        0        0     5988 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/file_dictionary.py
--rw-rw-rw-   0        0        0     5420 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_context_manager.py
--rw-rw-rw-   0        0        0     4020 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_tag_counts.py
--rw-rw-rw-   0        0        0     6314 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_type_counts.py
--rw-rw-rw-   0        0        0     5558 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_type_definitions.py
--rw-rw-rw-   0        0        0     5368 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_type_factors.py
--rw-rw-rw-   0        0        0     5186 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_type_manager.py
--rw-rw-rw-   0        0        0    12334 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/hed_type_values.py
--rw-rw-rw-   0        0        0     9729 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/key_map.py
--rw-rw-rw-   0        0        0    10677 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/analysis/tabular_summary.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/bids/
--rw-rw-rw-   0        0        0       42 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/__init__.py
--rw-rw-rw-   0        0        0     5039 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_dataset.py
--rw-rw-rw-   0        0        0     3176 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_file.py
--rw-rw-rw-   0        0        0     9519 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_file_dictionary.py
--rw-rw-rw-   0        0        0     9479 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_file_group.py
--rw-rw-rw-   0        0        0     2960 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_sidecar_file.py
--rw-rw-rw-   0        0        0     8308 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_tabular_dictionary.py
--rw-rw-rw-   0        0        0     1433 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/bids/bids_tabular_file.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/remodeling/
--rw-rw-rw-   0        0        0       67 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/__init__.py
--rw-rw-rw-   0        0        0     9905 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/backup_manager.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/remodeling/cli/
--rw-rw-rw-   0        0        0       52 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/cli/__init__.py
--rw-rw-rw-   0        0        0     8095 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/cli/run_remodel.py
--rw-rw-rw-   0        0        0     3148 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/cli/run_remodel_backup.py
--rw-rw-rw-   0        0        0     1845 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/cli/run_remodel_restore.py
--rw-rw-rw-   0        0        0    10039 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/remodeling/operations/
--rw-rw-rw-   0        0        0       30 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/__init__.py
--rw-rw-rw-   0        0        0     8321 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/base_context.py
--rw-rw-rw-   0        0        0     3963 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/base_op.py
--rw-rw-rw-   0        0        0     3189 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/factor_column_op.py
--rw-rw-rw-   0        0        0     5093 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/factor_hed_tags_op.py
--rw-rw-rw-   0        0        0     3240 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/factor_hed_type_op.py
--rw-rw-rw-   0        0        0     6913 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/merge_consecutive_op.py
--rw-rw-rw-   0        0        0     4755 2023-02-14 21:37:40.000000 hedtools-0.2.0/hed/tools/remodeling/operations/number_groups_op.py
--rw-rw-rw-   0        0        0     3553 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/number_rows_op.py
--rw-rw-rw-   0        0        0     5628 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/remap_columns_op.py
--rw-rw-rw-   0        0        0     2470 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/remove_columns_op.py
--rw-rw-rw-   0        0        0     1973 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/remove_rows_op.py
--rw-rw-rw-   0        0        0     2456 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/rename_columns_op.py
--rw-rw-rw-   0        0        0     2851 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/reorder_columns_op.py
--rw-rw-rw-   0        0        0     5413 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/split_rows_op.py
--rw-rw-rw-   0        0        0     4132 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/summarize_column_names_op.py
--rw-rw-rw-   0        0        0     6252 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/summarize_column_values_op.py
--rw-rw-rw-   0        0        0     7229 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/summarize_hed_tags_op.py
--rw-rw-rw-   0        0        0     7803 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/summarize_hed_type_op.py
--rw-rw-rw-   0        0        0     9395 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/summarize_hed_validation_op.py
--rw-rw-rw-   0        0        0     4838 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
--rw-rw-rw-   0        0        0     2386 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/remodeling/operations/valid_operations.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/tools/util/
--rw-rw-rw-   0        0        0       44 2022-09-12 19:32:19.000000 hedtools-0.2.0/hed/tools/util/__init__.py
--rw-rw-rw-   0        0        0    11399 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/util/data_util.py
--rw-rw-rw-   0        0        0     1546 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/util/hed_logger.py
--rw-rw-rw-   0        0        0    12468 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/tools/util/io_util.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hed/validator/
--rw-rw-rw-   0        0        0      111 2022-02-04 21:37:41.000000 hedtools-0.2.0/hed/validator/__init__.py
--rw-rw-rw-   0        0        0     6710 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/validator/hed_validator.py
--rw-rw-rw-   0        0        0    27283 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/validator/tag_validator.py
--rw-rw-rw-   0        0        0     1849 2023-02-14 21:37:41.000000 hedtools-0.2.0/hed/validator/tag_validator_util.py
-drwxrwxrwx   0        0        0        0 2023-02-14 21:42:44.000000 hedtools-0.2.0/hedtools.egg-info/
--rw-rw-rw-   0        0        0     5504 2023-02-14 21:42:43.000000 hedtools-0.2.0/hedtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8460 2023-02-14 21:42:44.000000 hedtools-0.2.0/hedtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-14 21:42:43.000000 hedtools-0.2.0/hedtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      216 2023-02-14 21:42:43.000000 hedtools-0.2.0/hedtools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      121 2023-02-14 21:42:43.000000 hedtools-0.2.0/hedtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-02-14 21:42:43.000000 hedtools-0.2.0/hedtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      103 2022-06-20 19:04:23.000000 hedtools-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      196 2023-02-14 21:37:41.000000 hedtools-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0     1361 2023-02-14 21:42:44.000000 hedtools-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      199 2022-06-20 19:04:23.000000 hedtools-0.2.0/setup.py
--rw-rw-rw-   0        0        0    81180 2022-06-20 19:04:23.000000 hedtools-0.2.0/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/
+-rw-rw-rw-   0        0        0     1103 2023-06-20 20:23:24.000000 hedtools-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       70 2022-06-20 19:04:23.000000 hedtools-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5981 2023-06-20 20:41:22.000000 hedtools-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5337 2023-06-20 20:23:24.000000 hedtools-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/
+-rw-rw-rw-   0        0        0      773 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/__init__.py
+-rw-rw-rw-   0        0        0      518 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/_version.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/errors/
+-rw-rw-rw-   0        0        0      326 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/__init__.py
+-rw-rw-rw-   0        0        0    20119 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/error_messages.py
+-rw-rw-rw-   0        0        0    22248 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/error_reporter.py
+-rw-rw-rw-   0        0        0     5664 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/error_types.py
+-rw-rw-rw-   0        0        0     2079 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/errors/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/models/
+-rw-rw-rw-   0        0        0      711 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/__init__.py
+-rw-rw-rw-   0        0        0    19941 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/base_input.py
+-rw-rw-rw-   0        0        0    17951 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/column_mapper.py
+-rw-rw-rw-   0        0        0     5298 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/column_metadata.py
+-rw-rw-rw-   0        0        0     8455 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/def_expand_gather.py
+-rw-rw-rw-   0        0        0    13845 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/definition_dict.py
+-rw-rw-rw-   0        0        0     3044 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/definition_entry.py
+-rw-rw-rw-   0        0        0     6302 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/df_util.py
+-rw-rw-rw-   0        0        0    15583 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/expression_parser.py
+-rw-rw-rw-   0        0        0    18781 2023-06-20 20:23:24.000000 hedtools-0.3.0/hed/models/hed_group.py
+-rw-rw-rw-   0        0        0    14042 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/hed_string.py
+-rw-rw-rw-   0        0        0     4418 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/hed_string_group.py
+-rw-rw-rw-   0        0        0    20438 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/hed_tag.py
+-rw-rw-rw-   0        0        0      749 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/model_constants.py
+-rw-rw-rw-   0        0        0     9063 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/sidecar.py
+-rw-rw-rw-   0        0        0     2704 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/spreadsheet_input.py
+-rw-rw-rw-   0        0        0     2974 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/tabular_input.py
+-rw-rw-rw-   0        0        0      925 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/models/timeseries_input.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/schema/
+-rw-rw-rw-   0        0        0      563 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/__init__.py
+-rw-rw-rw-   0        0        0    19301 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_cache.py
+-rw-rw-rw-   0        0        0    30335 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema.py
+-rw-rw-rw-   0        0        0     2104 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_constants.py
+-rw-rw-rw-   0        0        0    10197 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_entry.py
+-rw-rw-rw-   0        0        0     6990 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_group.py
+-rw-rw-rw-   0        0        0     7202 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_io.py
+-rw-rw-rw-   0        0        0     8969 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/hed_schema_section.py
+-rw-rw-rw-   0        0        0     9013 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_compliance.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/schema/schema_data/
+-rw-rw-rw-   0        0        0   316118 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED8.0.0.xml
+-rw-rw-rw-   0        0        0   335759 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED8.1.0.xml
+-rw-rw-rw-   0        0        0   345995 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_data/HED8.2.0.xml
+-rw-rw-rw-   0        0        0   350310 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED_score_1.0.0.xml
+-rw-rw-rw-   0        0        0   316637 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/schema/schema_data/HED_testlib_1.0.2.xml
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/schema/schema_io/
+-rw-rw-rw-   0        0        0        0 2022-06-20 19:04:23.000000 hedtools-0.3.0/hed/schema/schema_io/__init__.py
+-rw-rw-rw-   0        0        0     5464 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema2base.py
+-rw-rw-rw-   0        0        0     5847 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema2wiki.py
+-rw-rw-rw-   0        0        0     5576 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema2xml.py
+-rw-rw-rw-   0        0        0     3692 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/schema_util.py
+-rw-rw-rw-   0        0        0    24745 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/wiki2schema.py
+-rw-rw-rw-   0        0        0      945 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/wiki_constants.py
+-rw-rw-rw-   0        0        0    14077 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/xml2schema.py
+-rw-rw-rw-   0        0        0     2507 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_io/xml_constants.py
+-rw-rw-rw-   0        0        0     6221 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/schema/schema_validation_util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/
+-rw-rw-rw-   0        0        0     3090 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/analysis/
+-rw-rw-rw-   0        0        0       29 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/__init__.py
+-rw-rw-rw-   0        0        0     9402 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/analysis_util.py
+-rw-rw-rw-   0        0        0    15621 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/annotation_util.py
+-rw-rw-rw-   0        0        0     5505 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/event_manager.py
+-rw-rw-rw-   0        0        0     5988 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/file_dictionary.py
+-rw-rw-rw-   0        0        0     5796 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_context_manager.py
+-rw-rw-rw-   0        0        0     4987 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_tag_counts.py
+-rw-rw-rw-   0        0        0     6314 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_counts.py
+-rw-rw-rw-   0        0        0     5573 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_definitions.py
+-rw-rw-rw-   0        0        0     5368 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_factors.py
+-rw-rw-rw-   0        0        0     5189 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_manager.py
+-rw-rw-rw-   0        0        0    12301 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/hed_type_values.py
+-rw-rw-rw-   0        0        0     9733 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/key_map.py
+-rw-rw-rw-   0        0        0     1615 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/tabular_column_name_summary.py
+-rw-rw-rw-   0        0        0    10722 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/tabular_summary.py
+-rw-rw-rw-   0        0        0     1077 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/analysis/temporal_event.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/bids/
+-rw-rw-rw-   0        0        0       42 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/__init__.py
+-rw-rw-rw-   0        0        0     4726 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_dataset.py
+-rw-rw-rw-   0        0        0     3176 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/bids_file.py
+-rw-rw-rw-   0        0        0     9525 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_file_dictionary.py
+-rw-rw-rw-   0        0        0     9280 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_file_group.py
+-rw-rw-rw-   0        0        0     2960 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/bids_sidecar_file.py
+-rw-rw-rw-   0        0        0     8310 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/bids/bids_tabular_dictionary.py
+-rw-rw-rw-   0        0        0     1433 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/bids/bids_tabular_file.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/remodeling/
+-rw-rw-rw-   0        0        0       67 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/remodeling/__init__.py
+-rw-rw-rw-   0        0        0    10544 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/backup_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/remodeling/cli/
+-rw-rw-rw-   0        0        0       52 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/remodeling/cli/__init__.py
+-rw-rw-rw-   0        0        0     9165 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel.py
+-rw-rw-rw-   0        0        0     3738 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_backup.py
+-rw-rw-rw-   0        0        0     2188 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_restore.py
+-rw-rw-rw-   0        0        0    10276 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/remodeling/operations/
+-rw-rw-rw-   0        0        0       30 2023-02-14 21:37:40.000000 hedtools-0.3.0/hed/tools/remodeling/operations/__init__.py
+-rw-rw-rw-   0        0        0     3891 2023-06-20 20:23:25.000000 hedtools-0.3.0/hed/tools/remodeling/operations/base_op.py
+-rw-rw-rw-   0        0        0    10985 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/base_summary.py
+-rw-rw-rw-   0        0        0     2437 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/convert_columns_op.py
+-rw-rw-rw-   0        0        0     3143 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/factor_column_op.py
+-rw-rw-rw-   0        0        0     4145 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_tags_op.py
+-rw-rw-rw-   0        0        0     3307 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_type_op.py
+-rw-rw-rw-   0        0        0     6750 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/merge_consecutive_op.py
+-rw-rw-rw-   0        0        0     4716 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/number_groups_op.py
+-rw-rw-rw-   0        0        0     3568 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/number_rows_op.py
+-rw-rw-rw-   0        0        0     5552 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/remap_columns_op.py
+-rw-rw-rw-   0        0        0     2472 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/remove_columns_op.py
+-rw-rw-rw-   0        0        0     1988 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/remove_rows_op.py
+-rw-rw-rw-   0        0        0     2428 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/rename_columns_op.py
+-rw-rw-rw-   0        0        0     2847 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/reorder_columns_op.py
+-rw-rw-rw-   0        0        0     5360 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/split_rows_op.py
+-rw-rw-rw-   0        0        0     6092 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_column_names_op.py
+-rw-rw-rw-   0        0        0    11856 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_column_values_op.py
+-rw-rw-rw-   0        0        0     8064 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_definitions_op.py
+-rw-rw-rw-   0        0        0     9588 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_tags_op.py
+-rw-rw-rw-   0        0        0     9956 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_type_op.py
+-rw-rw-rw-   0        0        0    10230 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_validation_op.py
+-rw-rw-rw-   0        0        0     7408 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
+-rw-rw-rw-   0        0        0     2660 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/remodeling/operations/valid_operations.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/tools/util/
+-rw-rw-rw-   0        0        0       44 2022-09-12 19:32:19.000000 hedtools-0.3.0/hed/tools/util/__init__.py
+-rw-rw-rw-   0        0        0    11413 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/util/data_util.py
+-rw-rw-rw-   0        0        0     1546 2023-02-14 21:37:41.000000 hedtools-0.3.0/hed/tools/util/hed_logger.py
+-rw-rw-rw-   0        0        0    11590 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/util/io_util.py
+-rw-rw-rw-   0        0        0     1266 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/tools/util/schema_util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hed/validator/
+-rw-rw-rw-   0        0        0      298 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/__init__.py
+-rw-rw-rw-   0        0        0     5053 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/def_validator.py
+-rw-rw-rw-   0        0        0     8849 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/hed_validator.py
+-rw-rw-rw-   0        0        0     4563 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/onset_validator.py
+-rw-rw-rw-   0        0        0    13152 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/sidecar_validator.py
+-rw-rw-rw-   0        0        0     5618 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/spreadsheet_validator.py
+-rw-rw-rw-   0        0        0    30296 2023-06-20 20:23:26.000000 hedtools-0.3.0/hed/validator/tag_validator.py
+-rw-rw-rw-   0        0        0     1849 2023-02-14 21:37:41.000000 hedtools-0.3.0/hed/validator/tag_validator_util.py
+drwxrwxrwx   0        0        0        0 2023-06-20 20:41:22.000000 hedtools-0.3.0/hedtools.egg-info/
+-rw-rw-rw-   0        0        0     5981 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9254 2023-06-20 20:41:22.000000 hedtools-0.3.0/hedtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      216 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      112 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 20:41:21.000000 hedtools-0.3.0/hedtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      103 2022-06-20 19:04:23.000000 hedtools-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0      121 2023-06-20 20:23:26.000000 hedtools-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0     1350 2023-06-20 20:41:22.000000 hedtools-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0      199 2022-06-20 19:04:23.000000 hedtools-0.3.0/setup.py
+-rw-rw-rw-   0        0        0    81180 2022-06-20 19:04:23.000000 hedtools-0.3.0/versioneer.py
```

### Comparing `hedtools-0.2.0/LICENSE` & `hedtools-0.3.0/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2020 HED Standard Working Group
+Copyright (c) 2020+ HED Standard Working Group
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `hedtools-0.2.0/PKG-INFO` & `hedtools-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 Metadata-Version: 2.1
 Name: hedtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: HED validation, summary, and analysis tools.
 Home-page: https://github.com/hed-standard/hed-python/
 Author: VisLab, Ian Callanan, Jeremy Cockfield, Alexander Jones, Owen Winterberg, Kay Robbins
 Author-email: Kay.Robbins@utsa.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8056010.svg)](https://doi.org/10.5281/zenodo.8056010)
+[![Maintainability](https://api.codeclimate.com/v1/badges/11bf2329590e7b0164ba/maintainability)](https://codeclimate.com/github/hed-standard/hed-python/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/11bf2329590e7b0164ba/test_coverage)](https://codeclimate.com/github/hed-standard/hed-python/test_coverage)
+![PyPI - Status](https://img.shields.io/pypi/v/hedtools)
+
+
 # HEDTools - Python
 HED (Hierarchical Event Descriptors) is a framework for systematically describing
 both laboratory and real-world events as well as other experimental metadata.
 HED tags are comma-separated path strings.
 HED, itself, is platform-independent, extendable, and data-neutral. 
 
 This repository contains the underlying python tools that support validation,
 summarization, and analysis of datasets using HED tags.
 
 Most people will simply annotate their events by creating a spreadsheet
 or a BIDS JSON sidecar that associates HED tags with event codes or the events themselves.
 If you have such a spreadsheet or a JSON, 
 you can use the HED Online Validator currently available at 
-[https://hedtools.ucsd.edu/hed](https://hedtools.ucsd.edu/hed) to validate or transform
+[https://hedtools.org](https://hedtools.org) to validate or transform
 your files without downloading any tools. 
 
 A version of the online tools corresponding to the `develop` branch can be found at:
-[https://hedtools.ucsd.edu/hed_dev](https://hedtools.ucsd.edu/hed_dev).
+[https://hedtools.org/hed_dev](https://hedtools.org/hed_dev).
 
 ### Installation
 Use `pip` to install `hedtools` from PyPI:
 
    ```
        pip install hedtools
    ```
@@ -105,12 +111,12 @@
 Cached Schemas by default are stored in "home/.hedtools/" 
 Location of "home" directory varies by OS.
 
 Use `hed.schema.set_cache_directory` to change the location.
 The HED cache can be shared across processes.
 
 Starting with `hedtools 0.2.0` local copies of the most recent schema versions
-are stored within the code modules for easy access.
+are stored within the code modules for easy access.  
 
 ### Other links of interest
 
 Code climate reports: [https://codeclimate.com/github/hed-standard/hed-python](https://codeclimate.com/github/hed-standard/hed-python).
```

### Comparing `hedtools-0.2.0/README.md` & `hedtools-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,31 @@
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8056010.svg)](https://doi.org/10.5281/zenodo.8056010)
+[![Maintainability](https://api.codeclimate.com/v1/badges/11bf2329590e7b0164ba/maintainability)](https://codeclimate.com/github/hed-standard/hed-python/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/11bf2329590e7b0164ba/test_coverage)](https://codeclimate.com/github/hed-standard/hed-python/test_coverage)
+![PyPI - Status](https://img.shields.io/pypi/v/hedtools)
+
+
 # HEDTools - Python
 HED (Hierarchical Event Descriptors) is a framework for systematically describing
 both laboratory and real-world events as well as other experimental metadata.
 HED tags are comma-separated path strings.
 HED, itself, is platform-independent, extendable, and data-neutral. 
 
 This repository contains the underlying python tools that support validation,
 summarization, and analysis of datasets using HED tags.
 
 Most people will simply annotate their events by creating a spreadsheet
 or a BIDS JSON sidecar that associates HED tags with event codes or the events themselves.
 If you have such a spreadsheet or a JSON, 
 you can use the HED Online Validator currently available at 
-[https://hedtools.ucsd.edu/hed](https://hedtools.ucsd.edu/hed) to validate or transform
+[https://hedtools.org](https://hedtools.org) to validate or transform
 your files without downloading any tools. 
 
 A version of the online tools corresponding to the `develop` branch can be found at:
-[https://hedtools.ucsd.edu/hed_dev](https://hedtools.ucsd.edu/hed_dev).
+[https://hedtools.org/hed_dev](https://hedtools.org/hed_dev).
 
 ### Installation
 Use `pip` to install `hedtools` from PyPI:
 
    ```
        pip install hedtools
    ```
@@ -91,12 +97,12 @@
 Cached Schemas by default are stored in "home/.hedtools/" 
 Location of "home" directory varies by OS.
 
 Use `hed.schema.set_cache_directory` to change the location.
 The HED cache can be shared across processes.
 
 Starting with `hedtools 0.2.0` local copies of the most recent schema versions
-are stored within the code modules for easy access.
+are stored within the code modules for easy access.  
 
 ### Other links of interest
 
 Code climate reports: [https://codeclimate.com/github/hed-standard/hed-python](https://codeclimate.com/github/hed-standard/hed-python).
```

### Comparing `hedtools-0.2.0/hed/errors/error_messages.py` & `hedtools-0.3.0/hed/errors/error_messages.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,337 +2,447 @@
 This module contains the actual formatted error messages for each type.
 
 Add new errors here, or any other file imported after error_reporter.py.
 """
 
 from hed.errors.error_reporter import hed_error, hed_tag_error
 from hed.errors.error_types import ValidationErrors, SchemaErrors, \
-    SidecarErrors, SchemaWarnings, ErrorSeverity, DefinitionErrors, OnsetErrors
+    SidecarErrors, SchemaWarnings, ErrorSeverity, DefinitionErrors, OnsetErrors, ColumnErrors
 
 
-@hed_tag_error(ValidationErrors.HED_UNITS_INVALID)
-def val_error_invalid_unit(tag, unit_class_units):
-    units_string = ','.join(sorted(unit_class_units))
-    return f'Invalid unit - "{tag}" valid units are "{units_string}"', {
-        "unit_class_units": sorted(unit_class_units)
-    }
+@hed_tag_error(ValidationErrors.UNITS_INVALID)
+def val_error_invalid_unit(tag, units):
+    units_string = ','.join(sorted(units))
+    return f'Invalid unit - "{tag}" valid units are "{units_string}"'
 
 
-@hed_error(ValidationErrors.HED_TAG_EMPTY)
+@hed_error(ValidationErrors.TAG_EMPTY)
 def val_error_extra_comma(source_string, char_index):
     character = source_string[char_index]
-    return f"HED tags cannot be empty.  Extra delimiter found: '{character}' at index {char_index}'", {
-               'char_index': char_index
-           }
+    return f"HED tags cannot be empty.  Extra delimiter found: '{character}' at index {char_index}'"
 
 
-@hed_tag_error(ValidationErrors.HED_GROUP_EMPTY, actual_code=ValidationErrors.HED_TAG_EMPTY)
+@hed_tag_error(ValidationErrors.HED_GROUP_EMPTY, actual_code=ValidationErrors.TAG_EMPTY)
 def val_error_empty_group(tag):
-    return f"HED tags cannot be empty.  Extra delimiters found: '{tag}'", {}
+    return f"HED tags cannot be empty.  Extra delimiters found: '{tag}'"
 
 
-@hed_tag_error(ValidationErrors.HED_TAG_EXTENDED, has_sub_tag=True, default_severity=ErrorSeverity.WARNING)
+@hed_tag_error(ValidationErrors.TAG_EXTENDED, has_sub_tag=True, default_severity=ErrorSeverity.WARNING)
 def val_error_tag_extended(tag, problem_tag):
-    return f"Hed tag is extended. '{problem_tag}' in {tag}", {}
+    return f"Hed tag is extended. '{problem_tag}' in {tag}"
 
 
-@hed_error(ValidationErrors.HED_CHARACTER_INVALID)
+@hed_error(ValidationErrors.CHARACTER_INVALID)
 def val_error_invalid_char(source_string, char_index):
     character = source_string[char_index]
-    return f'Invalid character "{character}" at index {char_index}"', {
-               'char_index': char_index
-           }
+    return f'Invalid character "{character}" at index {char_index}"'
 
 
 @hed_tag_error(ValidationErrors.INVALID_TAG_CHARACTER, has_sub_tag=True,
-               actual_code=ValidationErrors.HED_CHARACTER_INVALID)
+               actual_code=ValidationErrors.CHARACTER_INVALID)
 def val_error_invalid_tag_character(tag, problem_tag):
-    return f"Invalid character '{problem_tag}' in {tag}", {}
+    return f"Invalid character '{problem_tag}' in {tag}"
 
 
-@hed_error(ValidationErrors.HED_TILDES_UNSUPPORTED)
+@hed_error(ValidationErrors.TILDES_UNSUPPORTED)
 def val_error_tildes_not_supported(source_string, char_index):
     character = source_string[char_index]
-    return f"Tildes not supported.  Replace (a ~ b ~ c) with (a, (b, c)).  '{character}' at index {char_index}'", {
-               'char_index': char_index
-           }
+    return f"Tildes not supported.  Replace (a ~ b ~ c) with (a, (b, c)).  '{character}' at index {char_index}'"
 
 
-@hed_error(ValidationErrors.HED_COMMA_MISSING)
+@hed_error(ValidationErrors.COMMA_MISSING)
 def val_error_comma_missing(tag):
-    return f"Comma missing after - '{tag}'", {}
+    return f"Comma missing after - '{tag}'"
 
 
-@hed_tag_error(ValidationErrors.HED_TAG_REPEATED)
+@hed_tag_error(ValidationErrors.HED_TAG_REPEATED, actual_code=ValidationErrors.TAG_EXPRESSION_REPEATED)
 def val_error_duplicate_tag(tag):
-    return f'Repeated tag - "{tag}"', {}
+    return f'Repeated tag - "{tag}"'
 
 
-@hed_error(ValidationErrors.HED_TAG_REPEATED_GROUP)
+@hed_error(ValidationErrors.HED_TAG_REPEATED_GROUP, actual_code=ValidationErrors.TAG_EXPRESSION_REPEATED)
 def val_error_duplicate_group(group):
-    return f'Repeated group - "{group}"', {}
+    return f'Repeated group - "{group}"'
 
 
-@hed_error(ValidationErrors.HED_PARENTHESES_MISMATCH)
+@hed_error(ValidationErrors.PARENTHESES_MISMATCH)
 def val_error_parentheses(opening_parentheses_count, closing_parentheses_count):
     return f'Number of opening and closing parentheses are unequal. '\
            f'{opening_parentheses_count} opening parentheses. {closing_parentheses_count} '\
-           'closing parentheses', {}
+           'closing parentheses'
 
 
-@hed_tag_error(ValidationErrors.HED_TAG_REQUIRES_CHILD)
+@hed_tag_error(ValidationErrors.TAG_REQUIRES_CHILD)
 def val_error_require_child(tag):
-    return f"Descendant tag required - '{tag}'", {}
+    return f"Descendant tag required - '{tag}'"
 
 
-@hed_error(ValidationErrors.HED_TAG_NOT_UNIQUE)
-def val_error_multiple_unique(tag_prefix):
-    return f"Multiple unique tags with prefix - '{tag_prefix}'", {}
+@hed_error(ValidationErrors.TAG_NOT_UNIQUE)
+def val_error_multiple_unique(tag_namespace):
+    return f"Multiple unique tags with namespace - '{tag_namespace}'"
 
 
-@hed_tag_error(ValidationErrors.INVALID_EXTENSION, actual_code=ValidationErrors.HED_TAG_INVALID)
+@hed_tag_error(ValidationErrors.TAG_NAMESPACE_PREFIX_INVALID)
+def val_error_prefix_invalid(tag, tag_namespace):
+    return f"Prefixes can only contain alpha characters. - '{tag_namespace}'"
+
+
+@hed_tag_error(ValidationErrors.TAG_EXTENSION_INVALID)
 def val_error_invalid_extension(tag):
-    return f'Invalid extension on tag - "{tag}"', {}
+    return f'Invalid extension on tag - "{tag}"'
 
 
-@hed_tag_error(ValidationErrors.INVALID_PARENT_NODE, has_sub_tag=True, actual_code=ValidationErrors.HED_TAG_INVALID)
+@hed_tag_error(ValidationErrors.INVALID_PARENT_NODE, has_sub_tag=True, actual_code=ValidationErrors.TAG_EXTENSION_INVALID)
 def val_error_invalid_parent(tag, problem_tag, expected_parent_tag):
-    return f"In '{tag}', '{problem_tag}' appears as '{str(expected_parent_tag)}' and cannot be used " \
-           f"as an extension.", {"expected_parent_tag": expected_parent_tag}
+    return f"In '{tag}', '{problem_tag}' appears as '{str(expected_parent_tag)}' and cannot be used as an extension."
 
 
-@hed_tag_error(ValidationErrors.NO_VALID_TAG_FOUND, has_sub_tag=True, actual_code=ValidationErrors.HED_TAG_INVALID)
+@hed_tag_error(ValidationErrors.NO_VALID_TAG_FOUND, has_sub_tag=True, actual_code=ValidationErrors.TAG_INVALID)
 def val_error_no_valid_tag(tag, problem_tag):
-    return f"'{problem_tag}' in {tag} is not a valid base hed tag.", {}
+    return f"'{problem_tag}' in {tag} is not a valid base hed tag."
 
 
-@hed_tag_error(ValidationErrors.HED_VALUE_INVALID)
+@hed_tag_error(ValidationErrors.VALUE_INVALID)
 def val_error_no_value(tag):
-    return f"''{tag}' has an invalid value portion.", {}
+    return f"'{tag}' has an invalid value portion."
 
 
 @hed_error(ValidationErrors.HED_MISSING_REQUIRED_COLUMN, default_severity=ErrorSeverity.WARNING)
-def val_error_missing_column(column_name):
-    return f"Required column '{column_name}' not specified or found in file.", {}
+def val_error_missing_column(column_name, column_type):
+    return f"Required {column_type} column '{column_name}' not specified or found in file."
 
 
 @hed_error(ValidationErrors.HED_UNKNOWN_COLUMN, default_severity=ErrorSeverity.WARNING)
 def val_error_extra_column(column_name):
     return f"Column named '{column_name}' found in file, but not specified as a tag column " + \
-        "or identified in sidecars.", {}
+        "or identified in sidecars."
 
 
-@hed_error(ValidationErrors.HED_BLANK_COLUMN, default_severity=ErrorSeverity.WARNING)
-def val_error_hed_blank_column(column_number):
-    return f"Column number {column_number} has no column name", {}
+@hed_error(ValidationErrors.SIDECAR_AND_OTHER_COLUMNS)
+def val_error_sidecar_with_column(column_names):
+    return f"You cannot use a sidecar and tag or prefix columns at the same time. " \
+            f"Found {column_names}."
+
+
+@hed_error(ValidationErrors.DUPLICATE_COLUMN_IN_LIST)
+def val_error_duplicate_clumn(column_number, column_name, list_name):
+    if column_name:
+        return f"Found column '{column_name}' at index {column_number} twice in {list_name}."
+    else:
+        return f"Found column number {column_number} twice in {list_name}.  This isn't a major concern, but does indicate a mistake."
+
+
+@hed_error(ValidationErrors.DUPLICATE_COLUMN_BETWEEN_SOURCES)
+def val_error_duplicate_clumn(column_number, column_name, list_names):
+    if column_name:
+        return f"Found column '{column_name}' at index {column_number} in the following inputs: {list_names}. " \
+               f"Each entry must be unique."
+    else:
+        return f"Found column number {column_number} in the following inputs: {list_names}. " \
+               f"Each entry must be unique."
 
 
-@hed_error(ValidationErrors.HED_DUPLICATE_COLUMN, default_severity=ErrorSeverity.WARNING)
-def val_error_hed_duplicate_column(column_name):
-    return f"Multiple columns have name {column_name}.  This is not a fatal error, but discouraged.", {}
+@hed_error(ValidationErrors.HED_BLANK_COLUMN, default_severity=ErrorSeverity.WARNING)
+def val_error_hed_blank_column(column_number):
+    return f"Column number {column_number} has no column name"
 
 
-@hed_tag_error(ValidationErrors.HED_LIBRARY_UNMATCHED)
-def val_error_unknown_prefix(tag, unknown_prefix, known_prefixes):
-    return f"Tag '{tag} has unknown prefix '{unknown_prefix}'.  Valid prefixes: {known_prefixes}", {}
+@hed_tag_error(ValidationErrors.HED_LIBRARY_UNMATCHED, actual_code=ValidationErrors.TAG_NAMESPACE_PREFIX_INVALID)
+def val_error_unknown_namespace(tag, unknown_prefix, known_prefixes):
+    return f"Tag '{tag} has unknown namespace '{unknown_prefix}'.  Valid prefixes: {known_prefixes}"
 
 
-@hed_tag_error(ValidationErrors.HED_NODE_NAME_EMPTY, has_sub_tag=True)
+@hed_tag_error(ValidationErrors.NODE_NAME_EMPTY, has_sub_tag=True)
 def val_error_extra_slashes_spaces(tag, problem_tag):
-    return f"Extra slashes or spaces '{problem_tag}' in tag '{tag}'", {}
+    return f"Extra slashes or spaces '{problem_tag}' in tag '{tag}'"
 
 
-@hed_error(ValidationErrors.HED_SIDECAR_KEY_MISSING, default_severity=ErrorSeverity.WARNING)
+@hed_error(ValidationErrors.SIDECAR_KEY_MISSING, default_severity=ErrorSeverity.WARNING)
 def val_error_sidecar_key_missing(invalid_key, category_keys):
-    return f"Category key '{invalid_key}' does not exist in column.  Valid keys are: {category_keys}", {}
+    return f"Category key '{invalid_key}' does not exist in column.  Valid keys are: {category_keys}"
 
 
-@hed_tag_error(ValidationErrors.HED_DEF_UNMATCHED)
-def val_error_def_unmatched(tag):
-    return f"A data-recording’s Def tag cannot be matched to definition.  Tag: '{tag}'", {}
 
 
-@hed_tag_error(ValidationErrors.HED_DEF_EXPAND_INVALID)
+@hed_tag_error(ValidationErrors.HED_DEF_EXPAND_INVALID, actual_code=ValidationErrors.DEF_EXPAND_INVALID)
 def val_error_bad_def_expand(tag, actual_def, found_def):
     return f"A data-recording’s Def-expand tag does not match the given definition." + \
-           f"Tag: '{tag}'.  Actual Def: {actual_def}.  Found Def: {found_def}", {}
+           f"Tag: '{tag}'.  Actual Def: {actual_def}.  Found Def: {found_def}"
 
 
-@hed_tag_error(ValidationErrors.HED_DEF_VALUE_MISSING, actual_code=ValidationErrors.HED_DEF_VALUE_INVALID)
+@hed_tag_error(ValidationErrors.HED_DEF_UNMATCHED, actual_code=ValidationErrors.DEF_INVALID)
+def val_error_def_unmatched(tag):
+    return f"A data-recording’s Def tag cannot be matched to definition.  Tag: '{tag}'"
+
+
+@hed_tag_error(ValidationErrors.HED_DEF_VALUE_MISSING, actual_code=ValidationErrors.DEF_INVALID)
 def val_error_def_value_missing(tag):
-    return f"A def tag requires a placeholder value, but was not given one.  Definition: '{tag}'", {}
+    return f"A def tag requires a placeholder value, but was not given one.  Definition: '{tag}'"
 
 
-@hed_tag_error(ValidationErrors.HED_DEF_VALUE_EXTRA, actual_code=ValidationErrors.HED_DEF_VALUE_INVALID)
+@hed_tag_error(ValidationErrors.HED_DEF_VALUE_EXTRA, actual_code=ValidationErrors.DEF_INVALID)
 def val_error_def_value_extra(tag):
-    return f"A def tag does not take a placeholder value, but was given one.  Definition: '{tag}", {}
+    return f"A def tag does not take a placeholder value, but was given one.  Definition: '{tag}"
+
+
+@hed_tag_error(ValidationErrors.HED_DEF_EXPAND_UNMATCHED, actual_code=ValidationErrors.DEF_EXPAND_INVALID)
+def val_error_def_expand_unmatched(tag):
+    return f"A data-recording’s Def-expand tag cannot be matched to definition.  Tag: '{tag}'"
+
 
+@hed_tag_error(ValidationErrors.HED_DEF_EXPAND_VALUE_MISSING, actual_code=ValidationErrors.DEF_EXPAND_INVALID)
+def val_error_def_expand_value_missing(tag):
+    return f"A Def-expand tag requires a placeholder value, but was not given one.  Definition: '{tag}'"
 
-@hed_tag_error(ValidationErrors.HED_TOP_LEVEL_TAG, actual_code=ValidationErrors.HED_TAG_GROUP_ERROR)
+
+@hed_tag_error(ValidationErrors.HED_DEF_EXPAND_VALUE_EXTRA, actual_code=ValidationErrors.DEF_EXPAND_INVALID)
+def val_error_def_expand_value_extra(tag):
+    return f"A Def-expand tag does not take a placeholder value, but was given one.  Definition: '{tag}"
+
+
+@hed_tag_error(ValidationErrors.HED_TOP_LEVEL_TAG, actual_code=ValidationErrors.TAG_GROUP_ERROR)
 def val_error_top_level_tag(tag):
-    return f"A tag that must be in a top level group was found in another location.  {str(tag)}", {}
+    return f"A tag that must be in a top level group was found in another location.  {str(tag)}"
 
 
-@hed_tag_error(ValidationErrors.HED_TAG_GROUP_TAG, actual_code=ValidationErrors.HED_TAG_GROUP_ERROR)
+@hed_tag_error(ValidationErrors.HED_TAG_GROUP_TAG, actual_code=ValidationErrors.TAG_GROUP_ERROR)
 def val_error_tag_group_tag(tag):
-    return f"A tag that must be in a group was found in another location.  {str(tag)}", {}
+    return f"A tag that must be in a group was found in another location.  {str(tag)}"
 
 
-@hed_tag_error(ValidationErrors.HED_MULTIPLE_TOP_TAGS, actual_code=ValidationErrors.HED_TAG_GROUP_ERROR)
+@hed_tag_error(ValidationErrors.HED_MULTIPLE_TOP_TAGS, actual_code=ValidationErrors.TAG_GROUP_ERROR)
 def val_error_top_level_tags(tag, multiple_tags):
     tags_as_string = [str(tag) for tag in multiple_tags]
     return f"Multiple top level tags found in a single group.  First one found: {str(tag)}. " + \
-           f"Remainder:{str(tags_as_string)}", {}
+           f"Remainder:{str(tags_as_string)}"
 
 
-@hed_error(ValidationErrors.HED_REQUIRED_TAG_MISSING)
-def val_warning_required_prefix_missing(tag_prefix):
-    return f"Tag with prefix '{tag_prefix}' is required", {}
+@hed_error(ValidationErrors.REQUIRED_TAG_MISSING)
+def val_warning_required_prefix_missing(tag_namespace):
+    return f"Tag with namespace '{tag_namespace}' is required"
 
 
-@hed_tag_error(ValidationErrors.HED_STYLE_WARNING, default_severity=ErrorSeverity.WARNING)
+@hed_tag_error(ValidationErrors.STYLE_WARNING, default_severity=ErrorSeverity.WARNING)
 def val_warning_capitalization(tag):
-    return f"First word not capitalized or camel case - '{tag}'", {}
+    return f"First word not capitalized or camel case - '{tag}'"
 
 
-@hed_tag_error(ValidationErrors.HED_UNITS_DEFAULT_USED, default_severity=ErrorSeverity.WARNING)
+@hed_tag_error(ValidationErrors.UNITS_MISSING, default_severity=ErrorSeverity.WARNING)
 def val_warning_default_units_used(tag, default_unit):
-    return f"No unit specified. Using '{default_unit}' as the default - '{tag}'", {}
+    return f"No unit specified. Using '{default_unit}' as the default - '{tag}'"
 
 
 @hed_error(SchemaErrors.HED_SCHEMA_DUPLICATE_NODE)
 def schema_error_hed_duplicate_node(tag, duplicate_tag_list, section):
     tag_join_delimiter = "\n\t"
-    return f"Duplicate term '{str(tag)}' used {len(duplicate_tag_list)} places in '{section}' section schema as: " + \
-           f"{tag_join_delimiter} {tag_join_delimiter.join(duplicate_tag_list)}", {}
+    return f"Duplicate term '{str(tag)}' used {len(duplicate_tag_list)} places in '{section}' section schema as:" + \
+           f"{tag_join_delimiter}{tag_join_delimiter.join(duplicate_tag_list)}"
+
+
+@hed_error(SchemaErrors.HED_SCHEMA_DUPLICATE_FROM_LIBRARY)
+def schema_error_hed_duplicate_node(tag, duplicate_tag_list, section):
+    tag_join_delimiter = "\n\t"
+    return f"Duplicate term '{str(tag)}' was found in the library and in the standard schema in '{section}' section schema as:" + \
+           f"{tag_join_delimiter}{tag_join_delimiter.join(duplicate_tag_list)}"
 
 
-@hed_error(SchemaErrors.HED_SCHEMA_ATTRIBUTE_INVALID)
+@hed_error(SchemaErrors.SCHEMA_ATTRIBUTE_INVALID)
 def schema_error_unknown_attribute(attribute_name, source_tag):
     return f"Attribute '{attribute_name}' used by '{source_tag}' was not defined in the schema, " \
-           f"or was used outside of it's defined class.", {}
+           f"or was used outside of it's defined class."
 
 
 @hed_error(SchemaWarnings.INVALID_CHARACTERS_IN_DESC, default_severity=ErrorSeverity.WARNING,
            actual_code=SchemaWarnings.HED_SCHEMA_CHARACTER_INVALID)
 def schema_warning_invalid_chars_desc(desc_string, tag_name, problem_char, char_index):
-    return f"Invalid character '{problem_char}' in desc for '{tag_name}' at position {char_index}.  '{desc_string}", {}
+    return f"Invalid character '{problem_char}' in desc for '{tag_name}' at position {char_index}.  '{desc_string}"
 
 
 @hed_error(SchemaWarnings.INVALID_CHARACTERS_IN_TAG, default_severity=ErrorSeverity.WARNING,
            actual_code=SchemaWarnings.HED_SCHEMA_CHARACTER_INVALID)
 def schema_warning_invalid_chars_tag(tag_name, problem_char, char_index):
-    return f"Invalid character '{problem_char}' in tag '{tag_name}' at position {char_index}.", {}
+    return f"Invalid character '{problem_char}' in tag '{tag_name}' at position {char_index}."
 
 
 @hed_error(SchemaWarnings.INVALID_CAPITALIZATION, default_severity=ErrorSeverity.WARNING)
 def schema_warning_invalid_capitalization(tag_name, problem_char, char_index):
     return "First character must be a capital letter or number.  " + \
-           f"Found character '{problem_char}' in tag '{tag_name}' at position {char_index}.", \
-           {'problem_char': problem_char}
+           f"Found character '{problem_char}' in tag '{tag_name}' at position {char_index}."
 
 
 @hed_error(SchemaWarnings.NON_PLACEHOLDER_HAS_CLASS, default_severity=ErrorSeverity.WARNING)
 def schema_warning_non_placeholder_class(tag_name, invalid_attribute_name):
     return "Only placeholder nodes('#') can have a unit or value class." + \
-           f"Found {invalid_attribute_name} on {tag_name}", {}
+           f"Found {invalid_attribute_name} on {tag_name}"
+
+
+@hed_error(SchemaWarnings.INVALID_ATTRIBUTE, default_severity=ErrorSeverity.ERROR)
+def schema_error_invalid_attribute(tag_name, invalid_attribute_name):
+    return f"'{invalid_attribute_name}' should not be present in a loaded schema, found on '{tag_name}'." \
+           f"Something went very wrong."
+
 
 
 @hed_error(SidecarErrors.BLANK_HED_STRING)
 def sidecar_error_blank_hed_string():
-    return "No HED string found for Value or Category column.", {}
+    return "No HED string found for Value or Category column."
 
 
 @hed_error(SidecarErrors.WRONG_HED_DATA_TYPE)
 def sidecar_error_hed_data_type(expected_type, given_type):
-    return f"Invalid HED string datatype sidecar. Should be '{expected_type}', but got '{given_type}'", {}
+    return f"Invalid HED string datatype sidecar. Should be '{expected_type}', but got '{given_type}'"
 
 
-@hed_error(SidecarErrors.INVALID_POUND_SIGNS_VALUE, actual_code=ValidationErrors.HED_PLACEHOLDER_INVALID)
+@hed_error(SidecarErrors.INVALID_POUND_SIGNS_VALUE, actual_code=ValidationErrors.PLACEHOLDER_INVALID)
 def sidecar_error_invalid_pound_sign_count(pound_sign_count):
-    return f"There should be exactly one # character in a sidecar string. Found {pound_sign_count}", {}
+    return f"There should be exactly one # character in a sidecar string. Found {pound_sign_count}"
 
 
-@hed_error(SidecarErrors.INVALID_POUND_SIGNS_CATEGORY, actual_code=ValidationErrors.HED_PLACEHOLDER_INVALID)
+@hed_error(SidecarErrors.INVALID_POUND_SIGNS_CATEGORY, actual_code=ValidationErrors.PLACEHOLDER_INVALID)
 def sidecar_error_too_many_pound_signs(pound_sign_count):
-    return f"There should be no # characters in a category sidecar string. Found {pound_sign_count}", {}
+    return f"There should be no # characters in a category sidecar string. Found {pound_sign_count}"
 
 
 @hed_error(SidecarErrors.UNKNOWN_COLUMN_TYPE)
 def sidecar_error_unknown_column(column_name):
     return f"Could not automatically identify column '{column_name}' type from file. "\
-           "Most likely the column definition in question needs a # sign to replace a number somewhere.", {}
+           "Most likely the column definition in question needs a # sign to replace a number somewhere."
+
+
+@hed_error(SidecarErrors.SIDECAR_HED_USED, actual_code=ValidationErrors.SIDECAR_INVALID)
+def SIDECAR_HED_USED():
+    return "'HED' is a reserved name and cannot be used as a sidecar except in expected places."
+
 
+@hed_error(SidecarErrors.SIDECAR_HED_USED_COLUMN, actual_code=ValidationErrors.SIDECAR_INVALID)
+def SIDECAR_HED_USED_COLUMN():
+    return "'HED' is a reserved name and cannot be used as a sidecar column name"
 
-@hed_tag_error(DefinitionErrors.DEF_TAG_IN_DEFINITION, actual_code=ValidationErrors.HED_DEFINITION_INVALID)
+
+@hed_error(SidecarErrors.SIDECAR_NA_USED, actual_code=ValidationErrors.SIDECAR_INVALID)
+def sidecar_na_used(column_name):
+    return f"Invalid category key 'n/a' found in column {column_name}."
+
+
+@hed_tag_error(DefinitionErrors.DEF_TAG_IN_DEFINITION, actual_code=ValidationErrors.DEFINITION_INVALID)
 def def_error_def_tag_in_definition(tag, def_name):
     return f"Invalid tag {tag} found in definition for {def_name}. " +\
-           f"Def and Def-expand tags cannot be in definitions.", {}
+           f"Def, Def-expand, and Definition tags cannot be in definitions."
+
 
+@hed_error(DefinitionErrors.NO_DEFINITION_CONTENTS, actual_code=ValidationErrors.DEFINITION_INVALID)
+def def_error_no_group_tags(def_name):
+    return f"No group tag found in definition for {def_name}."
 
-@hed_error(DefinitionErrors.WRONG_NUMBER_GROUP_TAGS, actual_code=ValidationErrors.HED_DEFINITION_INVALID)
+
+@hed_error(DefinitionErrors.WRONG_NUMBER_GROUPS, actual_code=ValidationErrors.DEFINITION_INVALID)
 def def_error_wrong_group_tags(def_name, tag_list):
     tag_list_strings = [str(tag) for tag in tag_list]
-    return f"Too many group tags found in definition for {def_name}.  Expected 1, found: {tag_list_strings}", {}
+    return f"Too many group tags found in definition for {def_name}.  Expected 1, found: {tag_list_strings}"
 
 
-@hed_error(DefinitionErrors.WRONG_NUMBER_PLACEHOLDER_TAGS, actual_code=ValidationErrors.HED_DEFINITION_INVALID)
+@hed_error(DefinitionErrors.WRONG_NUMBER_TAGS, actual_code=ValidationErrors.DEFINITION_INVALID)
+def def_error_wrong_group_tags(def_name, tag_list):
+    tag_list_strings = [str(tag) for tag in tag_list]
+    return f"Too many tags found in definition for {def_name}.  Expected 1, found: {tag_list_strings}"
+
+
+
+@hed_error(DefinitionErrors.WRONG_NUMBER_PLACEHOLDER_TAGS, actual_code=ValidationErrors.DEFINITION_INVALID)
 def def_error_wrong_placeholder_count(def_name, expected_count, tag_list):
     tag_list_strings = [str(tag) for tag in tag_list]
-    return f"Incorrect number placeholder tags found in definition for {def_name}.  " + \
-           f"Expected {expected_count}, found: {tag_list_strings}", {}
+    return f"Incorrect number placeholders or placeholder tags found in definition for {def_name}.  " + \
+           f"Expected {expected_count}, found: {tag_list_strings}"
 
 
-@hed_error(DefinitionErrors.DUPLICATE_DEFINITION, actual_code=ValidationErrors.HED_DEFINITION_INVALID)
+@hed_error(DefinitionErrors.DUPLICATE_DEFINITION, actual_code=ValidationErrors.DEFINITION_INVALID)
 def def_error_duplicate_definition(def_name):
-    return f"Duplicate definition found for '{def_name}'.", {}
+    return f"Duplicate definition found for '{def_name}'."
+
+
+@hed_tag_error(DefinitionErrors.INVALID_DEFINITION_EXTENSION, actual_code=ValidationErrors.DEFINITION_INVALID)
+def def_error_invalid_def_extension(tag, def_name):
+    return f"Tag '{str(tag)}' has an invalid placeholder in definition '{def_name}'"
+
 
+@hed_error(DefinitionErrors.PLACEHOLDER_NO_TAKES_VALUE, actual_code=ValidationErrors.DEFINITION_INVALID)
+def def_error_no_takes_value(def_name, placeholder_tag):
+    return f"Definition '{def_name}' has has a placeholder tag {str(placeholder_tag)} that isn't a takes value tag."
 
-@hed_error(DefinitionErrors.TAG_IN_SCHEMA, actual_code=ValidationErrors.HED_DEFINITION_INVALID)
-def def_error_tag_already_in_schema(def_name):
-    return f"Term '{def_name}' already used as term in schema and cannot be re-used as a definition.", {}
 
+@hed_tag_error(DefinitionErrors.BAD_PROP_IN_DEFINITION, actual_code=ValidationErrors.DEFINITION_INVALID)
+def def_error_no_takes_value(tag, def_name):
+    return f"Tag '{str(tag)}' in Definition '{def_name}' has has a tag with the unique or required attribute."
 
-@hed_error(DefinitionErrors.INVALID_DEFINITION_EXTENSION, actual_code=ValidationErrors.HED_DEFINITION_INVALID)
-def def_error_invalid_def_extension(def_name):
-    return f"Term '{def_name}' has an invalid extension.  Definitions can only have one term.", {}
 
+@hed_tag_error(DefinitionErrors.BAD_DEFINITION_LOCATION, actual_code=ValidationErrors.DEFINITION_INVALID)
+def def_error_bad_location(tag):
+    return f"Tag '{str(tag)}' is found in a location it is not allowed to be."
 
-@hed_tag_error(OnsetErrors.ONSET_DEF_UNMATCHED, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+
+@hed_tag_error(OnsetErrors.ONSET_DEF_UNMATCHED, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_error_def_unmatched(tag):
-    return f"The def tag in an onset/offset tag is unmatched.  Def tag: '{tag}'", {}
+    return f"The def tag in an onset/offset tag is unmatched.  Def tag: '{tag}'"
 
 
-@hed_tag_error(OnsetErrors.OFFSET_BEFORE_ONSET, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+@hed_tag_error(OnsetErrors.OFFSET_BEFORE_ONSET, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_error_offset_before_onset(tag):
-    return f"Offset tag '{tag}' does not have a matching onset.", {}
+    return f"Offset tag '{tag}' does not have a matching onset."
+
 
+@hed_tag_error(OnsetErrors.INSET_BEFORE_ONSET, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
+def onset_error_inset_before_onset(tag):
+    return f"Inset tag '{tag}' does not have a matching onset."
 
-@hed_tag_error(OnsetErrors.ONSET_NO_DEF_TAG_FOUND, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+
+@hed_tag_error(OnsetErrors.ONSET_NO_DEF_TAG_FOUND, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_no_def_found(tag):
-    return f"'{tag}' tag has no def or def-expand tag in string.", {}
+    return f"'{tag}' tag has no def or def-expand tag in string."
 
 
-@hed_tag_error(OnsetErrors.ONSET_TOO_MANY_DEFS, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+@hed_tag_error(OnsetErrors.ONSET_TOO_MANY_DEFS, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_too_many_defs(tag, tag_list):
     tag_list_strings = [str(tag) for tag in tag_list]
-    return f"Too many def tags found in onset for {tag}.  Expected 1, also found: {tag_list_strings}", {}
+    return f"Too many def tags found in onset for {tag}.  Expected 1, also found: {tag_list_strings}"
 
 
-@hed_tag_error(OnsetErrors.ONSET_WRONG_NUMBER_GROUPS, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+@hed_tag_error(OnsetErrors.ONSET_WRONG_NUMBER_GROUPS, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_too_many_groups(tag, tag_list):
     tag_list_strings = [str(a_tag) for a_tag in tag_list]
     return f"An onset tag should have at most 2 sibling nodes, an offset tag should have 1. " +\
-           f"Found {len(tag_list_strings)}: {tag_list_strings}", {}
+           f"Found {len(tag_list_strings)}: {tag_list_strings}"
 
 
-@hed_tag_error(OnsetErrors.ONSET_TAG_OUTSIDE_OF_GROUP, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+@hed_tag_error(OnsetErrors.ONSET_TAG_OUTSIDE_OF_GROUP, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_wrong_type_tag(tag, def_tag):
     return f"Onset def tag '{def_tag}' has an improper sibling tag '{tag}'.  All onset context tags must be " + \
-           f"in a single group together.", {}
+           f"in a single group together."
 
 
-@hed_tag_error(OnsetErrors.ONSET_PLACEHOLDER_WRONG, actual_code=ValidationErrors.HED_ONSET_OFFSET_ERROR)
+@hed_tag_error(OnsetErrors.ONSET_PLACEHOLDER_WRONG, actual_code=ValidationErrors.ONSET_OFFSET_INSET_ERROR)
 def onset_wrong_placeholder(tag, has_placeholder):
     if has_placeholder:
-        return f"Onset/offset def tag {tag} expects a placeholder value, but does not have one.", {}
-    return f"Onset/offset def tag {tag} should not have a placeholder, but has one.", {}
+        return f"Onset/offset def tag {tag} expects a placeholder value, but does not have one."
+    return f"Onset/offset def tag {tag} should not have a placeholder, but has one."
+
+
+@hed_error(ColumnErrors.INVALID_COLUMN_REF, actual_code=SidecarErrors.SIDECAR_BRACES_INVALID)
+def invalid_column_ref(bad_ref):
+    return f"The column '{bad_ref}' is unknown.'"
+
+
+@hed_error(ColumnErrors.SELF_COLUMN_REF, actual_code=SidecarErrors.SIDECAR_BRACES_INVALID)
+def self_column_ref(self_ref):
+    return f"Column references itself: {self_ref}"
+
+
+@hed_error(ColumnErrors.NESTED_COLUMN_REF, actual_code=SidecarErrors.SIDECAR_BRACES_INVALID)
+def nested_column_ref(column_name, ref_column):
+    return f"Column {column_name} has a nested reference to {ref_column}.  " \
+           f"Column reference columns cannot contain other column references."
+
+
+@hed_error(ColumnErrors.MALFORMED_COLUMN_REF, actual_code=SidecarErrors.SIDECAR_BRACES_INVALID)
+def nested_column_ref(column_name, index, symbol):
+    return f"Column {column_name} has a malformed column reference.  Improper symbol {symbol} found at index {index}."
+
+
```

### Comparing `hedtools-0.2.0/hed/errors/error_reporter.py` & `hedtools-0.3.0/hed/errors/error_reporter.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,40 @@
 
 from functools import wraps
 import copy
 from hed.errors.error_types import ErrorContext, ErrorSeverity
 
 error_functions = {}
 
+# Controls if the default issue printing skips adding indentation for this context
+no_tab_context = {ErrorContext.HED_STRING, ErrorContext.SCHEMA_ATTRIBUTE}
+
+# Default sort ordering for issues list
+default_sort_list = [
+    ErrorContext.CUSTOM_TITLE,
+    ErrorContext.FILE_NAME,
+    ErrorContext.SIDECAR_COLUMN_NAME,
+    ErrorContext.SIDECAR_KEY_NAME,
+    ErrorContext.ROW,
+    ErrorContext.COLUMN,
+    ErrorContext.LINE,
+    # ErrorContext.HED_STRING, # temporarily disable hed string sort(maybe perm, not sure it's needed)
+    ErrorContext.SCHEMA_SECTION,
+    ErrorContext.SCHEMA_TAG,
+    ErrorContext.SCHEMA_ATTRIBUTE,
+]
+
+# ErrorContext which is expected to be int based.
+int_sort_list = [
+    ErrorContext.ROW
+]
+
+hed_string_sort_list = [
+    ErrorContext.HED_STRING
+]
 
 def _register_error_function(error_type, wrapper_func):
     if error_type in error_functions:
         raise KeyError(f"{error_type} defined more than once.")
 
     error_functions[error_type] = wrapper_func
 
@@ -39,16 +65,16 @@
                 args (args): non keyword args.
                 severity (ErrorSeverity): Will override the default error value if passed.
                 kwargs (**kwargs): Any keyword args to be passed down to error message function.
 
             Returns:
                 list: A list of dict with the errors.=
             """
-            base_message, error_vars = func(*args, **kwargs)
-            error_object = ErrorHandler._create_error_object(actual_code, base_message, severity, **error_vars)
+            base_message = func(*args, **kwargs)
+            error_object = ErrorHandler._create_error_object(actual_code, base_message, severity)
             return error_object
 
         _register_error_function(error_type, wrapper_func=wrapper)
         return wrapper
 
     return inner_decorator
 
@@ -93,16 +119,16 @@
                     index_in_tag_end = len(tag_as_string)
                 problem_sub_tag = tag_as_string[index_in_tag: index_in_tag_end]
                 try:
                     org_tag_text = tag.org_tag
                 except AttributeError:
                     org_tag_text = str(tag)
 
-                base_message, error_vars = func(org_tag_text, problem_sub_tag, *args, **kwargs)
-                error_object = ErrorHandler._create_error_object(actual_code, base_message, severity, **error_vars,
+                base_message = func(org_tag_text, problem_sub_tag, *args, **kwargs)
+                error_object = ErrorHandler._create_error_object(actual_code, base_message, severity,
                                                                  index_in_tag=index_in_tag,
                                                                  index_in_tag_end=index_in_tag_end, source_tag=tag)
 
                 return error_object
 
             _register_error_function(error_type, wrapper_func=wrapper)
             return wrapper
@@ -125,16 +151,16 @@
                 from hed.models.hed_group import HedGroup
                 if isinstance(tag, HedTag):
                     org_tag_text = tag.org_tag
                 elif isinstance(tag, HedGroup):
                     org_tag_text = tag.get_original_hed_string()
                 else:
                     org_tag_text = str(tag)
-                base_message, error_vars = func(org_tag_text, *args, **kwargs)
-                error_object = ErrorHandler._create_error_object(actual_code, base_message, severity, **error_vars,
+                base_message = func(org_tag_text, *args, **kwargs)
+                error_object = ErrorHandler._create_error_object(actual_code, base_message, severity,
                                                                  source_tag=tag)
 
                 return error_object
 
             _register_error_function(error_type, wrapper_func=wrapper)
             return wrapper
 
@@ -144,31 +170,39 @@
 # Import after hed_error decorators are defined.
 from hed.errors import error_messages
 # Intentional to make sure tools don't think the import is unused
 error_messages.mark_as_used = True
 
 
 class ErrorHandler:
-    def __init__(self):
+    def __init__(self, check_for_warnings=True):
         # The current (ordered) dictionary of contexts.
         self.error_context = []
+        self._check_for_warnings = check_for_warnings
 
-    def push_error_context(self, context_type, context, increment_depth_after=True):
+    def push_error_context(self, context_type, context):
         """ Push a new error context to narrow down error scope.
 
         Parameters:
             context_type (ErrorContext): A value from ErrorContext representing the type of scope.
             context (str, int, or HedString): The main value for the context_type.
-            increment_depth_after (bool): If True, add an extra tab to any subsequent errors in the scope.
 
         Notes:
             The context depends on the context_type. For ErrorContext.FILE_NAME this would be the actual filename.
 
         """
-        self.error_context.append((context_type, context, increment_depth_after))
+        if context is None:
+            from hed import HedString
+            if context_type in int_sort_list:
+                context = 0
+            elif context_type in hed_string_sort_list:
+                context = HedString("")
+            else:
+                context = ""
+        self.error_context.append((context_type, context))
 
     def pop_error_context(self):
         """ Remove the last scope from the error context.
 
         Notes:
             Modifies the error context of this reporter.
 
@@ -187,28 +221,32 @@
 
     def get_error_context_copy(self):
         return copy.copy(self.error_context)
 
     def format_error_with_context(self, *args, **kwargs):
         error_object = ErrorHandler.format_error(*args, **kwargs)
         if self is not None:
-            self._add_context_to_errors(error_object[0], self.error_context)
-            self._update_error_with_char_pos(error_object[0])
+            actual_error = error_object[0]
+            # # Filter out warning errors
+            if not self._check_for_warnings and actual_error['severity'] >= ErrorSeverity.WARNING:
+                return []
+            self._add_context_to_errors(actual_error, self.error_context)
+            self._update_error_with_char_pos(actual_error)
 
         return error_object
 
     @staticmethod
     def format_error(error_type, *args, actual_error=None, **kwargs):
         """ Format an error based on the parameters, which vary based on what type of error this is.
 
         Parameters:
             error_type (str): The type of error for this.  Registered with @hed_error or @hed_tag_error.
             args (args): Any remaining non keyword args after those required by the error type.
             actual_error (str or None): Code to actually add to report out.
-            kwargs (dict): The other keyword args to pass down to the error handling func.
+            kwargs (kwargs): The other keyword args to pass down to the error handling func.
 
         Returns:
             list:   A list containing a single dictionary representing a single error.
 
         Notes:
             The actual error is useful for errors that are shared like invalid character.
 
@@ -221,34 +259,27 @@
 
         error_object = error_func(*args, **kwargs)
         if actual_error:
             error_object['code'] = actual_error
 
         return [error_object]
 
-    def add_context_to_issues(self, issues):
+    def add_context_and_filter(self, issues):
+        """ Filter out warnings if requested, while adding context to issues.
+
+            issues(list):
+                list:   A list containing a single dictionary representing a single error.
+        """
+        if not self._check_for_warnings:
+            issues[:] = self.filter_issues_by_severity(issues, ErrorSeverity.ERROR)
+
         for error_object in issues:
             self._add_context_to_errors(error_object, self.error_context)
             self._update_error_with_char_pos(error_object)
 
-    def format_error_list(self, issue_params):
-        """ Convert an issue params list to an issues list.  This means adding the error context primarily.
-
-        Parameters:
-            issue_params (list):  A list of dict containing the unformatted issues list.
-
-        Returns:
-            list: A list of dict containing unformatted errors.
-
-        """
-        formatted_issues = []
-        for issue in issue_params:
-            formatted_issues += self.format_error(**issue)
-        return formatted_issues
-
     @staticmethod
     def format_error_from_context(error_type, error_context, *args, actual_error=None, **kwargs):
         """ Format an error based on the error type.
 
         Parameters:
             error_type (str): The type of error.  Registered with @hed_error or @hed_tag_error.
             error_context (list): Contains the error context to use for this error.
@@ -258,14 +289,15 @@
 
         Returns:
             list:  A list containing a single dictionary
 
         Notes:
             - Generally the error_context is returned from _add_context_to_errors.
             - The actual_error is useful for errors that are shared like invalid character.
+            - This can't filter out warnings like the other ones.
 
         """
         error_func = error_functions.get(error_type)
         if not error_func:
             error_object = ErrorHandler.val_error_unknown(*args, **kwargs)
             error_object['code'] = error_type
             ErrorHandler._add_context_to_errors(error_object, error_context)
@@ -289,16 +321,16 @@
 
         Returns:
             list: A list of dict with needed context strings added at the beginning of the list.
 
         """
         if error_object is None:
             error_object = {}
-        for (context_type, context, increment_count) in error_context_to_add:
-            error_object[context_type] = (context, increment_count)
+        for (context_type, context) in error_context_to_add:
+            error_object[context_type] = context
 
         return error_object
 
     @staticmethod
     def _create_error_object(error_type, base_message, severity, **kwargs):
         if severity == ErrorSeverity.ERROR:
             error_prefix = "ERROR: "
@@ -327,15 +359,15 @@
         elif 'source_tag' in error_object:
             source_tag = error_object['source_tag']
             if isinstance(source_tag, int):
                 return None, None
         else:
             return None, None
 
-        hed_string = error_object[ErrorContext.HED_STRING][0]
+        hed_string = error_object[ErrorContext.HED_STRING]
         span = hed_string._get_org_span(source_tag)
         return span
 
     @staticmethod
     def _update_error_with_char_pos(error_object):
         # This part is optional as you can always generate these as needed.
         start, end = ErrorHandler._get_tag_span_to_error_object(error_object)
@@ -360,18 +392,17 @@
 
         Parameters:
             args (args):     List of non-keyword parameters (varies).
             kwargs (kwargs): Keyword parameters (varies)
 
         Returns:
             str: The error message.
-            dict: The extra args.
 
         """
-        return f"Unknown error.  Args: {str(args)}", kwargs
+        return f"Unknown error.  Args: {str(args), str(kwargs)}"
 
     @staticmethod
     def filter_issues_by_severity(issues_list, severity):
         """ Gather all issues matching or below a given severity.
 
         Parameters:
             issues_list (list): A list of dictionaries containing the full issue list.
@@ -380,39 +411,38 @@
         Returns:
             list: A list of dictionaries containing the issue list after filtering by severity.
 
         """
         return [issue for issue in issues_list if issue['severity'] <= severity]
 
 
-def get_exception_issue_string(issues, title=None):
-    """ Return a string with issues list flatted into single string, one issue per line.
+def sort_issues(issues, reverse=False):
+    """Sorts a list of issues by the error context values.
 
     Parameters:
-        issues (list):  A list of strings containing issues to print.
-        title (str or None): An optional title that will always show up first if present.
+        issues (list): A list of dictionaries representing the issues to be sorted.
+        reverse (bool, optional): If True, sorts the list in descending order. Default is False.
 
     Returns:
-        str: A str containing printable version of the issues or ''.
+        list: The sorted list of issues."""
+    def _get_keys(d):
+        from hed import HedString
+        result = []
+        for key in default_sort_list:
+            if key in int_sort_list:
+                result.append(d.get(key, -1))
+            elif key in hed_string_sort_list:
+                result.append(d.get(key, HedString("")))
+            else:
+                result.append(d.get(key, ""))
+        return tuple(result)
 
-    """
-    issue_str = ''
-    if issues:
-        issue_list = []
-        for issue in issues:
-            this_str = f"{issue['message']}"
-            if 'code' in issue:
-                this_str = f"{issue['code']}:" + this_str
-            if 'line_number' in issue:
-                this_str = this_str + f"\n\tLine number {issue['line_number']}: {issue.get('line', '')} "
-            issue_list.append(this_str)
-        issue_str += '\n' + '\n'.join(issue_list)
-    if title:
-        issue_str = title + '\n' + issue_str
-    return issue_str
+    issues = sorted(issues, key=_get_keys, reverse=reverse)
+
+    return issues
 
 
 def get_printable_issue_string(issues, title=None, severity=None, skip_filename=True):
     """ Return a string with issues list flatted into single string, one per line.
 
     Parameters:
         issues (list):  Issues to print.
@@ -468,15 +498,15 @@
 
     """
     single_issue_context = []
     for key in val_issue:
         if skip_filename and key == ErrorContext.FILE_NAME:
             continue
         if key.startswith("ec_"):
-            single_issue_context.append((key, *val_issue[key]))
+            single_issue_context.append((key, val_issue[key]))
 
     return single_issue_context
 
 
 def _format_single_context_string(context_type, context, tab_count=0):
     """ Return the human readable form of a single context tuple.
 
@@ -495,29 +525,30 @@
     error_types = {
         ErrorContext.FILE_NAME: f"\nErrors in file '{context}'",
         ErrorContext.SIDECAR_COLUMN_NAME: f"Column '{context}':",
         ErrorContext.SIDECAR_KEY_NAME: f"Key: {context}",
         ErrorContext.ROW: f'Issues in row {context}:',
         ErrorContext.COLUMN: f'Issues in column {context}:',
         ErrorContext.CUSTOM_TITLE: context,
+        ErrorContext.LINE: f"Line: {context}",
         ErrorContext.HED_STRING: f"hed string: {context}",
         ErrorContext.SCHEMA_SECTION: f"Schema Section: {context}",
         ErrorContext.SCHEMA_TAG: f"Source tag: {context}",
         ErrorContext.SCHEMA_ATTRIBUTE: f"Source Attribute: {context}",
     }
     context_portion = error_types[context_type]
     context_string = f"{tab_string}{context_portion}\n"
     return context_string
 
 
 def _get_context_string(single_issue_context, last_used_context):
     """ Convert a single context list into the final human readable output form.
 
     Parameters:
-        single_issue_context (list): A list of tuples containing the context(context_type, context, increment_tab)
+        single_issue_context (list): A list of tuples containing the context(context_type, context)
         last_used_context (list): A list of tuples containing the last drawn context.
 
     Returns:
         str: The full string of context(potentially multiline) to add before the error.
         str: The tab string to add to the front of any message line with this context.
 
     Notes:
@@ -525,23 +556,23 @@
         so that the error handling can only add the parts that have changed.
 
     """
     context_string = ""
     tab_count = 0
     found_difference = False
     for i, context_tuple in enumerate(single_issue_context):
-        (context_type, context, increment_tab) = context_tuple
+        (context_type, context) = context_tuple
         if len(last_used_context) > i and not found_difference:
             last_drawn = last_used_context[i]
             # Was drawn, and hasn't changed.
             if last_drawn == context_tuple:
-                if increment_tab:
+                if context_type not in no_tab_context:
                     tab_count += 1
                 continue
 
         context_string += _format_single_context_string(context_type, context, tab_count)
         found_difference = True
-        if increment_tab:
+        if context_type not in no_tab_context:
             tab_count += 1
 
     tab_string = '\t' * tab_count
     return context_string, tab_string
```

### Comparing `hedtools-0.2.0/hed/errors/error_types.py` & `hedtools-0.3.0/hed/errors/error_types.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,108 +9,147 @@
     # Use this one to display any passed in message without modification
     CUSTOM_TITLE = 'ec_title'
     FILE_NAME = 'ec_filename'
     SIDECAR_COLUMN_NAME = 'ec_sidecarColumnName'
     SIDECAR_KEY_NAME = 'ec_sidecarKeyName'
     ROW = 'ec_row'
     COLUMN = 'ec_column'
+    LINE = "ec_line"
     HED_STRING = 'ec_HedString'
     SCHEMA_SECTION = 'ec_section'
     SCHEMA_TAG = 'ec_schema_tag'
     SCHEMA_ATTRIBUTE = 'ec_attribute'
 
 
 class ValidationErrors:
     # General validation errors
-    HED_CHARACTER_INVALID = 'HED_CHARACTER_INVALID'
-    HED_COMMA_MISSING = 'HED_COMMA_MISSING'
+    CHARACTER_INVALID = 'CHARACTER_INVALID'
+    COMMA_MISSING = 'COMMA_MISSING'
+    DEF_EXPAND_INVALID = "DEF_EXPAND_INVALID"
+    DEF_INVALID = "DEF_INVALID"
+    DEFINITION_INVALID = "DEFINITION_INVALID"
+    NODE_NAME_EMPTY = 'NODE_NAME_EMPTY'
+    ONSET_OFFSET_INSET_ERROR = 'ONSET_OFFSET_INSET_ERROR'
+    PARENTHESES_MISMATCH = 'PARENTHESES_MISMATCH'
+    PLACEHOLDER_INVALID = 'PLACEHOLDER_INVALID'
+    REQUIRED_TAG_MISSING = 'REQUIRED_TAG_MISSING'
+    SIDECAR_INVALID = 'SIDECAR_INVALID'
+    SIDECAR_KEY_MISSING = 'SIDECAR_KEY_MISSING'
+    STYLE_WARNING = "STYLE_WARNING"
+    TAG_EMPTY = 'TAG_EMPTY'
+    TAG_EXPRESSION_REPEATED = 'TAG_EXPRESSION_REPEATED'
+    TAG_EXTENDED = 'TAG_EXTENDED'
+    TAG_EXTENSION_INVALID = 'TAG_EXTENSION_INVALID'
+    TAG_GROUP_ERROR = "TAG_GROUP_ERROR"
+    TAG_INVALID = "TAG_INVALID"
+    TAG_NOT_UNIQUE = 'TAG_NOT_UNIQUE'
+    TAG_NAMESPACE_PREFIX_INVALID = 'TAG_NAMESPACE_PREFIX_INVALID'
+    TAG_REQUIRES_CHILD = 'TAG_REQUIRES_CHILD'
+    TILDES_UNSUPPORTED = 'TILDES_UNSUPPORTED'
+    UNITS_INVALID = 'UNITS_INVALID'
+    UNITS_MISSING = 'UNITS_MISSING'
+    VERSION_DEPRECATED = 'VERSION_DEPRECATED'
+    VALUE_INVALID = 'VALUE_INVALID'
+
+    # Internal codes
     HED_DEF_UNMATCHED = "HED_DEF_UNMATCHED"
+    HED_DEF_VALUE_MISSING = "HED_DEF_VALUE_MISSING"
+    HED_DEF_VALUE_EXTRA = "HED_DEF_VALUE_EXTRA"
+
     HED_DEF_EXPAND_INVALID = "HED_DEF_EXPAND_INVALID"
-    HED_DEF_VALUE_INVALID = "HED_DEF_VALUE_INVALID"
-    HED_DEFINITION_INVALID = "HED_DEFINITION_INVALID"
-    HED_NODE_NAME_EMPTY = 'HED_NODE_NAME_EMPTY'
-    HED_ONSET_OFFSET_ERROR = 'HED_ONSET_OFFSET_ERROR'
-    HED_PARENTHESES_MISMATCH = 'HED_PARENTHESES_MISMATCH'
-    HED_PLACEHOLDER_INVALID = 'HED_PLACEHOLDER_INVALID'
-    HED_REQUIRED_TAG_MISSING = 'HED_REQUIRED_TAG_MISSING'
-    HED_SIDECAR_KEY_MISSING = 'HED_SIDECAR_KEY_MISSING'
-    HED_STYLE_WARNING = 'HED_STYLE_WARNING'
-    HED_TAG_EMPTY = 'HED_TAG_EMPTY'
-    HED_TAG_EXTENDED = 'HED_TAG_EXTENDED'
-    HED_TAG_GROUP_ERROR = "HED_TAG_GROUP_ERROR"
-    HED_TAG_INVALID = "HED_TAG_INVALID"
-    HED_TAG_NOT_UNIQUE = 'HED_TAG_NOT_UNIQUE'
+    HED_DEF_EXPAND_UNMATCHED = "HED_DEF_EXPAND_UNMATCHED"
+    HED_DEF_EXPAND_VALUE_MISSING = "HED_DEF_EXPAND_VALUE_MISSING"
+    HED_DEF_EXPAND_VALUE_EXTRA = "HED_DEF_EXPAND_VALUE_EXTRA"
+
     HED_TAG_REPEATED = 'HED_TAG_REPEATED'
     HED_TAG_REPEATED_GROUP = 'HED_TAG_REPEATED_GROUP'
-    HED_TAG_REQUIRES_CHILD = 'HED_TAG_REQUIRES_CHILD'
-    HED_TILDES_UNSUPPORTED = 'HED_TILDES_UNSUPPORTED'
-    HED_UNITS_INVALID = 'HED_UNITS_INVALID'
-    HED_UNITS_DEFAULT_USED = 'HED_UNITS_DEFAULT_USED'
-    HED_VALUE_INVALID = 'HED_VALUE_INVALID'
+
+    INVALID_PARENT_NODE = "invalidParent"
+    NO_VALID_TAG_FOUND = "invalidTag"
+
     HED_LIBRARY_UNMATCHED = "HED_LIBRARY_UNMATCHED"
-    # HED_VERSION_WARNING
+
+    HED_TOP_LEVEL_TAG = "HED_TOP_LEVEL_TAG"
+    HED_MULTIPLE_TOP_TAGS = "HED_MULTIPLE_TOP_TAGS"
+    HED_TAG_GROUP_TAG = "HED_TAG_GROUP_TAG"
+
+    HED_GROUP_EMPTY = 'HED_GROUP_EMPTY'
+    # end internal codes
+
+
+    # Still being worked on below this line
 
     HED_MISSING_REQUIRED_COLUMN = "HED_MISSING_REQUIRED_COLUMN"
     HED_UNKNOWN_COLUMN = "HED_UNKNOWN_COLUMN"
-    HED_DUPLICATE_COLUMN = "HED_DUPLICATE_COLUMN"
-    HED_BLANK_COLUMN = "HED_BLANK_COLUMN"
+    SIDECAR_AND_OTHER_COLUMNS = "SIDECAR_AND_OTHER_COLUMNS"
 
+    DUPLICATE_COLUMN_IN_LIST = "DUPLICATE_COLUMN_IN_LIST"
+    DUPLICATE_COLUMN_BETWEEN_SOURCES = "DUPLICATE_COLUMN_BETWEEN_SOURCES"
+    HED_BLANK_COLUMN = "HED_BLANK_COLUMN"
 
     # Below here shows what the given error maps to
-    HED_GROUP_EMPTY = 'emptyHedGroup'
-    INVALID_TAG_CHARACTER = 'invalidTagCharacter'
-
-    # These are all HED_TAG_INVALID
-    INVALID_EXTENSION = 'invalidExtension'
-    INVALID_PARENT_NODE = "invalidParent"
-    NO_VALID_TAG_FOUND = "invalidTag"
 
-    # These are misc errors that need categorization.
-    HED_TOP_LEVEL_TAG = "HED_TOP_LEVEL_TAG"
-    HED_MULTIPLE_TOP_TAGS = "HED_MULTIPLE_TOP_TAGS"
-    HED_TAG_GROUP_TAG = "HED_TAG_GROUP_TAG"
+    INVALID_TAG_CHARACTER = 'invalidTagCharacter'
 
-    HED_DEF_VALUE_MISSING = "HED_DEF_VALUE_MISSING"
-    HED_DEF_VALUE_EXTRA = "HED_DEF_VALUE_EXTRA"
 
 
 class SidecarErrors:
     # These are for json sidecar validation errors(sidecars can also produce most normal validation errors)
     BLANK_HED_STRING = 'blankValueString'
     WRONG_HED_DATA_TYPE = 'wrongHedDataType'
     INVALID_POUND_SIGNS_VALUE = 'invalidNumberPoundSigns'
     INVALID_POUND_SIGNS_CATEGORY = 'tooManyPoundSigns'
     UNKNOWN_COLUMN_TYPE = 'sidecarUnknownColumn'
+    SIDECAR_HED_USED_COLUMN = 'SIDECAR_HED_USED_COLUMN'
+    SIDECAR_NA_USED = 'SIDECAR_NA_USED'
+    SIDECAR_HED_USED = 'SIDECAR_HED_USED'
+    SIDECAR_BRACES_INVALID = "SIDECAR_BRACES_INVALID"
 
 
 class SchemaErrors:
     HED_SCHEMA_DUPLICATE_NODE = 'HED_SCHEMA_DUPLICATE_NODE'
-    HED_SCHEMA_ATTRIBUTE_INVALID = 'HED_SCHEMA_ATTRIBUTE_INVALID'
+    SCHEMA_ATTRIBUTE_INVALID = 'SCHEMA_ATTRIBUTE_INVALID'
+    HED_SCHEMA_DUPLICATE_FROM_LIBRARY = "SCHEMA_LIBRARY_INVALID"
 
 
 class SchemaWarnings:
     INVALID_CHARACTERS_IN_DESC = "INVALID_CHARACTERS_IN_DESC"
     INVALID_CHARACTERS_IN_TAG = "INVALID_CHARACTERS_IN_TAG"
     # The actual reported error for the above two
     HED_SCHEMA_CHARACTER_INVALID = "HED_SCHEMA_CHARACTER_INVALID"
     INVALID_CAPITALIZATION = 'invalidCaps'
     NON_PLACEHOLDER_HAS_CLASS = 'NON_PLACEHOLDER_HAS_CLASS'
+    INVALID_ATTRIBUTE = "INVALID_ATTRIBUTE"
 
 
-# These are all HED_DEFINITION_INVALID errors
 class DefinitionErrors:
-    DEF_TAG_IN_DEFINITION = 'DEF_TAG_IN_DEFINITION'
-    WRONG_NUMBER_GROUP_TAGS = 'wrongNumberGroupTags'
+    # These are all DEFINITION_INVALID errors
     WRONG_NUMBER_PLACEHOLDER_TAGS = 'wrongNumberPlaceholderTags'
     DUPLICATE_DEFINITION = 'duplicateDefinition'
-    TAG_IN_SCHEMA = 'defAlreadyInSchema'
     INVALID_DEFINITION_EXTENSION = 'invalidDefExtension'
+    DEF_TAG_IN_DEFINITION = 'DEF_TAG_IN_DEFINITION'
+    NO_DEFINITION_CONTENTS = "NO_DEFINITION_CONTENTS"
+    PLACEHOLDER_NO_TAKES_VALUE = 'PLACEHOLDER_NO_TAKES_VALUE'
+
+    WRONG_NUMBER_TAGS = 'WRONG_NUMBER_TAGS'
+    WRONG_NUMBER_GROUPS = 'WRONG_NUMBER_GROUPS'
+    BAD_PROP_IN_DEFINITION = 'BAD_PROP_IN_DEFINITION'
+
+    BAD_DEFINITION_LOCATION = 'BAD_DEFINITION_LOCATION'
 
 
 class OnsetErrors:
+    # These are all ONSET_OFFSET_INSET_ERROR
     OFFSET_BEFORE_ONSET = "OFFSET_BEFORE_ONSET"
     ONSET_DEF_UNMATCHED = "ONSET_DEF_UNMATCHED"
     ONSET_WRONG_NUMBER_GROUPS = "ONSET_WRONG_NUMBER_GROUPS"
     ONSET_NO_DEF_TAG_FOUND = "ONSET_NO_DEF_TAG_FOUND"
     ONSET_PLACEHOLDER_WRONG = "ONSET_PLACEHOLDER_WRONG"
     ONSET_TOO_MANY_DEFS = "ONSET_TOO_MANY_DEFS"
     ONSET_TAG_OUTSIDE_OF_GROUP = "ONSET_TAG_OUTSIDE_OF_GROUP"
+    INSET_BEFORE_ONSET = "INSET_BEFORE_ONSET"
+
+class ColumnErrors:
+    INVALID_COLUMN_REF = "INVALID_COLUMN_REF"
+    SELF_COLUMN_REF = "SELF_COLUMN_REF"
+    NESTED_COLUMN_REF = "NESTED_COLUMN_REF"
+    MALFORMED_COLUMN_REF = "MALFORMED_COLUMN_REF"
```

### Comparing `hedtools-0.2.0/hed/models/__init__.py` & `hedtools-0.3.0/hed/models/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """ Data structures for HED tag handling. """
 
 from .base_input import BaseInput
 from .column_mapper import ColumnMapper
 from .column_metadata import ColumnMetadata, ColumnType
 from .definition_dict import DefinitionDict
 from .definition_entry import DefinitionEntry
-from .def_mapper import DefMapper
 from .expression_parser import QueryParser
 from .hed_group import HedGroup
 from .spreadsheet_input import SpreadsheetInput
-from .hed_ops import HedOps
 from .hed_string import HedString
 from .hed_string_group import HedStringGroup
 from .hed_tag import HedTag
-from .onset_mapper import OnsetMapper
 from .sidecar import Sidecar
 from .tabular_input import TabularInput
 from .timeseries_input import TimeseriesInput
+from .df_util import get_assembled, convert_to_form, shrink_defs, expand_defs, process_def_expands
```

### Comparing `hedtools-0.2.0/hed/models/column_mapper.py` & `hedtools-0.3.0/hed/models/column_mapper.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,193 +1,209 @@
 from hed.models.column_metadata import ColumnMetadata, ColumnType
 from hed.models.sidecar import Sidecar
-from hed.models.hed_string import HedString
-from hed.models import model_constants
 from hed.errors.error_reporter import ErrorHandler
 from hed.errors.error_types import ValidationErrors
 
 import copy
-
+from collections import Counter
 
 PANDAS_COLUMN_PREFIX_TO_IGNORE = "Unnamed: "
 
 
 class ColumnMapper:
     """ Mapping of a base input file columns into HED tags.
 
     Notes:
-        - Functions and type_variables column and row indexing starts at 0.
+        - All column numbers are 0 based.
     """
+
     def __init__(self, sidecar=None, tag_columns=None, column_prefix_dictionary=None,
-                 optional_tag_columns=None, requested_columns=None, warn_on_missing_column=False):
+                 optional_tag_columns=None, warn_on_missing_column=False):
         """ Constructor for ColumnMapper.
 
         Parameters:
             sidecar (Sidecar): A sidecar to gather column data from.
             tag_columns: (list):  A list of ints or strings containing the columns that contain the HED tags.
                 Sidecar column definitions will take precedent if there is a conflict with tag_columns.
-            column_prefix_dictionary (dict): Dictionary with keys that are column numbers and values are HED tag
+            column_prefix_dictionary (dict): Dictionary with keys that are column numbers/names and values are HED tag
                 prefixes to prepend to the tags in that column before processing.
             optional_tag_columns (list): A list of ints or strings containing the columns that contain
                 the HED tags. If the column is otherwise unspecified, convert this column type to HEDTags.
-            requested_columns (list or None): A list of columns you wish to retrieve.
-                If None, retrieve all columns.
             warn_on_missing_column (bool): If True, issue mapping warnings on column names that are missing from
                                             the sidecar.
 
         Notes:
-            - All column numbers are 0 based.
-
-        Examples:
-            column_prefix_dictionary = {3: 'Description/', 4: 'Label/'}
+            - All column numbers are 0 based.  
+            - The column_prefix_dictionary may be deprecated/renamed in the future.
+                - These are no longer prefixes, but rather converted to value columns:  
+                  {"key": "Description", 1: "Label/"} will turn into value columns as
+                  {"key": "Description/#", 1: "Label/#"}
+                  It will be a validation issue if column 1 is called "key" in the above example.
+                  This means it no longer accepts anything but the value portion only in the columns.
 
-            The third column contains tags that need Description/ tag prepended, while the fourth column
-            contains tag that needs Label/ prepended.
         """
-        # This points to column_type entries based on column names or indexes if columns have no column_name.
-        self.column_data = {}
+        
         # Maps column number to column_entry.  This is what's actually used by most code.
         self._final_column_map = {}
         self._no_mapping_info = True
 
         self._column_map = {}
         self._reverse_column_map = {}
-        self._requested_columns = []
         self._warn_on_missing_column = warn_on_missing_column
-        self._tag_columns = []
-        self._optional_tag_columns = []
-        self._column_prefix_dictionary = {}
+        if tag_columns is None:
+            tag_columns = []
+        self._tag_columns = tag_columns
+        if optional_tag_columns is None:
+            optional_tag_columns = []
+        self._optional_tag_columns = optional_tag_columns
+        if column_prefix_dictionary is None:
+            column_prefix_dictionary = {}
+        self._column_prefix_dictionary = column_prefix_dictionary
 
         self._na_patterns = ["n/a", "nan"]
-        self._finalize_mapping_issues = []
         self._sidecar = None
         self._set_sidecar(sidecar)
 
-        self.set_requested_columns(requested_columns, False)
-        self.set_tag_columns(tag_columns, optional_tag_columns, False)
-        self.set_column_prefix_dict(column_prefix_dictionary, False)
-
         # finalize the column map based on initial settings with no header
         self._finalize_mapping()
 
+    @property
+    def tag_columns(self):
+        """ Returns the known tag and optional tag columns with numbers as names when possible
+
+            Returns:
+                tag_columns(list of str or int): A list of all tag and optional tag columns as labels
+        """
+        joined_list = self._tag_columns + self._optional_tag_columns
+        return list(set(self._convert_to_names(self._column_map, joined_list)))
+
+    @property
+    def column_prefix_dictionary(self):
+        """ Returns the column_prefix_dictionary with numbers turned into names where possible
+
+            Returns:
+                column_prefix_dictionary(list of str or int): A column_prefix_dictionary with column labels as keys
+        """
+        return self._convert_to_names_dict(self._column_map, self._column_prefix_dictionary)
+
+    def get_transformers(self):
+        """ Return the transformers to use on a dataframe
+
+            Returns:
+                tuple(dict, list):
+                    dict({str or int: func}): the functions to use to transform each column
+                    need_categorical(list of int): a list of columns to treat as categoriacl
+        """
+        final_transformers = {}
+        need_categorical = []
+        for column in self._final_column_map.values():
+            assign_to_column = column.column_name
+            if isinstance(assign_to_column, int):
+                if self._column_map:
+                    assign_to_column = self._column_map[assign_to_column]
+                else:
+                    assign_to_column = assign_to_column
+            if column.column_type == ColumnType.Ignore:
+                continue
+            elif column.column_type == ColumnType.Value:
+                value_str = column.hed_dict
+                from functools import partial
+                final_transformers[assign_to_column] = partial(self._value_handler, value_str)
+            elif column.column_type == ColumnType.Categorical:
+                need_categorical.append(column.column_name)
+                category_values = column.hed_dict
+                from functools import partial
+                final_transformers[assign_to_column] = partial(self._category_handler, category_values)
+            else:
+                final_transformers[assign_to_column] = lambda x: x
+
+        return final_transformers, need_categorical
+
     @staticmethod
-    def validate_column_map(column_map, allow_blank_names):
-        """ Validate there are no issues with column names.
+    def check_for_blank_names(column_map, allow_blank_names):
+        """ Validate there are no blank column names
 
         Parameters:
             column_map(iterable): A list of column names
             allow_blank_names(bool): Only find issues if this is true
 
         Returns:
             issues(list): A list of dicts, one per issue.
         """
         # We don't have any checks right now if blank/duplicate is allowed
         if allow_blank_names:
             return []
+
         issues = []
-        used_names = set()
         for column_number, name in enumerate(column_map):
-            if name is None or name.startswith(PANDAS_COLUMN_PREFIX_TO_IGNORE):
+            if name is None or not name or name.startswith(PANDAS_COLUMN_PREFIX_TO_IGNORE):
                 issues += ErrorHandler.format_error(ValidationErrors.HED_BLANK_COLUMN, column_number)
                 continue
-            if name in used_names:
-                # todo: Add this check once it's more fleshed out
-                # issues += ErrorHandler.format_error(ValidationErrors.HED_DUPLICATE_COLUMN, name)
-                continue
-            used_names.add(name)
 
         return issues
 
     def _set_sidecar(self, sidecar):
         """ Set the sidecar this column mapper uses
 
         Parameters:
             sidecar (Sidecar or None): the sidecar to use
 
-        Returns:
-
+        :raises ValueError:
+            - A sidecar was prevoiusly set
         """
         if self._sidecar:
             raise ValueError("Trying to set a second sidecar on a column mapper.")
         if not sidecar:
             return None
-        for column_data in sidecar.column_data:
-            self._add_column_data(column_data)
 
         self._sidecar = sidecar
 
-    def get_tag_columns(self):
-        """ Returns the column numbers that are mapped to be HedTags
-
-            Note: This is NOT the tag_columns or optional_tag_columns parameter, though they set it.
+    @property
+    def sidecar_column_data(self):
+        """ Pass through to get the sidecar ColumnMetadata
 
         Returns:
-            column_numbers(list): A list of column numbers that are ColumnType.HedTags
+            dict({str:ColumnMetadata}): the column metadata defined by this sidecar
         """
-        return [number for number, column_entry in self._final_column_map.items()
-                if column_entry.column_type == ColumnType.HEDTags]
+        if self._sidecar:
+            return self._sidecar.column_data
 
-    def set_column_prefix_dict(self, column_prefix_dictionary, finalize_mapping=True):
-        """ Replace the column prefix dictionary
+        return {}
 
-        Parameters:
-            column_prefix_dictionary (dict):  Dictionary with keys that are column numbers and values are HED tag
-                prefixes to prepend to the tags in that column before processing.
-            finalize_mapping (bool): Re-generate the internal mapping if True, otherwise no effect until finalize.
+    def get_tag_columns(self):
+        """ Returns the column numbers or names that are mapped to be HedTags
 
-        Returns:
-            list:  List of issues that occurred during this process. Each issue is a dictionary.
+            Note: This is NOT the tag_columns or optional_tag_columns parameter, though they set it.
 
+        Returns:
+            column_identifiers(list): A list of column numbers or names that are ColumnType.HedTags.
+                0-based if integer-based, otherwise column name.
         """
-        if column_prefix_dictionary:
-            self._column_prefix_dictionary = column_prefix_dictionary
-        if finalize_mapping:
-            return self._finalize_mapping()
-        return []
+        return [column_entry.column_name for number, column_entry in self._final_column_map.items()
+                if column_entry.column_type == ColumnType.HEDTags]
 
     def set_tag_columns(self, tag_columns=None, optional_tag_columns=None, finalize_mapping=True):
         """ Set tag columns and optional tag columns
 
         Parameters:
             tag_columns (list): A list of ints or strings containing the columns that contain the HED tags.
                                 If None, clears existing tag_columns
             optional_tag_columns (list): A list of ints or strings containing the columns that contain the HED tags,
                                          but not an error if missing.
                                          If None, clears existing tag_columns
             finalize_mapping (bool): Re-generate the internal mapping if True, otherwise no effect until finalize.
-
-        Returns:
-            list: List of issues that occurred during this process. Each issue is a dictionary.
-
         """
         if tag_columns is None:
             tag_columns = []
         if optional_tag_columns is None:
             optional_tag_columns = []
         self._tag_columns = tag_columns
         self._optional_tag_columns = optional_tag_columns
         if finalize_mapping:
-            issues = self._finalize_mapping()
-            return issues
-        return []
-
-    def set_requested_columns(self, requested_columns, finalize_mapping=True):
-        """ Set to return only the columns listed in requested_columns
-
-        Parameters:
-            requested_columns(list or None): If this is not None, return ONLY these columns.  Names or numbers allowed.
-            finalize_mapping(bool): Finalize the mapping right now if True
-
-        Returns:
-        issues(list): An empty list of mapping issues
-        """
-        self._requested_columns = requested_columns
-        if finalize_mapping:
-            return self._finalize_mapping()
-        return []
+            self._finalize_mapping()
 
     def set_column_map(self, new_column_map=None):
         """ Set the column number to name mapping.
 
         Parameters:
             new_column_map (list or dict):  Either an ordered list of the column names or column_number:column name
                 dictionary. In both cases, column numbers start at 0
@@ -201,300 +217,201 @@
         if isinstance(new_column_map, dict):
             column_map = new_column_map
         # List like
         else:
             column_map = {column_number: column_name for column_number, column_name in enumerate(new_column_map)}
         self._column_map = column_map
         self._reverse_column_map = {column_name: column_number for column_number, column_name in column_map.items()}
-        return self._finalize_mapping()
-
-    def add_columns(self, column_names_or_numbers, column_type=ColumnType.HEDTags):
-        """ Add blank columns in the given column category.
-
-        Parameters:
-            column_names_or_numbers (list): A list of column names or numbers to add as the specified type.
-            column_type (ColumnType property): The category of column these should be.
-
-        """
-        if column_names_or_numbers:
-            if not isinstance(column_names_or_numbers, list):
-                column_names_or_numbers = [column_names_or_numbers]
-            for column_name in column_names_or_numbers:
-                new_def = ColumnMetadata(column_type, column_name)
-                self._add_column_data(new_def)
-
-    def _expand_column(self, column_number, input_text):
-        """ Expand the specified text based on the rules for expanding the specified column.
-
-        Parameters:
-            column_number (int): The column number this text should be treated as from.
-            input_text (str): The text to expand, generally from a single cell of a spreadsheet.
-
-        Returns:
-            str or None: The text after expansion or None if this column is undefined or the given text is null.
-            False or str: Depends on the value of first return value. If None, this is an error message.
-                If string, this is an attribute name that should be stored separately.
-
-        """
-
-        # Default 1-1 mapping if we don't have specific behavior.
-        if self._no_mapping_info:
-            return HedString(input_text), False
-
-        # If no entry, ignore this column.
-        if column_number not in self._final_column_map:
-            return None, False
-
-        if not input_text or input_text in self._na_patterns:
-            return None, False
-
-        column_entry = self._final_column_map[column_number]
-        return column_entry.expand(input_text)
-
-    def expand_row_tags(self, row_text):
-        """ Expand all mapped columns for row.
-
-        Parameters:
-            row_text (list): The text for the given row, one list entry per column number.
-
-        Returns:
-            dict: A dictionary containing the keys COLUMN_TO_HED_TAGS, COLUMN_ISSUES.
-
-        Notes:
-            - The "column_to_hed_tags" is each expanded column given separately as a list of HedStrings.
-            - Attributes are any column identified as an attribute.
-              They will appear in the return value as {attribute_name: value_of_column}
-
-        """
-        result_dict = {}
-        column_to_hed_tags_dictionary = {}
-        column_issues_dict = {}
-        for column_number, cell_text in enumerate(row_text):
-            translated_column, translation_errors = self._expand_column(column_number, str(cell_text))
-            if translated_column is None:
-                if translation_errors:
-                    if column_number not in column_issues_dict:
-                        column_issues_dict[column_number] = []
-                    column_issues_dict[column_number] += translation_errors
-                    column_to_hed_tags_dictionary[column_number] = translated_column
-                continue
-
-            column_to_hed_tags_dictionary[column_number] = translated_column
-
-        result_dict[model_constants.COLUMN_TO_HED_TAGS] = column_to_hed_tags_dictionary
-        if column_issues_dict:
-            result_dict[model_constants.COLUMN_ISSUES] = column_issues_dict
-
-        return result_dict
-
-    def get_prefix_remove_func(self, column_number):
-        """ Return a function to removes name prefixes for column
-
-        Parameters:
-            column_number (int): Column number to look up in the prefix dictionary.
-
-        Returns:
-            func: A function taking a tag and string, returning a string.
-
-        """
-        if column_number not in self._final_column_map:
-            return None
-
-        entry = self._final_column_map[column_number]
-        if not entry.column_prefix:
-            return None
-
-        return entry.remove_prefix
-
-    def _add_column_data(self, new_column_entry):
-        """ Add the metadata of a column to this column mapper.
-
-        Parameters:
-            new_column_entry (ColumnMetadata): The column definition to add.
-
-        Notes:
-            If an entry with the same name exists, the new entry will replace it.
-
-        """
-        column_name = new_column_entry.column_name
-        self.column_data[column_name] = copy.deepcopy(new_column_entry)
-
-    @staticmethod
-    def _set_column_prefix(final_map, column_number, new_required_prefix):
-        """ Internal function to add this as a required name_prefix to a column
-
-        Parameters:
-            final_map (dict): {column_number:prefix} Dict of column numbers with prefixes
-            column_number (int): The column number with this name_prefix.
-            new_required_prefix (str): The name_prefix to add to the column when loading from a spreadsheet.
-
-        Raises:
-            TypeError if column number is passed as a str rather an int.
-
-        Notes:
-            If the column is not known to the mapper, it will be added as a HEDTags column.
-
-        """
-        if isinstance(column_number, str):
-            raise TypeError("Must pass in a column number not column_name to _set_column_prefix")
-        if column_number not in final_map:
-            column_entry = ColumnMetadata(ColumnType.HEDTags)
-            final_map[column_number] = column_entry
-        else:
-            column_entry = final_map[column_number]
+        self._finalize_mapping()
 
-        column_entry.column_prefix = new_required_prefix
-        if column_entry.column_type is None or column_entry.column_type == ColumnType.Ignore:
-            column_entry.column_type = ColumnType.HEDTags
+    def set_column_prefix_dictionary(self, column_prefix_dictionary, finalize_mapping=True):
+        """Sets the column prefix dictionary"""
+        self._column_prefix_dictionary = column_prefix_dictionary
+        if finalize_mapping:
+            self._finalize_mapping()
 
     @staticmethod
-    def _get_basic_final_map(column_map, column_data):
+    def _get_sidecar_basic_map(column_map, column_data):
         basic_final_map = {}
-        unhandled_names = {}
+        unhandled_cols = []
         if column_map:
             for column_number, column_name in column_map.items():
                 if column_name is None:
                     continue
                 if column_name in column_data:
                     column_entry = copy.deepcopy(column_data[column_name])
                     column_entry.column_name = column_name
-                    basic_final_map[column_number] = column_entry
+                    basic_final_map[column_name] = column_entry
                     continue
-                elif column_name.startswith(PANDAS_COLUMN_PREFIX_TO_IGNORE):
+                elif isinstance(column_name, str) and column_name.startswith(PANDAS_COLUMN_PREFIX_TO_IGNORE):
                     continue
-                unhandled_names[column_name] = column_number
-        for column_number in column_data:
-            if isinstance(column_number, int):
-                column_entry = copy.deepcopy(column_data[column_number])
-                column_entry.column_name = column_number
-                basic_final_map[column_number] = column_entry
+                unhandled_cols.append(column_name)
 
-        return basic_final_map, unhandled_names
+        return basic_final_map, unhandled_cols
 
     @staticmethod
-    def _convert_to_indexes(name_to_column_map, column_list):
-        converted_indexes = []
-        unknown_names = []
-        for name in column_list:
-            if isinstance(name, str):
-                if name in name_to_column_map:
-                    converted_indexes.append(name_to_column_map[name])
-                    continue
-                else:
-                    unknown_names.append(name)
+    def _convert_to_names(column_to_name_map, column_list):
+        converted_names = []
+        for index in column_list:
+            if isinstance(index, int):
+                if not column_to_name_map:
+                    converted_names.append(index)
+                elif index in column_to_name_map:
+                    converted_names.append(column_to_name_map[index])
             else:
-                # Name is in int here
-                converted_indexes.append(name)
-        return converted_indexes, unknown_names
+                if index in column_to_name_map.values():
+                    converted_names.append(index)
+        return converted_names
 
     @staticmethod
-    def _add_tag_columns(final_map, unhandled_names, all_tag_columns, required_tag_columns, warn_on_missing_columns):
-        issues = []
-
-        # Add numbered tag columns
-        for column_name, column_number in unhandled_names.items():
-            if column_number in all_tag_columns:
-                final_map[column_number] = ColumnMetadata(ColumnType.HEDTags, column_name)
+    def _convert_to_names_dict(column_to_name_map, column_dict):
+        converted_dict = {}
+        for index, column_data in column_dict.items():
+            if isinstance(index, int):
+                if not column_to_name_map:
+                    converted_dict[index] = column_data
+                elif index in column_to_name_map:
+                    converted_dict[column_to_name_map[index]] = column_data
             else:
-                if warn_on_missing_columns and column_number not in required_tag_columns:
-                    issues += ErrorHandler.format_error(ValidationErrors.HED_UNKNOWN_COLUMN,
-                                                        column_name=column_name)
-
-        # Add numbered tag columns
-        for column_name_or_number in all_tag_columns:
-            if isinstance(column_name_or_number, int):
-                if column_name_or_number not in final_map:
-                    final_map[column_name_or_number] = ColumnMetadata(ColumnType.HEDTags,
-                                                                      column_name_or_number)
-
-        # Switch any tag/requested columns to be HedTags if they were being ignored
-        for column_number, entry in final_map.items():
-            if column_number in all_tag_columns and entry.column_type == ColumnType.Ignore:
-                entry.column_type = ColumnType.HEDTags
-
-        return issues
+                if index in column_to_name_map.values():
+                    converted_dict[index] = column_data
+        return converted_dict
 
     @staticmethod
-    def _filter_by_requested(final_map, requested_columns):
-        if requested_columns is not None:
-            return {key: value for key, value in final_map.items()
-                    if key in requested_columns or value.column_name in requested_columns}
-        return final_map
+    def _add_value_columns(final_map, column_prefix_dictionary):
+        for col, prefix in column_prefix_dictionary.items():
+            if prefix.endswith("/"):
+                prefix = prefix + "#"
+            else:
+                prefix = prefix + "/#"
+            new_def = ColumnMetadata(ColumnType.Value, col, source=prefix)
+            final_map[col] = new_def
 
     @staticmethod
-    def _convert_tag_columns(tag_columns, optional_tag_columns, requested_columns, reverse_column_map):
-        all_tag_columns = tag_columns + optional_tag_columns
-        required_tag_columns = tag_columns.copy()
-        if requested_columns:
-            all_tag_columns += requested_columns
-            required_tag_columns += requested_columns
-
-        all_tag_columns, _ = ColumnMapper._convert_to_indexes(reverse_column_map, all_tag_columns)
-        required_tag_columns, missing_tag_column_names = ColumnMapper._convert_to_indexes(reverse_column_map,
-                                                                                          required_tag_columns)
+    def _add_tag_columns(final_map, tag_columns):
+        for col in tag_columns:
+            new_def = ColumnMetadata(ColumnType.HEDTags, col)
+            final_map[col] = new_def
+
+    def _get_column_lists(self):
+        column_lists = self._tag_columns, self._optional_tag_columns, self._column_prefix_dictionary
+        list_names = ["tag_columns", "optional_tag_columns", "column_prefix_dictionary"]
+
+        if not any(column for column in column_lists):
+            return column_lists, list_names
+        # Filter out empty lists from the above
+        column_lists, list_names = zip(*[(col_list, list_name) for col_list, list_name in zip(column_lists, list_names)
+                                         if col_list])
 
+        return column_lists, list_names
+
+    def _check_for_duplicates_and_required(self, list_names, column_lists):
         issues = []
-        for column_name in missing_tag_column_names:
-            issues += ErrorHandler.format_error(ValidationErrors.HED_MISSING_REQUIRED_COLUMN,
-                                                column_name=column_name)
+        for list_name, col_list in zip(list_names, column_lists):
+            # Convert all known strings to ints, then check for duplicates
+            converted_list = [item if isinstance(item, int) else self._reverse_column_map.get(item, item)
+                              for item in col_list]
+
+            if col_list != self._optional_tag_columns:
+                for test_col in converted_list:
+                    if isinstance(test_col, str) and test_col not in self._reverse_column_map:
+                        issues += ErrorHandler.format_error(ValidationErrors.HED_MISSING_REQUIRED_COLUMN,
+                                                            test_col, list_name)
 
-        return all_tag_columns, required_tag_columns, issues
+            issues += self._check_for_duplicates_between_lists(converted_list, list_name,
+                                                               ValidationErrors.DUPLICATE_COLUMN_IN_LIST)
 
-    def _finalize_mapping(self):
-        # 1. All named and numbered columns are located from sidecars and put in final mapping
-        # 2. Add any tag columns and note issues about missing columns
-        # 3. Add any numbered columns that have required prefixes
-        # 4. Filter to just requested columns, if any
-        final_map, unhandled_names = self._get_basic_final_map(self._column_map, self.column_data)
-
-        # convert all tag lists to indexes -> Issuing warnings at this time potentially for unknown ones
-        all_tag_columns, required_tag_columns, issues = self._convert_tag_columns(self._tag_columns,
-                                                                                  self._optional_tag_columns,
-                                                                                  self._requested_columns,
-                                                                                  self._reverse_column_map)
-
-        # Notes any missing required columns
-        issues += self._add_tag_columns(final_map, unhandled_names, all_tag_columns, required_tag_columns,
-                                        self._warn_on_missing_column)
-
-        # Add prefixes
-        for column_number, prefix in self._column_prefix_dictionary.items():
-            self._set_column_prefix(final_map, column_number, prefix)
+        return issues
+
+    def _check_for_duplicates_between_lists(self, checking_list, list_names, error_type):
+        issues = []
+        duplicates = [item for item, count in Counter(checking_list).items() if count > 1]
+        for duplicate in duplicates:
+            issues += ErrorHandler.format_error(error_type, duplicate,
+                                                self._column_map.get(duplicate), list_names)
+        return issues
+
+    def check_for_mapping_issues(self, allow_blank_names=False):
+        """ Find all issues given the current column_map, tag_columns, etc.
+
+        Parameters:
+            allow_blank_names(bool): Only flag blank names if False
+
+        Returns:
+            issue_list(list of dict): Returns all issues found as a list of dicts
+        """
+        # 1. Get the lists with entries
+        column_lists, list_names = self._get_column_lists()
+        # 2. Verify column_prefix columns and tag columns are present, and check for duplicates
+        issues = self._check_for_duplicates_and_required(list_names, column_lists)
+
+        combined_list = self.tag_columns + list(self.column_prefix_dictionary)
+        # 3. Verify prefix and tag columns do not conflict.
+        issues += self._check_for_duplicates_between_lists(combined_list, list_names,
+                                                           ValidationErrors.DUPLICATE_COLUMN_BETWEEN_SOURCES)
 
-        issues += ColumnMapper.validate_column_map(self._column_map.values(), allow_blank_names=False)
+        # 4. Verify we didn't get both a sidecar and a tag column list
+        if self._sidecar and combined_list and combined_list != ["HED"]:
+            issues += ErrorHandler.format_error(ValidationErrors.SIDECAR_AND_OTHER_COLUMNS, column_names=combined_list)
 
-        self._final_column_map = self._filter_by_requested(final_map, self._requested_columns)
+        # 5. Verify we handled all columns
+        if self._warn_on_missing_column:
+            fully_combined_list = list(self.sidecar_column_data) + combined_list
+            for column in self._column_map.values():
+                if column not in fully_combined_list:
+                    issues += ErrorHandler.format_error(ValidationErrors.HED_UNKNOWN_COLUMN, column)
 
-        self._no_mapping_info = not self._check_if_mapping_info()
-        self._finalize_mapping_issues = issues
+        issues += self.check_for_blank_names(self._column_map.values(), allow_blank_names=allow_blank_names)
         return issues
 
-    def _check_if_mapping_info(self):
-        # If any of these have any data, don't do default behavior.
-        return bool(self.column_data or self._final_column_map
-                    or self._requested_columns is not None or self._tag_columns
-                    or self._optional_tag_columns or self._column_prefix_dictionary)
-
-    def _column_name_requested(self, column_name):
-        if self._requested_columns is None:
-            return True
-        return column_name in self._requested_columns
+    def _finalize_mapping(self):
+        final_map, unhandled_cols = self._get_sidecar_basic_map(self._column_map, self.sidecar_column_data)
+
+        self._add_tag_columns(final_map, self.tag_columns)
+        self._remove_from_list(unhandled_cols, self.tag_columns)
+
+        self._add_value_columns(final_map, self.column_prefix_dictionary)
+        self._remove_from_list(unhandled_cols, self.column_prefix_dictionary)
 
-    def get_def_dicts(self):
+        self._final_column_map = dict(sorted(final_map.items()))
+
+    @staticmethod
+    def _remove_from_list(list_to_alter, to_remove):
+        return [item for item in list_to_alter if item not in to_remove]
+
+    def get_def_dict(self, hed_schema=None, extra_def_dicts=None):
         """ Return def dicts from every column description.
 
-        Returns:
-           list:   A list of DefinitionDict objects corresponding to each column entry.
+        Parameters:
+            hed_schema (Schema or None): A HED schema object to use for extracting definitions.
+            extra_def_dicts (list, DefinitionDict, or None): Extra dicts to add to the list.
 
+        Returns:
+           DefinitionDict:   A single definition dict representing all the data(and extra def dicts)
         """
         if self._sidecar:
-            return self._sidecar.get_def_dicts()
+            return self._sidecar.get_def_dict(hed_schema=hed_schema, extra_def_dicts=extra_def_dicts)
+
         return []
 
     def get_column_mapping_issues(self):
-        """ Get all the issues with finalizing column mapping.  Primarily a missing required column.
+        """ Get all the issues with finalizing column mapping(duplicate columns, missing required, etc)
+
+        Notes:
+            - This is deprecated and now a wrapper for "check_for_mapping_issues()"
 
         Returns:
             list: A list dictionaries of all issues found from mapping column names to numbers.
 
         """
-        return self._finalize_mapping_issues
+        return self.check_for_mapping_issues()
+
+    @staticmethod
+    def _category_handler(category_values, x):
+        return category_values.get(x, "")
+
+    @staticmethod
+    def _value_handler(value_str, x):
+        if x == "n/a":
+            return "n/a"
+
+        return value_str.replace("#", str(x))
```

### Comparing `hedtools-0.2.0/hed/models/definition_entry.py` & `hedtools-0.3.0/hed/models/definition_entry.py`

 * *Files 27% similar despite different names*

```diff
@@ -14,77 +14,56 @@
             name (str):            The label portion of this name (not including Definition/).
             contents (HedGroup):   The contents of this definition.
             takes_value (bool):    If True, expects ONE tag to have a single # sign in it.
             source_context (list, None): List (stack) of dictionaries giving context for reporting errors.
         """
         self.name = name
         if contents:
-            contents = contents.copy()
+            contents = contents.copy().sort()
         self.contents = contents
         self.takes_value = takes_value
         self.source_context = source_context
-        self.tag_dict = {}
-        if contents:
-            add_group_to_dict(contents, self.tag_dict)
 
-    def get_definition(self, replace_tag, placeholder_value=None):
+    def get_definition(self, replace_tag, placeholder_value=None, return_copy_of_tag=False):
         """ Return a copy of the definition with the tag expanded and the placeholder plugged in.
 
+            Returns None if placeholder_value passed when it doesn't take value, or vice versa.
+
         Parameters:
             replace_tag (HedTag): The def hed tag to replace with an expanded version
             placeholder_value (str or None):    If present and required, will replace any pound signs
                                                 in the definition contents.
+            return_copy_of_tag(bool): Set to true for validation
 
         Returns:
-            str:          The expanded def tag name
-            HedGroup:     The contents of this definition(including the def tag itself)
-
-        Raises:
-            ValueError:  If a placeholder_value is passed, but this definition doesn't have a placeholder.
+            tuple:
+                str:          The expanded def tag name
+                HedGroup:     The contents of this definition(including the def tag itself)
 
+        :raises ValueError:
+            - Something internally went wrong with finding the placeholder tag.  This should not be possible.
         """
         if self.takes_value == (placeholder_value is None):
             return None, []
 
+        if return_copy_of_tag:
+            replace_tag = replace_tag.copy()
         output_contents = [replace_tag]
         name = self.name
         if self.contents:
             output_group = self.contents
-            if placeholder_value:
+            if placeholder_value is not None:
                 output_group = copy.deepcopy(self.contents)
                 placeholder_tag = output_group.find_placeholder_tag()
                 if not placeholder_tag:
                     raise ValueError("Internal error related to placeholders in definition mapping")
                 name = f"{name}/{placeholder_value}"
                 placeholder_tag.replace_placeholder(placeholder_value)
 
             output_contents = [replace_tag, output_group]
 
         output_contents = HedGroup(replace_tag._hed_string,
                                    startpos=replace_tag.span[0], endpos=replace_tag.span[1], contents=output_contents)
         return f"{DefTagNames.DEF_EXPAND_ORG_KEY}/{name}", output_contents
 
-
-def add_group_to_dict(group, tag_dict=None):
-    """ Add the tags and their values from a HED group to a tag dictionary.
-
-    Parameters:
-        group (HedGroup):   Contents to add to the tag dict.
-        tag_dict (dict):    The starting tag dictionary to add to.
-
-    Returns:
-        dict:  The updated tag_dict containing the tags with a list of values.
-
-    Notes:
-        - Expects tags to have forms calculated already.
-
-    """
-    if tag_dict is None:
-        tag_dict = {}
-    for tag in group.get_all_tags():
-        short_base_tag = tag.short_base_tag
-        value = tag.extension_or_value_portion
-        value_dict = tag_dict.get(short_base_tag, {})
-        if value:
-            value_dict[value] = ''
-        tag_dict[short_base_tag] = value_dict
-    return tag_dict
+    def __str__(self):
+        return str(self.contents)
```

### Comparing `hedtools-0.2.0/hed/models/expression_parser.py` & `hedtools-0.3.0/hed/models/expression_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import re
 
 
-# todo: Add support for early outs with and(only try to match groups we already matched instead of all groups)
 class search_result:
     def __init__(self, group, tag):
         self.group = group
         # todo: rename tag: children
         if not isinstance(tag, list):
             new_tags = [tag]
         else:
@@ -175,28 +174,27 @@
                         if merged_result.has_same_tags(finalized_value):
                             dont_add = True
                             break
                     if dont_add:
                         continue
                     return_list.append(merged_result)
 
-        # finally simplify the list and remove duplicates.
-
         return return_list
 
     def __str__(self):
         output_str = "("
         if self.left:
             output_str += str(self.left)
         output_str += " " + str(self.token)
         if self.right:
             output_str += str(self.right)
         output_str += ")"
         return output_str
 
+
 class ExpressionWildcardNew(Expression):
     def handle_expr(self, hed_group, exact=False):
         groups_found = []
         if self.token.text == "?":
             # Any tag or group
             groups_searching = hed_group.get_all_groups()
             for group in groups_searching:
```

### Comparing `hedtools-0.2.0/hed/models/hed_group.py` & `hedtools-0.3.0/hed/models/hed_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,18 +9,15 @@
         """ Return an empty HedGroup object.
 
         Parameters:
             hed_string (str or None): Source hed string for this group.
             startpos (int or None):   Starting index of group(including parentheses) in hed_string.
             endpos (int or None):     Position after the end (including parentheses) in hed_string.
             contents (list or None):  A list of HedTags and/or HedGroups that will be set as the contents of this group.
-
-        Notes:
-            - contents parameter is mainly used for processing definitions.
-
+                                      Mostly used during definition expansion.
         """
         self._startpos = startpos
         self._endpos = endpos
         self._hed_string = hed_string
         self._parent = None
 
         if contents:
@@ -32,18 +29,14 @@
         self._original_children = self._children
 
     def append(self, tag_or_group):
         """ Add a tag or group to this group.
 
         Parameters:
             tag_or_group (HedTag or HedGroup): The new object to add to this group.
-
-        Raises:
-            ValueError: If a HedGroupFrozen.
-
         """
         tag_or_group._parent = self
         self._children.append(tag_or_group)
 
     def check_if_in_original(self, tag_or_group):
         """ Check if the tag or group in original string.
 
@@ -68,14 +61,16 @@
     def replace(self, item_to_replace, new_contents):
         """ Replace an existing tag or group.
 
         Parameters:
             item_to_replace (HedTag or HedGroup): The item to replace must exist or this will raise an error.
             new_contents (HedTag or HedGroup): Replacement contents.
 
+        :raises KeyError:
+            - item_to_replace does not exist
         """
         if self._original_children is self._children:
             self._original_children = self._children.copy()
 
         replace_index = -1
         for i, child in enumerate(self._children):
             if item_to_replace is child:
@@ -84,32 +79,23 @@
         self._children[replace_index] = new_contents
         new_contents._parent = self
 
     def remove(self, items_to_remove):
         """ Remove any tags/groups in items_to_remove.
 
         Parameters:
-            items_to_remove (list):  List of HedGroups and/or HedTags to remove.
+            items_to_remove (list):  List of HedGroups and/or HedTags to remove by identity.
 
         Notes:
             - Any groups that become empty will also be pruned.
-            - Identity, not equivalence is used in determining whether to remove.
-
         """
         all_groups = self.get_all_groups()
         self._remove(items_to_remove, all_groups)
 
     def _remove(self, items_to_remove, all_groups):
-        """ Needs to be documented.
-
-        Parameters:
-            items_to_remove (list):  List of HedGroups and/or HedTags to remove.
-            all_groups (list):   List of HedGroups.
-
-        """
         empty_groups = []
         for remove_child in items_to_remove:
             for group in all_groups:
                 # only proceed if we have an EXACT match for this child
                 if any(remove_child is child for child in group._children):
                     if group._original_children is group._children:
                         group._original_children = group._children.copy()
@@ -128,17 +114,14 @@
 
     def copy(self):
         """ Return a deep copy of this group.
 
         Returns:
             HedGroup: The copied group.
 
-        Notes:
-            - The parent tag is removed.
-
         """
         save_parent = self._parent
         self._parent = None
         return_copy = copy.deepcopy(self)
         self._parent = save_parent
         return return_copy
 
@@ -156,23 +139,26 @@
 
         Parameters:
             update_self (bool): If True, update the contents of this group to be sorted as well.
 
         Returns:
             list: The list of all tags in this group, with subgroups being returned as further nested lists
         """
-        output_list = []
+        tag_list = []
+        group_list = []
         queue_list = list(self.children)
         for child in queue_list:
             if isinstance(child, HedTag):
-                output_list.append((child, child))
+                tag_list.append((child, child))
             else:
-                output_list.append((child, child.sorted(update_self)))
+                group_list.append((child, child.sorted(update_self)))
 
-        output_list.sort(key=lambda x: str(x[0]))
+        tag_list.sort(key=lambda x: str(x[0]))
+        group_list.sort(key=lambda x: str(x[0]))
+        output_list = tag_list + group_list
         if update_self:
             self._children = [x[0] for x in output_list]
         return [x[1] for x in output_list]
 
     @property
     def children(self):
         """ A list of the direct children. """
@@ -259,14 +245,27 @@
 
         Returns:
             list: All groups directly in this group, filtering out HedTag children.
 
         """
         return [group for group in self.children if isinstance(group, HedGroup)]
 
+    def get_first_group(self):
+        """ Returns the first group in this hed string or group.
+
+            Useful for things like Def-expand where they only have a single group.
+
+            Raises a ValueError if there are no groups.
+
+        Returns:
+            HedGroup: The first group
+
+        """
+        return self.groups()[0]
+
     def get_original_hed_string(self):
         """ Get the original hed string.
 
         Returns:
             str: The original string with no modification.
 
         """
@@ -308,35 +307,25 @@
 
         Returns:
             str: The group as a string with all tags as long tags.
 
         """
         return self.get_as_form("long_tag")
 
-    def get_as_form(self, tag_attribute, tag_transformer=None):
+    def get_as_form(self, tag_attribute):
         """ Get the string corresponding to the specified form.
 
         Parameters:
             tag_attribute (str): The hed_tag property to use to construct the string (usually short_tag or long_tag).
-            tag_transformer (func or None): A function that is applied to each tag string before returning.
 
         Returns:
             str: The constructed string after transformation
-
-        Notes:
-            - The signature of a tag_transformer is str def(HedTag, str).
-
         """
-        if tag_transformer:
-            result = ",".join([tag_transformer(child, child.__getattribute__(tag_attribute))
-                               if isinstance(child, HedTag) else child.get_as_form(tag_attribute, tag_transformer)
-                               for child in self.children])
-        else:
-            result = ",".join([child.__getattribute__(tag_attribute) if isinstance(child, HedTag) else
-                               child.get_as_form(tag_attribute) for child in self.children])
+        result = ",".join([child.__getattribute__(tag_attribute) if isinstance(child, HedTag) else
+                           child.get_as_form(tag_attribute) for child in self.children])
         if self.is_group:
             return f"({result})"
         return result
 
     def lower(self):
         """ Convenience function, equivalent to str(self).lower() """
         return str(self).lower()
@@ -345,30 +334,38 @@
         """ Return a placeholder tag, if present in this group.
 
         Returns:
             HedTag or None: The placeholder tag if found.
 
         Notes:
             - Assumes a valid HedString with no erroneous "#" characters.
-
         """
         for tag in self.get_all_tags():
-            if "#" in tag.org_tag:
+            if tag.is_placeholder():
                 return tag
 
         return None
 
     def __bool__(self):
         return bool(self._children)
 
     def __eq__(self, other):
-        """ Test whether other is equal to this object. """
+        """ Test whether other is equal to this object.
+
+            Note: This does not account for sorting.  Objects must be in the same order to match.
+        """
         if self is other:
             return True
 
+        # Allow us to compare to a list of groups.
+        # Note this comparison will NOT check if the list has the outer parenthesis
+        if isinstance(other, list):
+            return self.children == other
+        if isinstance(other, str):
+            return str(self) == other
         if not isinstance(other, HedGroup) or self.children != other.children or self.is_group != other.is_group:
             return False
         return True
 
     def find_tags(self, search_tags, recursive=False, include_groups=2):
         """ Find the tags and their containing groups.
 
@@ -406,25 +403,24 @@
     def find_wildcard_tags(self, search_tags, recursive=False, include_groups=2):
         """ Find the tags and their containing groups.
 
         Parameters:
             search_tags (container):    A container of the starts of short tags to search.
             recursive (bool):           If true, also check subgroups.
             include_groups (0, 1 or 2): Specify return values.
+                If 0: return a list of the HedTags.
+                If 1: return a list of the HedGroups containing the HedTags.
+                If 2: return a list of tuples (HedTag, HedGroup) for the found tags.
 
         Returns:
             list: The contents of the list depends on the value of include_groups.
 
         Notes:
-            - If include_groups is 0, return a list of the HedTags.
-            - If include_groups is 1, return a list of the HedGroups containing the HedTags.
-            - If include_groups is 2, return a list of tuples (HedTag, HedGroup) for the found tags.
             - This can only find identified tags.
             - By default, definition, def, def-expand, onset, and offset are identified, even without a schema.
-
         """
         found_tags = []
         if recursive:
             groups = self.get_all_groups()
         else:
             groups = (self, )
 
@@ -452,19 +448,14 @@
             list: A list of HedGroups the given tags/groups were found in.
 
         Notes:
             - If you pass in groups it will only find EXACT matches.
             - This can only find identified tags.
             - By default, definition, def, def-expand, onset, and offset are identified, even without a schema.
             - If this is a HedGroup, order matters.  (b, a) != (a, b)
-            - If this is a HedGroupFrozen:
-                    if "(a, b)" in tags_or_groups, then it will match 1 and 2, but not 3.
-                        1. (a, b)
-                        2. (b, a)
-                        3. (a, b, c)
 
         """
         found_tags = []
         if recursive:
             groups = self.get_all_groups()
         else:
             groups = (self,)
@@ -478,65 +469,62 @@
         if include_groups == 0 or include_groups == 1:
             return [tag[include_groups] for tag in found_tags]
 
         return found_tags
 
     def find_def_tags(self, recursive=False, include_groups=3):
         """ Find def and def-expand tags
+
         Parameters:
             recursive (bool): If true, also check subgroups.
-            include_groups (int, 0, 1, 2, 3): options for how to expand or include groups
+            include_groups (int, 0, 1, 2, 3): options for return values
+                If 0: Return only def and def expand tags/.
+                If 1: Return only def tags and def-expand groups.
+                If 2: Return only groups containing defs, or def-expand groups.
+                If 3 or any other value: Return all 3 as a tuple.
         Returns:
-            list: A list of tuples. The contents depends on the values of the include group.
-        Notes:
-            - The include_groups option controls the tag expansion as follows:
-                - If 0: Return only def and def expand tags/.
-                - If 1: Return only def tags and def-expand groups.
-                - If 2: Return only groups containing defs, or def-expand groups.
-                - If 3 or any other value: Return all 3 as a tuple.
+            list: A list of tuples. The contents depend on the values of the include_group.
         """
         from hed.models.definition_dict import DefTagNames
         if recursive:
             groups = self.get_all_groups()
         else:
             groups = (self, )
 
         def_tags = []
         for group in groups:
             for child in group.children:
                 if isinstance(child, HedTag):
-                    if child.short_base_tag.lower() == DefTagNames.DEF_KEY:
+                    if child.short_base_tag == DefTagNames.DEF_ORG_KEY:
                         def_tags.append((child, child, group))
                 else:
                     for tag in child.tags():
-                        if tag.short_base_tag.lower() == DefTagNames.DEF_EXPAND_KEY:
+                        if tag.short_base_tag == DefTagNames.DEF_EXPAND_ORG_KEY:
                             def_tags.append((tag, child, group))
 
         if include_groups == 0 or include_groups == 1 or include_groups == 2:
             return [tag[include_groups] for tag in def_tags]
         return def_tags
 
     def find_tags_with_term(self, term, recursive=False, include_groups=2):
         """  Find any tags that contain the given term.
 
             Note: This can only find identified tags.
 
         Parameters:
             term (str): A single term to search for.
             recursive (bool): If true, recursively check subgroups.
-            include_groups: 0, 1 or 2
+            include_groups(0, 1 or 2): Controls return values
                 If 0: Return only tags
                 If 1: Return only groups
                 If 2 or any other value: Return both
 
         Returns:
             list:
-
         """
-
         found_tags = []
         if recursive:
             groups = self.get_all_groups()
         else:
             groups = (self,)
 
         search_for = term.lower()
```

### Comparing `hedtools-0.2.0/hed/models/hed_string.py` & `hedtools-0.3.0/hed/models/hed_string.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 """
 This module is used to split tags in a HED string.
 """
 from hed.models.hed_group import HedGroup
 from hed.models.hed_tag import HedTag
-from hed.errors.error_reporter import ErrorHandler, check_for_any_errors
-from hed.errors.error_types import ErrorContext
-from hed.models.hed_ops import translate_ops
 from hed.models.model_constants import DefTagNames
 
 
 class HedString(HedGroup):
     """ A HED string. """
 
     OPENING_GROUP_CHARACTER = '('
     CLOSING_GROUP_CHARACTER = ')'
 
-    def __init__(self, hed_string, hed_schema=None, _contents=None):
+    def __init__(self, hed_string, hed_schema=None, def_dict=None, _contents=None):
         """ Constructor for the HedString class.
 
         Parameters:
             hed_string (str): A HED string consisting of tags and tag groups.
             hed_schema (HedSchema or None): The schema to use to identify tags.  Can be passed later.
             _contents ([HedGroup and/or HedTag] or None): Create a HedString from this exact list of children.
                                                               Does not make a copy.
@@ -28,15 +25,15 @@
 
         """
 
         if _contents is not None:
             contents = _contents
         else:
             try:
-                contents = self.split_into_groups(hed_string, hed_schema)
+                contents = self.split_into_groups(hed_string, hed_schema, def_dict)
             except ValueError:
                 contents = []
         super().__init__(hed_string, contents=contents, startpos=0, endpos=len(hed_string))
 
     @classmethod
     def from_hed_strings(cls, contents):
         """ Factory for creating HedStrings via combination.
@@ -55,18 +52,16 @@
     def is_group(self):
         """ Always False since the underlying string is not a group with parentheses. """
         return False
 
     def convert_to_canonical_forms(self, hed_schema):
         """ Identify all tags using the given schema.
 
-            If schema is None, still identify "key" tags such as definitions.
-
         Parameters:
-            hed_schema (HedSchema, HedSchemaGroup, None): The schema to use to validate/convert tags.
+            hed_schema (HedSchema, HedSchemaGroup): The schema to use to validate/convert tags.
 
         Returns:
             list: A list of issues found while converting the string. Each issue is a dictionary.
 
         """
         validation_issues = []
         for tag in self.get_all_tags():
@@ -74,24 +69,58 @@
 
         return validation_issues
 
     def remove_definitions(self):
         """ Remove definition tags and groups from this string.
 
             This does not validate definitions and will blindly removing invalid ones as well.
-
-        Returns:
-            list: An empty list as there are no possible issues, this list is always blank.
-
         """
         definition_groups = self.find_top_level_tags({DefTagNames.DEFINITION_KEY}, include_groups=1)
         if definition_groups:
             self.remove(definition_groups)
 
-        return []
+    def shrink_defs(self):
+        """ Replace def-expand tags with def tags
+
+            This does not validate them and will blindly shrink invalid ones as well.
+
+        Returns:
+            self
+        """
+        for def_expand_tag, def_expand_group in self.find_tags({DefTagNames.DEF_EXPAND_KEY}, recursive=True):
+            expanded_parent = def_expand_group._parent
+            if expanded_parent:
+                def_expand_tag.short_base_tag = DefTagNames.DEF_ORG_KEY
+                def_expand_tag._parent = expanded_parent
+                expanded_parent.replace(def_expand_group, def_expand_tag)
+
+        return self
+
+    def expand_defs(self):
+        """ Replace def tags with def-expand tags
+
+            This does very minimal validation
+
+        Returns:
+            self
+        """
+        def_tags = self.find_def_tags(recursive=True, include_groups=0)
+
+        replacements = []
+        for tag in def_tags:
+            if tag.expandable and not tag.expanded:
+                replacements.append((tag, tag.expandable))
+
+        for tag, group in replacements:
+            tag_parent = tag._parent
+            tag_parent.replace(tag, group)
+            tag._parent = group
+            tag.short_base_tag = DefTagNames.DEF_EXPAND_KEY
+
+        return self
 
     def convert_to_short(self, hed_schema):
         """ Compute canonical forms and return the short form.
 
         Parameters:
             hed_schema (HedSchema or None): The schema to use to calculate forms.
 
@@ -136,37 +165,36 @@
         Notes:
             Potentially with some extraneous spaces removed on returned string.
 
         """
         return self.get_as_form("org_tag")
 
     @staticmethod
-    def split_into_groups(hed_string, hed_schema=None):
+    def split_into_groups(hed_string, hed_schema=None, def_dict=None):
         """ Split the HED string into a parse tree.
 
         Parameters:
             hed_string (str): A hed string consisting of tags and tag groups to be processed.
-            hed_schema (HedSchema or None): Hed schema to use to identify tags.
-
+            hed_schema (HedSchema or None): HED schema to use to identify tags.
+            def_dict(DefinitionDict): The definitions to identify
         Returns:
             list:  A list of HedTag and/or HedGroup.
 
-        Raises:
-            ValueError: If the string is significantly malformed, such as mismatched parentheses.
+        :raises ValueError:
+            - The string is significantly malformed, such as mismatched parentheses.
 
         Notes:
             - The parse tree consists of tag groups, tags, and delimiters.
         """
-
         current_tag_group = [[]]
 
         input_tags = HedString.split_hed_string(hed_string)
         for is_hed_tag, (startpos, endpos) in input_tags:
             if is_hed_tag:
-                new_tag = HedTag(hed_string, (startpos, endpos), hed_schema)
+                new_tag = HedTag(hed_string, (startpos, endpos), hed_schema, def_dict)
                 current_tag_group[-1].append(new_tag)
             else:
                 string_portion = hed_string[startpos:endpos]
                 delimiter_index = 0
                 for i, char in enumerate(string_portion):
                     if not char.isspace():
                         delimiter_index = i
@@ -174,14 +202,16 @@
 
                 delimiter_char = string_portion[delimiter_index]
 
                 if delimiter_char is HedString.OPENING_GROUP_CHARACTER:
                     current_tag_group.append(HedGroup(hed_string, startpos + delimiter_index))
 
                 if delimiter_char is HedString.CLOSING_GROUP_CHARACTER:
+                    # if prev_delimiter == ",":
+                    #     raise ValueError(f"Closing parentheses in hed string {hed_string}")
                     # Terminate existing group, and save it off.
                     paren_end = startpos + delimiter_index + 1
 
                     if len(current_tag_group) > 1:
                         new_group = current_tag_group.pop()
                         new_group._endpos = paren_end
 
@@ -278,85 +308,58 @@
             # view_string = hed_string[tag_start_pos: len(hed_string)]
             result_positions.append((True, (tag_start_pos, len(hed_string) - current_spacing)))
             if current_spacing:
                 result_positions.append((False, (len(hed_string) - current_spacing, len(hed_string))))
 
         return result_positions
 
-    def apply_funcs(self, string_funcs):
-        """ Run functions on this string.
-
-        Parameters:
-            string_funcs (list): A list of functions that take a hed string object and return a list of issues.
-
-        Returns:
-            list: A list of issues found by these operations. Each issue is a dictionary.
-
-        Notes:
-            - This method potentially modifies the hed string object.
-
+    def validate(self, hed_schema, allow_placeholders=True, error_handler=None):
         """
-        string_issues = []
-        for string_func in string_funcs:
-            string_issues += string_func(self)
-            if string_issues:
-                if check_for_any_errors(string_issues):
-                    break
-
-        return string_issues
-
-    def validate(self, hed_ops=None, error_handler=None, **kwargs):
-        """ Run the given hed_ops on this string.
+        Validate the string using the schema
 
         Parameters:
-            hed_ops: (func, HedOps, or list): Operations to apply to this object.
-            error_handler (ErrorHandler or None): Used to report errors in context.  Uses a default if None.
-            kwargs:
-                See models.hed_ops.translate_ops or the specific hed_ops for additional options
-
+            hed_schema(HedSchema): The schema to use to validate
+            allow_placeholders(bool): allow placeholders in the string
+            error_handler(ErrorHandler or None): the error handler to use, creates a default one if none passed
         Returns:
-            list:  A list of issues encountered in applying these operations. Each issue is a dictionary.
-
-        Notes:
-            - Although this function is called validation, the HedOps can represent other transformations.
-
+            issues (list of dict): A list of issues for hed string
         """
-        if error_handler is None:
-            error_handler = ErrorHandler()
-        tag_funcs = translate_ops(hed_ops, **kwargs)
-
-        error_handler.push_error_context(ErrorContext.HED_STRING, self, increment_depth_after=False)
-        issues = self.apply_funcs(tag_funcs)
-        error_handler.add_context_to_issues(issues)
-        error_handler.pop_error_context()
+        from hed.validator import HedValidator
 
-        return issues
+        validator = HedValidator(hed_schema)
+        return validator.validate(self, allow_placeholders=allow_placeholders, error_handler=error_handler)
 
     def find_top_level_tags(self, anchor_tags, include_groups=2):
         """ Find top level groups with an anchor tag.
 
+            A max of 1 tag located per top level group.
+
         Parameters:
             anchor_tags (container):     A list/set/etc of short_base_tags to find groups by.
             include_groups (0, 1 or 2):  Parameter indicating what return values to include.
-
+                If 0: return only tags.
+                If 1: return only groups.
+                If 2 or any other value: return both.
         Returns:
             list or tuple: The returned result depends on include_groups:
-                - If 0: return only tags.
-                - If 1: return only groups.
-                - If 2 or any other value: return both.
-
-        Notes:
-            - A max of 1 tag located per top level group.
-
         """
         top_level_tags = []
         for group in self.groups():
             for tag in group.tags():
                 if tag.short_base_tag.lower() in anchor_tags:
                     top_level_tags.append((tag, group))
                     # Only capture a max of 1 per group.  These are implicitly unique.
                     break
 
         if include_groups == 0 or include_groups == 1:
             return [tag[include_groups] for tag in top_level_tags]
         return top_level_tags
 
+    def remove_refs(self):
+        """ This removes any refs(tags contained entirely inside curly braces) from the string.
+
+            This does NOT validate the contents of the curly braces.  This is only relevant when directly
+            editing sidecar strings.  Tools will naturally ignore these.
+        """
+        ref_tags = [tag for tag in self.get_all_tags() if tag.is_column_ref()]
+        if ref_tags:
+            self.remove(ref_tags)
```

### Comparing `hedtools-0.2.0/hed/models/hed_string_group.py` & `hedtools-0.3.0/hed/models/hed_string_group.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         for child in self._children:
             for sub_child in child.children:
                 sub_child._parent = self
 
         self._original_children = self._children
 
     def get_original_hed_string(self):
-        return "".join([group._hed_string for group in self._children])
+        return ",".join([group._hed_string for group in self._children])
 
     def sort(self):
         combined_string = HedString.from_hed_strings(self._children)
         combined_string.sorted(update_self=True)
         return combined_string
 
     @property
@@ -56,23 +56,21 @@
         Returns:
             list: a list of direct children of this group.
 
         """
         return [child for sub_string in self._children for child in sub_string._children]
 
     def remove(self, items_to_remove):
-        """ Remove any tags/groups in items_to_remove.
+        """ Remove tags/groups by identity.
 
         Parameters:
             items_to_remove (list): A list of HedGroup and HedTag objects to remove.
 
         Notes:
             - Any groups that become empty will also be pruned.
-            - This goes by identity, not equivalence.
-
         """
         all_groups = [group for sub_group in self._children for group in sub_group.get_all_groups()]
         self._remove(items_to_remove, all_groups)
         # Remove any lingering empty HedStrings
         if any(not hed_string for hed_string in self._children):
             if self._original_children is self._children:
                 self._original_children = self._children.copy()
@@ -81,20 +79,17 @@
     def replace(self, item_to_replace, new_contents):
         """ Replace an existing tag or group.
 
         Parameters:
             item_to_replace (HedTag or HedGroup): The tag to replace.
             new_contents (HedTag or HedGroup or list): The replacements for the tag.
 
-        Notes:
-            - It tag must exist in this an error is raised.
-
+        :raises KeyError:
+            - item_to_replace does not exist
         """
-
-        # this needs to pass the tag off to the appropriate group
         replace_sub_string = None
         for sub_string in self._children:
             for i, child in enumerate(sub_string.children):
                 if item_to_replace is child:
                     replace_sub_string = sub_string
                     break
```

### Comparing `hedtools-0.2.0/hed/models/hed_tag.py` & `hedtools-0.3.0/hed/models/hed_tag.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,77 +1,98 @@
 from hed.schema.hed_schema_constants import HedKey
-from hed.schema.hed_schema_entry import HedTagEntry
+import copy
 
 
 class HedTag:
     """ A single HED tag.
 
     Notes:
         - HedTag is a smart class in that it keeps track of its original value and positioning
           as well as pointers to the relevant HED schema information, if relevant.
 
     """
 
-    def __init__(self, hed_string, span=None, hed_schema=None):
+    def __init__(self, hed_string, span=None, hed_schema=None, def_dict=None):
         """ Creates a HedTag.
 
         Parameters:
             hed_string (str): Source hed string for this tag.
             span  (int, int): The start and end indexes of the tag in the hed_string.
             hed_schema (HedSchema or None): A convenience parameter for calculating canonical forms on creation.
 
-        Notes:
-            - This does not produce issues and is used primarily for testing.
-
+        :raises ValueError:
+            - You cannot pass a def_dict without also passing a schema.
         """
+        if def_dict and not hed_schema:
+            raise ValueError("Passing a def_dict without also passing a schema is invalid.")
         self._hed_string = hed_string
         if span is None:
             span = (0, len(hed_string))
         # This is the span into the original hed string for this tag
         self.span = span
 
-        # If this is present, use this as the org tag for most purposes.  This is generally only filled out
-        # if the tag has a name_prefix added, or is an expanded def.
+        # If this is present, use this as the org tag for most purposes.
+        # This is not generally used anymore, but you can use it to replace a tag in place.
         self._tag = None
 
-        self._schema_prefix = self._get_schema_prefix(self.org_tag)
+        self._namespace = self._get_schema_namespace(self.org_tag)
 
         # This is the schema this tag was converted to.
         self._schema = None
         self._schema_entry = None
 
         self._extension_value = ""
         self._parent = None
 
+        # Downsides: two new parameters
+        # Have to check for this value, slowing everything down potentially.
+        self._expandable = None
+        self._expanded = False
+
         if hed_schema:
             self.convert_to_canonical_forms(hed_schema)
+            if def_dict:
+                def_dict.construct_def_tag(self)
+
+    def copy(self):
+        """ Return a deep copy of this tag.
+
+        Returns:
+            HedTag: The copied group.
+
+        """
+        save_parent = self._parent
+        self._parent = None
+        return_copy = copy.deepcopy(self)
+        self._parent = save_parent
+        return return_copy
 
     @property
-    def schema_prefix(self):
-        """ Library prefix for this tag if one exists.
+    def schema_namespace(self):
+        """ Library namespace for this tag if one exists.
 
         Returns:
-            prefix (str): The library prefix, including the colon.
+            namespace (str): The library namespace, including the colon.
 
         """
-        return self._schema_prefix
+        return self._namespace
 
     @property
     def short_tag(self):
         """ Short form including value or extension.
 
         Returns:
             short_tag (str): The short form of the tag, including value or extension.
 
          Note:
              Only valid after calling convert_to_canonical_forms
 
         """
         if self._schema_entry:
-            return f"{self._schema_prefix}{self._schema_entry.short_tag_name}{self._extension_value}"
+            return f"{self._namespace}{self._schema_entry.short_tag_name}{self._extension_value}"
 
         return str(self)
 
     @property
     def base_tag(self):
         """ Long form without value or extension.
 
@@ -104,43 +125,42 @@
     @short_base_tag.setter
     def short_base_tag(self, new_tag_val):
         """ Change base tag, leaving extension or value.
 
         Parameters:
             new_tag_val (str): The new short_base_tag for this tag.
 
-        Raises:
-            ValueError: If tags cannot unidentified.
+        :raises ValueError:
+            - If the tag wasn't already identified
 
         Note:
             - Generally this is used to swap def to def-expand.
         """
         if self._schema_entry:
+            tag_entry = None
             if self._schema:
-                tag_entry = self._schema.get_tag_entry(new_tag_val, schema_prefix=self.schema_prefix)
-            else:
-                tag_entry, remainder = HedTagEntry.get_fake_tag_entry(new_tag_val, [new_tag_val.lower()])
+                if self.is_takes_value_tag():
+                    new_tag_val = new_tag_val + "/#"
+                tag_entry = self._schema.get_tag_entry(new_tag_val, schema_namespace=self.schema_namespace)
 
             self._schema_entry = tag_entry
         else:
             raise ValueError("Cannot set unidentified tags")
 
     @property
     def org_base_tag(self):
         """ Original form without value or extension.
 
         Returns:
             base_tag (str): The original form of the tag, without value or extension.
 
         Notes:
             - Warning: This could be empty if the original tag had a name_prefix prepended.
-            e.g. a column where "Label/" is prepended, thus the column value has zero base portion.
-
+              e.g. a column where "Label/" is prepended, thus the column value has zero base portion.
             - Only valid after calling convert_to_canonical_forms.
-
         """
         if self._schema_entry:
             extension_len = len(self._extension_value)
             if not extension_len:
                 return self.tag
 
             org_len = len(self.tag)
@@ -181,26 +201,22 @@
     def tag(self, new_tag_val):
         """ Allow you to overwrite the tag output text.
 
         Parameters:
             new_tag_val (str): New (implicitly long form) of tag to set.
 
         Notes:
-            - Primarily used to add prefixes from column metadata to tags.
-            - Only valid before calling convert_to_canonical_forms.
-
+            - You probably don't actually want to call this.
         """
-
-        if self._schema_entry:
-            raise ValueError("Can only edit tags before calculating canonical forms. " +
-                             "This could be updated to instead remove computed forms.")
         self._tag = new_tag_val
+        self._schema_entry = None
+        self.convert_to_canonical_forms(self._schema)
 
     @property
-    def extension_or_value_portion(self):
+    def extension(self):
         """ Get the extension or value of tag
 
             Generally this is just the portion after the last slash.
             Returns an empty string if no extension or value.
 
         Returns:
             str: The tag name.
@@ -210,24 +226,28 @@
 
         """
         if self._extension_value:
             return self._extension_value[1:]
 
         return ""
 
+    @extension.setter
+    def extension(self, x):
+        self._extension_value = f"/{x}"
+
     @property
     def long_tag(self):
         """ Long form including value or extension.
 
         Returns:
             str: The long form of this tag.
 
         """
         if self._schema_entry:
-            return f"{self._schema_prefix}{self._schema_entry.long_tag_name}{self._extension_value}"
+            return f"{self._namespace}{self._schema_entry.long_tag_name}{self._extension_value}"
         return str(self)
 
     @property
     def org_tag(self):
         """ Return the original unmodified tag.
 
         Returns:
@@ -246,64 +266,62 @@
         Notes:
             - Does not include any extension.
 
         """
         if self._schema_entry:
             return self._schema_entry.tag_terms
 
-        # TODO: Potentially remove this.  It's just a quick hack for testing
-        return tuple(str(self).lower())
+        return tuple()
 
-    def __str__(self):
-        """ Convert this HedTag to a string.
+    @property
+    def expanded(self):
+        """Returns if this is currently expanded or not.
 
-        Returns:
-            str: The original tag if we haven't set a new tag.(e.g. short to long).
+           Will always be false unless expandable is set.  This is primarily used for Def/Def-expand tags at present.
 
+        Returns:
+            bool: Returns true if this is currently expanded
         """
-        if self._schema_entry:
-            return self.short_tag
-
-        if self._tag:
-            return self._tag
+        return self._expanded
 
-        return self._hed_string[self.span[0]:self.span[1]]
+    @property
+    def expandable(self):
+        """Returns if this is expandable
 
-    def add_prefix_if_needed(self, required_prefix):
-        """ Add a prefix to this tag *unless* already formatted.
+           This is primarily used for Def/Def-expand tags at present.
 
-        Parameters:
-            required_prefix (str): The full name_prefix to add if not present.
+        Returns:
+            HedGroup or HedTag or None: Returns the expanded form of this tag
+        """
+        return self._expandable
 
-        Notes:
-            - This means we verify the tag does not have the required name_prefix, or any partial name_prefix.
+    def is_column_ref(self):
+        """ Returns if this tag is a column reference from a sidecar.
 
-        Examples:
-            Required: KnownTag1/KnownTag2
+            You should only see these if you are directly accessing sidecar strings, tools should remove them otherwise.
 
-            Case 1: KnownTag1/KnownTag2/ColumnValue
-                Will not be changed, has name_prefix already.
+        Returns:
+            bool: Returns True if this is a column ref
+        """
+        return self.org_tag.startswith('{') and self.org_tag.endswith('}')
 
-            Case 2: KnownTag2/ColumnValue
-                Will not be changed, has partial name_prefix already.
+    def __str__(self):
+        """ Convert this HedTag to a string.
 
-            Case 3: ColumnValue
-                Prefix will be added.
+        Returns:
+            str: The original tag if we haven't set a new tag.(e.g. short to long).
 
         """
+        if self._schema_entry:
+            return self.short_tag
+
+        if self._tag:
+            return self._tag
 
-        checking_prefix = required_prefix
-        while checking_prefix:
-            if self.lower().startswith(checking_prefix.lower()):
-                return
-            slash_index = checking_prefix.find("/") + 1
-            if slash_index == 0:
-                break
-            checking_prefix = checking_prefix[slash_index:]
-        self.tag = required_prefix + self.org_tag
+        return self._hed_string[self.span[0]:self.span[1]]
 
     def lower(self):
         """ Convenience function, equivalent to str(self).lower(). """
         return str(self).lower()
 
     def convert_to_canonical_forms(self, hed_schema):
         """ Update internal state based on schema.
@@ -311,18 +329,15 @@
         Parameters:
             hed_schema (HedSchema or HedSchemaGroup): The schema to use to validate this tag
 
         Returns:
             list:  A list of issues found during conversion. Each element is a dictionary.
 
         """
-        if not hed_schema:
-            return self._convert_key_tags_to_canonical_form()
-
-        tag_entry, remainder, tag_issues = hed_schema.find_tag_entry(self, self.schema_prefix)
+        tag_entry, remainder, tag_issues = hed_schema.find_tag_entry(self, self.schema_namespace)
         self._schema_entry = tag_entry
         self._schema = hed_schema
         if self._schema_entry:
             if remainder:
                 self._extension_value = remainder
 
         return tag_issues
@@ -339,15 +354,15 @@
 
         """
         tag_unit_classes = self.unit_classes
         stripped_value, unit = self._get_tag_units_portion(tag_unit_classes)
         if stripped_value:
             return stripped_value, unit
 
-        return self.extension_or_value_portion, None
+        return self.extension, None
 
     @property
     def unit_classes(self):
         """ Return a dict of all the unit classes this tag accepts.
 
         Returns:
             unit_classes (dict):  A dict of unit classes this tag accepts.
@@ -428,29 +443,29 @@
             return bool(self._schema_entry.unit_classes)
         return False
 
     def is_value_class_tag(self):
         """ Return true if this is a value class tag.
 
         Returns:
-            bool:  True if this is a a tag with a value class.
+            bool:  True if this is a tag with a value class.
 
         """
         if self._schema_entry:
             return bool(self._schema_entry.value_classes)
         return False
 
     def is_basic_tag(self):
         """  Return True if a known tag with no extension or value.
 
         Returns:
             bool:  True if this is a known tag without extension or value.
 
         """
-        return bool(self._schema_entry and not self.extension_or_value_portion)
+        return bool(self._schema_entry and not self.extension)
 
     def has_attribute(self, attribute):
         """ Return true if this is an attribute this tag has.
 
         Parameters:
             attribute (str): Name of the attribute.
 
@@ -484,15 +499,15 @@
         Returns:
             list: A list containing the unit class units associated with a particular tag or an empty list.
 
         """
         units = []
         unit_classes = self.unit_classes
         for unit_class_entry in unit_classes.values():
-            units += unit_class_entry.unit_class_units.keys()
+            units += unit_class_entry.units.keys()
 
         return units
 
     def get_unit_class_default_unit(self):
         """ Get the default unit class unit for this tag.
 
         Returns:
@@ -531,41 +546,23 @@
         Returns:
             bool: True if the tag has the given attribute. False, if otherwise.
 
         """
         if self._schema_entry:
             return self._schema_entry.any_parent_has_attribute(attribute=attribute)
 
-    def _convert_key_tags_to_canonical_form(self):
-        """ Find the canonical form for basic known tags.
-
-        Returns:
-            list: Always return an empty list.
-
-        Notes:
-            -  This is used for such as definition and def when no schema present
-
-        """
-        tags_to_identify = ["onset", "definition", "offset", "def-expand", "def"]
-        tag_entry, remainder = HedTagEntry.get_fake_tag_entry(str(self), tags_to_identify)
-        if tag_entry:
-            self._schema_entry = tag_entry
-            self._schema = None
-            self._extension_value = remainder
-
-        return []
-
-    def _get_schema_prefix(self, org_tag):
-        """ Finds the library prefix for the tag.
+    @staticmethod
+    def _get_schema_namespace(org_tag):
+        """ Finds the library namespace for the tag.
 
         Parameters:
             org_tag (str): A string representing a tag.
 
         Returns:
-            str: Library prefix string or empty.
+            str: Library namespace string or empty.
 
         """
         first_slash = org_tag.find("/")
         first_colon = org_tag.find(":")
 
         if first_colon != -1:
             if first_slash != -1 and first_colon > first_slash:
@@ -580,15 +577,15 @@
         Parameters:
             tag_unit_classes (dict): Dictionary of valid UnitClassEntry objects for this tag.
 
         Returns:
             stripped_value (str): The value with the units removed.
 
         """
-        value, _, units = self.extension_or_value_portion.rpartition(" ")
+        value, _, units = self.extension.rpartition(" ")
         if not units:
             return None, None
 
         for unit_class_entry in tag_unit_classes.values():
             all_valid_unit_permutations = unit_class_entry.derivative_units
 
             possible_match = self._find_modifier_unit_entry(units, all_valid_unit_permutations)
@@ -608,31 +605,36 @@
         if not possible_match or not possible_match.has_attribute(HedKey.UnitSymbol):
             possible_match = all_valid_unit_permutations.get(units.lower())
             if possible_match and possible_match.has_attribute(HedKey.UnitSymbol):
                 possible_match = None
 
         return possible_match
 
+    def is_placeholder(self):
+        if "#" in self.org_tag or "#" in self._extension_value:
+            return True
+        return False
+
     def replace_placeholder(self, placeholder_value):
         """ If tag has a placeholder character(#), replace with value.
 
         Parameters:
             placeholder_value (str): Value to replace placeholder with.
 
         """
-        if "#" in self.org_tag:
+        if self.is_placeholder():
             if self._schema_entry:
                 self._extension_value = self._extension_value.replace("#", placeholder_value)
             else:
                 self._tag = self.tag.replace("#", placeholder_value)
 
     def __hash__(self):
         if self._schema_entry:
             return hash(
-                self._schema_prefix + self._schema_entry.short_tag_name.lower() + self._extension_value.lower())
+                self._namespace + self._schema_entry.short_tag_name.lower() + self._extension_value.lower())
         else:
             return hash(self.lower())
 
     def __eq__(self, other):
         if self is other:
             return True
 
@@ -644,7 +646,32 @@
 
         if self.short_tag.lower() == other.short_tag.lower():
             return True
 
         if self.org_tag.lower() == other.org_tag.lower():
             return True
         return False
+
+    def __deepcopy__(self, memo):
+        # check if the object has already been copied
+        if id(self) in memo:
+            return memo[id(self)]
+
+        # create a new instance of HedTag class
+        new_tag = HedTag(self._hed_string, self.span)
+
+        # add the new object to the memo dictionary
+        memo[id(self)] = new_tag
+
+        # copy all other attributes except schema and schema_entry
+        new_tag._tag = copy.deepcopy(self._tag, memo)
+        new_tag._namespace = copy.deepcopy(self._namespace, memo)
+        new_tag._extension_value = copy.deepcopy(self._extension_value, memo)
+        new_tag._parent = copy.deepcopy(self._parent, memo)
+        new_tag._expandable = copy.deepcopy(self._expandable, memo)
+        new_tag._expanded = copy.deepcopy(self._expanded, memo)
+
+        # reference the schema and schema_entry from the original object
+        new_tag._schema = self._schema
+        new_tag._schema_entry = self._schema_entry
+
+        return new_tag
```

### Comparing `hedtools-0.2.0/hed/models/model_constants.py` & `hedtools-0.3.0/hed/models/model_constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,19 +22,26 @@
 00000150: 4f52 475f 4b45 592e 6c6f 7765 7228 290a  ORG_KEY.lower().
 00000160: 2020 2020 4445 465f 4558 5041 4e44 5f4b      DEF_EXPAND_K
 00000170: 4559 203d 2044 4546 5f45 5850 414e 445f  EY = DEF_EXPAND_
 00000180: 4f52 475f 4b45 592e 6c6f 7765 7228 290a  ORG_KEY.lower().
 00000190: 2020 2020 4445 4649 4e49 5449 4f4e 5f4b      DEFINITION_K
 000001a0: 4559 203d 2044 4546 494e 4954 494f 4e5f  EY = DEFINITION_
 000001b0: 4f52 475f 4b45 592e 6c6f 7765 7228 290a  ORG_KEY.lower().
-000001c0: 0a20 2020 204f 4e53 4554 5f4f 5247 5f4b  .    ONSET_ORG_K
-000001d0: 4559 203d 2022 4f6e 7365 7422 0a20 2020  EY = "Onset".   
-000001e0: 204f 4646 5345 545f 4f52 475f 4b45 5920   OFFSET_ORG_KEY 
-000001f0: 3d20 224f 6666 7365 7422 0a0a 2020 2020  = "Offset"..    
-00000200: 4f4e 5345 545f 4b45 5920 3d20 4f4e 5345  ONSET_KEY = ONSE
-00000210: 545f 4f52 475f 4b45 592e 6c6f 7765 7228  T_ORG_KEY.lower(
-00000220: 290a 2020 2020 4f46 4653 4554 5f4b 4559  ).    OFFSET_KEY
-00000230: 203d 204f 4646 5345 545f 4f52 475f 4b45   = OFFSET_ORG_KE
-00000240: 592e 6c6f 7765 7228 290a 0a20 2020 2044  Y.lower()..    D
-00000250: 4546 5f4b 4559 5320 3d20 2844 4546 5f4b  EF_KEYS = (DEF_K
-00000260: 4559 2c20 4445 465f 4558 5041 4e44 5f4b  EY, DEF_EXPAND_K
-00000270: 4559 29                                  EY)
+000001c0: 2020 2020 4445 465f 4b45 5953 203d 2028      DEF_KEYS = (
+000001d0: 4445 465f 4b45 592c 2044 4546 5f45 5850  DEF_KEY, DEF_EXP
+000001e0: 414e 445f 4b45 5929 0a0a 2020 2020 4f4e  AND_KEY)..    ON
+000001f0: 5345 545f 4f52 475f 4b45 5920 3d20 224f  SET_ORG_KEY = "O
+00000200: 6e73 6574 220a 2020 2020 4f46 4653 4554  nset".    OFFSET
+00000210: 5f4f 5247 5f4b 4559 203d 2022 4f66 6673  _ORG_KEY = "Offs
+00000220: 6574 220a 2020 2020 494e 5345 545f 4f52  et".    INSET_OR
+00000230: 475f 4b45 5920 3d20 2249 6e73 6574 220a  G_KEY = "Inset".
+00000240: 0a20 2020 204f 4e53 4554 5f4b 4559 203d  .    ONSET_KEY =
+00000250: 204f 4e53 4554 5f4f 5247 5f4b 4559 2e6c   ONSET_ORG_KEY.l
+00000260: 6f77 6572 2829 0a20 2020 204f 4646 5345  ower().    OFFSE
+00000270: 545f 4b45 5920 3d20 4f46 4653 4554 5f4f  T_KEY = OFFSET_O
+00000280: 5247 5f4b 4559 2e6c 6f77 6572 2829 0a20  RG_KEY.lower(). 
+00000290: 2020 2049 4e53 4554 5f4b 4559 203d 2049     INSET_KEY = I
+000002a0: 4e53 4554 5f4f 5247 5f4b 4559 2e6c 6f77  NSET_ORG_KEY.low
+000002b0: 6572 2829 0a0a 2020 2020 5445 4d50 4f52  er()..    TEMPOR
+000002c0: 414c 5f4b 4559 5320 3d20 7b4f 4e53 4554  AL_KEYS = {ONSET
+000002d0: 5f4b 4559 2c20 4f46 4653 4554 5f4b 4559  _KEY, OFFSET_KEY
+000002e0: 2c20 494e 5345 545f 4b45 597d 0a         , INSET_KEY}.
```

### Comparing `hedtools-0.2.0/hed/models/onset_mapper.py` & `hedtools-0.3.0/hed/validator/onset_validator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,29 @@
 from hed.models.model_constants import DefTagNames
 from hed.models.hed_group import HedGroup
 from hed.errors.error_reporter import ErrorHandler
 from hed.errors.error_types import OnsetErrors
-from hed.models.hed_ops import HedOps
 
 
-class OnsetMapper(HedOps):
-    """ HedOps responsible for matching onset/offset pairs. """
+class OnsetValidator:
+    """ Validates onset/offset pairs. """
 
-    def __init__(self, def_mapper):
-        super().__init__()
-        self._def_mapper = def_mapper
+    def __init__(self, def_dict, run_full_onset_checks=True):
+        self._defs = def_dict
         self._onsets = {}
+        self._run_full_onset_checks = run_full_onset_checks
 
-    def check_for_onset_offset(self, hed_string_obj):
-        """ Check for onset or offset and track context.
+    def validate_onset_offset(self, hed_string_obj):
+        """ Validate onset/offset
 
         Parameters:
-            hed_string_obj (HedString): The hed string to check.  Finds a maximum of one onset tag.
+            hed_string_obj (HedString): The hed string to check.
 
         Returns:
             list: A list of issues found in validating onsets (i.e., out of order onsets, unknown def names).
-
-        Notes:
-            - Each issue in the return list is a dictionary.
-
         """
         onset_issues = []
         for found_onset, found_group in self._find_onset_tags(hed_string_obj):
             if not found_onset:
                 return []
 
             def_tags = found_group.find_def_tags()
@@ -45,15 +40,15 @@
             # Get all children but def group and onset/offset, then validate #/type of children.
             def_tag, def_group, _ = def_tags[0]
             if def_group is None:
                 def_group = def_tag
             children = [child for child in found_group.children if
                         def_group is not child and found_onset is not child]
             max_children = 1
-            if found_onset.short_base_tag.lower() == DefTagNames.OFFSET_KEY:
+            if found_onset.short_base_tag == DefTagNames.OFFSET_ORG_KEY:
                 max_children = 0
             if len(children) > max_children:
                 onset_issues += ErrorHandler.format_error(OnsetErrors.ONSET_WRONG_NUMBER_GROUPS,
                                                           def_tag,
                                                           found_group.children)
                 continue
 
@@ -67,43 +62,40 @@
 
             # At this point we have either an onset or offset tag and it's name
             onset_issues += self._handle_onset_or_offset(def_tag, found_onset)
 
         return onset_issues
 
     def _find_onset_tags(self, hed_string_obj):
-        return hed_string_obj.find_top_level_tags(anchor_tags={DefTagNames.ONSET_KEY, DefTagNames.OFFSET_KEY})
+        return hed_string_obj.find_top_level_tags(anchor_tags=DefTagNames.TEMPORAL_KEYS)
 
     def _handle_onset_or_offset(self, def_tag, onset_offset_tag):
-        is_onset = onset_offset_tag.short_base_tag.lower() == DefTagNames.ONSET_KEY
-        full_def_name = def_name = def_tag.extension_or_value_portion
+        is_onset = onset_offset_tag.short_base_tag == DefTagNames.ONSET_ORG_KEY
+        full_def_name = def_name = def_tag.extension
         placeholder = None
         found_slash = def_name.find("/")
         if found_slash != -1:
             placeholder = def_name[found_slash + 1:]
             def_name = def_name[:found_slash]
 
-        def_entry = self._def_mapper.get_def_entry(def_name)
+        def_entry = self._defs.get(def_name)
         if def_entry is None:
             return ErrorHandler.format_error(OnsetErrors.ONSET_DEF_UNMATCHED, tag=def_tag)
         if bool(def_entry.takes_value) != bool(placeholder):
             return ErrorHandler.format_error(OnsetErrors.ONSET_PLACEHOLDER_WRONG, tag=def_tag,
                                              has_placeholder=bool(def_entry.takes_value))
 
-        if is_onset:
-            # onset can never fail as it implies an offset
-            self._onsets[full_def_name.lower()] = full_def_name
-        else:
-            if full_def_name.lower() not in self._onsets:
-                return ErrorHandler.format_error(OnsetErrors.OFFSET_BEFORE_ONSET, tag=def_tag)
+        if self._run_full_onset_checks:
+            if is_onset:
+                # onset can never fail as it implies an offset
+                self._onsets[full_def_name.lower()] = full_def_name
             else:
-                del self._onsets[full_def_name.lower()]
-
-        return []
-
-    def __get_string_funcs__(self, **kwargs):
-        string_funcs = []
-        string_funcs.append(self.check_for_onset_offset)
-        return string_funcs
+                is_offset = onset_offset_tag.short_base_tag == DefTagNames.OFFSET_ORG_KEY
+                if full_def_name.lower() not in self._onsets:
+                    if is_offset:
+                        return ErrorHandler.format_error(OnsetErrors.OFFSET_BEFORE_ONSET, tag=def_tag)
+                    else:
+                        return ErrorHandler.format_error(OnsetErrors.INSET_BEFORE_ONSET, tag=def_tag)
+                elif is_offset:
+                    del self._onsets[full_def_name.lower()]
 
-    def __get_tag_funcs__(self, **kwargs):
         return []
```

### Comparing `hedtools-0.2.0/hed/models/sidecar.py` & `hedtools-0.3.0/hed/models/sidecar.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,92 +1,103 @@
 import json
+import re
+
 from hed.models.column_metadata import ColumnMetadata
-from hed.errors.error_types import ErrorContext, SidecarErrors
+from hed.errors.error_types import ErrorContext
 from hed.errors import ErrorHandler
 from hed.errors.exceptions import HedFileError, HedExceptions
 from hed.models.hed_string import HedString
 from hed.models.column_metadata import ColumnType
-from hed.models.hed_ops import apply_ops, hed_string_iter, set_hed_string
-from hed.models.sidecar_base import SidecarBase
+from hed.models.definition_dict import DefinitionDict
 
 
-class Sidecar(SidecarBase):
+class Sidecar:
     """ Contents of a JSON file or merged file.
 
     """
 
-    def __init__(self, files, name=None, hed_schema=None):
+    def __init__(self, files, name=None):
         """ Construct a Sidecar object representing a JSON file.
 
         Parameters:
             files (str or FileLike or list): A string or file-like object representing a JSON file, or a list of such.
             name (str or None): Optional name identifying this sidecar, generally a filename.
-            hed_schema(HedSchema or None): The schema to use by default in identifying tags
         """
-        super().__init__(name, hed_schema=hed_schema)
+        self.name = name
         self.loaded_dict = self.load_sidecar_files(files)
-        self.def_dict = self.extract_definitions(hed_schema)
+        self._def_dict = None
+        self._extract_definition_issues = []
 
-    @property
-    def column_data(self):
-        """ Generates the list of ColumnMetadata for this sidecar
+    def __iter__(self):
+        """ An iterator to go over the individual column metadata.
 
         Returns:
-            list(ColumnMetadata): the list of column metadata defined by this sidecar
+            iterator: An iterator over the column metadata values.
+
         """
-        for col_name, col_dict in self.loaded_dict.items():
-            yield self._generate_single_column(col_name, col_dict)
+        return iter(self.column_data.values())
 
-    def _hed_string_iter(self, tag_funcs, error_handler):
-        """ Low level function to retrieve hed string in sidecar
+    def __getitem__(self, column_name):
+        if column_name not in self.loaded_dict:
+            return None
+        return ColumnMetadata(name=column_name)
 
-        Parameters:
-            tag_funcs(list): A list of functions to apply to returned strings
-            error_handler(ErrorHandler): Error handler to use for context
+    @property
+    def all_hed_columns(self):
+        """ Returns all columns that are HED compatible
 
-        Yields:
-            tuple:
-                string(HedString): The retrieved and modified string
-                position(tuple): The location of this hed string.  Black box.
-                issues(list): A list of issues running the tag_funcs.
+            returns:
+                column_refs(list): A list of all valid hed columns by name
         """
-        for column_name, dict_for_entry in self.loaded_dict.items():
-            error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, column_name)
-            hed_dict = dict_for_entry.get("HED", {})
-            for (hed_string_obj, position, issues) in hed_string_iter(hed_dict, tag_funcs, error_handler):
-                yield hed_string_obj, (column_name, position), issues
+        possible_column_references = [column.column_name for column in self if column.column_type != ColumnType.Ignore]
+        if "HED" not in possible_column_references:
+            possible_column_references.append("HED")
 
-            error_handler.pop_error_context()
+        return possible_column_references
 
-    def _set_hed_string(self, new_hed_string, position):
-        """ Low level function to update hed string in sidecar
+    @property
+    def def_dict(self):
+        """This is the definitions from this sidecar.
 
-        Parameters:
-            new_hed_string (str or HedString): The new hed_string to replace the value at position.
-            position (tuple):   The value returned from hed_string_iter.
+            Generally you should instead call get_def_dict to get the relevant definitions
+
+        Returns:
+            DefinitionDict: The definitions for this sidecar
         """
-        column_name, position = position
-        hed_dict = self.loaded_dict[column_name]
-        hed_dict["HED"] = set_hed_string(new_hed_string, hed_dict["HED"], position)
+        return self._def_dict
 
-    def validate_structure(self, error_handler):
-        """ Validate the raw structure of this sidecar.
+    @property
+    def column_data(self):
+        """ Generates the ColumnMetadata for this sidecar
+
+        Returns:
+            dict({str:ColumnMetadata}): the column metadata defined by this sidecar
+        """
+        return {col_name: ColumnMetadata(name=col_name, source=self.loaded_dict) for col_name in self.loaded_dict}
+
+    def get_def_dict(self, hed_schema=None, extra_def_dicts=None):
+        """ Returns the definition dict for this sidecar.
 
         Parameters:
-            error_handler(ErrorHandler): The error handler to use for error context
+            hed_schema(HedSchema): used to identify tags to find definitions
+            extra_def_dicts (list, DefinitionDict, or None): Extra dicts to add to the list.
 
         Returns:
-            issues(list): A list of issues found with the structure
+            DefinitionDict:   A single definition dict representing all the data(and extra def dicts)
         """
-        all_validation_issues = []
-        for column_name, dict_for_entry in self.loaded_dict.items():
-            error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, column_name)
-            all_validation_issues += self._validate_column_structure(column_name, dict_for_entry, error_handler)
-            error_handler.pop_error_context()
-        return all_validation_issues
+        if self._def_dict is None and hed_schema:
+            self._def_dict = self.extract_definitions(hed_schema)
+        def_dicts = []
+        if self.def_dict:
+            def_dicts.append(self.def_dict)
+        if extra_def_dicts:
+            if not isinstance(extra_def_dicts, list):
+                extra_def_dicts = [extra_def_dicts]
+            def_dicts += extra_def_dicts
+        return DefinitionDict(def_dicts)
 
     def save_as_json(self, save_filename):
         """ Save column metadata to a JSON file.
 
         Parameters:
             save_filename (str): Path to save file
 
@@ -105,16 +116,17 @@
 
     def load_sidecar_file(self, file):
         """ Load column metadata from a given json file.
 
         Parameters:
             file (str or FileLike): If a string, this is a filename. Otherwise, it will be parsed as a file-like.
 
-        Raises:
-            HedFileError: If the file was not found or could not be parsed into JSON.
+        :raises HedFileError:
+            - If the file was not found or could not be parsed into JSON.
+            
         """
         if not file:
             return {}
         elif isinstance(file, str):
             try:
                 with open(file, "r") as fp:
                     if not self.name:
@@ -128,119 +140,112 @@
             return self._load_json_file(file)
 
     def load_sidecar_files(self, files):
         """ Load json from a given file or list
 
         Parameters:
             files (str or FileLike or list): A string or file-like object representing a JSON file, or a list of such.
-        Raises:
-            HedFileError: If the file was not found or could not be parsed into JSON.
+
+        :raises HedFileError:
+            - If the file was not found or could not be parsed into JSON.
+            
         """
         if not files:
             return {}
         if not isinstance(files, list):
             files = [files]
 
         merged_dict = {}
         for file in files:
             loaded_json = self.load_sidecar_file(file)
             merged_dict.update(loaded_json)
         return merged_dict
 
+    def validate(self, hed_schema, extra_def_dicts=None, name=None, error_handler=None):
+        """Create a SidecarValidator and validate this sidecar with the schema.
+
+        Parameters:
+            hed_schema (HedSchema): Input data to be validated.
+            extra_def_dicts(list or DefinitionDict): Extra def dicts in addition to sidecar.
+            name(str): The name to report this sidecar as.
+            error_handler (ErrorHandler): Error context to use.  Creates a new one if None.
+            
+        Returns:
+            issues (list of dict): A list of issues associated with each level in the HED string.
+        """
+        from hed.validator.sidecar_validator import SidecarValidator
+
+        if error_handler is None:
+            error_handler = ErrorHandler()
+
+        validator = SidecarValidator(hed_schema)
+        issues = validator.validate(self, extra_def_dicts, name, error_handler=error_handler)
+        return issues
+
     def _load_json_file(self, fp):
         """ Load the raw json of a given file
 
         Parameters:
             fp (File-like): The JSON source stream.
 
-        Raises:
-            HedFileError:  If the file cannot be parsed.
+        :raises HedFileError:
+            - If the file cannot be parsed.
+            
         """
         try:
             return json.load(fp)
         except json.decoder.JSONDecodeError as e:
             raise HedFileError(HedExceptions.CANNOT_PARSE_JSON, str(e), self.name)
 
-    def _generate_single_column(self, column_name, dict_for_entry, column_type=None):
-        """ Create a single column metadata entry and add to this sidecar.
-
-        Parameters:
-            column_name (str or int): The column name or number
-            dict_for_entry (dict): The loaded dictionary for a given column entry (needs the "HED" key if nothing else).
-            column_type (ColumnType): Optional indicator of how to treat the column.
-                This overrides auto-detection from the dict_for_entry.
-
-        """
-        if column_type is None:
-            column_type = self._detect_column_type(dict_for_entry)
-        if dict_for_entry:
-            hed_dict = dict_for_entry.get("HED")
-        else:
-            hed_dict = None
-        def_removed_dict, _ = apply_ops(hed_dict, HedString.remove_definitions)
-        column_entry = ColumnMetadata(column_type, column_name, def_removed_dict)
-        return column_entry
-
-    @staticmethod
-    def _detect_column_type(dict_for_entry):
-        """ Determine the ColumnType of a given json entry.
+    def extract_definitions(self, hed_schema=None, error_handler=None):
+        """ Gather and validate definitions in metadata.
 
         Parameters:
-            dict_for_entry (dict): The loaded json entry a specific column.
-                Generally has a "HED" entry among other optional ones.
+            hed_schema (HedSchema or None): The schema to used to identify tags.
+            error_handler (ErrorHandler or None): The error handler to use for context, uses a default one if None.
 
         Returns:
-            ColumnType: The determined type of given column.  Returns None if unknown.
+            DefinitionDict: Contains all the definitions located in the sidecar.
 
         """
-        if not dict_for_entry or not isinstance(dict_for_entry, dict):
-            return ColumnType.Ignore
-
-        minimum_required_keys = ("HED",)
-        if not set(minimum_required_keys).issubset(dict_for_entry.keys()):
-            return ColumnType.Ignore
-
-        hed_entry = dict_for_entry["HED"]
-        if isinstance(hed_entry, dict):
-            return ColumnType.Categorical
-
-        if not isinstance(hed_entry, str):
-            return None
+        if error_handler is None:
+            error_handler = ErrorHandler()
+        def_dict = DefinitionDict()
+
+        self._extract_definition_issues = []
+        if hed_schema:
+            for column_data in self:
+                error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, column_data.column_name)
+                hed_strings = column_data.get_hed_strings()
+                for key_name, hed_string in hed_strings.items():
+                    hed_string_obj = HedString(hed_string, hed_schema)
+                    if len(hed_strings) > 1:
+                        error_handler.push_error_context(ErrorContext.SIDECAR_KEY_NAME, key_name)
+                    error_handler.push_error_context(ErrorContext.HED_STRING, hed_string_obj)
+                    self._extract_definition_issues += def_dict.check_for_definitions(hed_string_obj, error_handler)
+                    error_handler.pop_error_context()
+                    if len(hed_strings) > 1:
+                        error_handler.pop_error_context()
 
-        if "#" not in dict_for_entry["HED"]:
-            return None
+                error_handler.pop_error_context()
 
-        return ColumnType.Value
+        return def_dict
 
-    def _validate_column_structure(self, column_name, dict_for_entry, error_handler):
-        """ Checks primarily for type errors such as expecting a string and getting a list in a json sidecar.
+    def get_column_refs(self):
+        """ Returns a list of column refs found in this sidecar.
 
-        Parameters:
-            error_handler (ErrorHandler)  Sets the context for the error reporting. Cannot be None.
+            This does not validate
 
         Returns:
-            list:  Issues in performing the operations. Each issue is a dictionary.
-
-        """
-        val_issues = []
-        column_type = self._detect_column_type(dict_for_entry=dict_for_entry)
-        if column_type is None:
-            val_issues += ErrorHandler.format_error(SidecarErrors.UNKNOWN_COLUMN_TYPE,
-                                                    column_name=column_name)
-        elif column_type == ColumnType.Categorical:
-            raw_hed_dict = dict_for_entry["HED"]
-            if not raw_hed_dict:
-                val_issues += ErrorHandler.format_error(SidecarErrors.BLANK_HED_STRING)
-            if not isinstance(raw_hed_dict, dict):
-                val_issues += ErrorHandler.format_error(SidecarErrors.WRONG_HED_DATA_TYPE,
-                                                        given_type=type(raw_hed_dict),
-                                                        expected_type="dict")
-            for key_name, hed_string in raw_hed_dict.items():
-                if not isinstance(hed_string, str):
-                    error_handler.push_error_context(ErrorContext.SIDECAR_KEY_NAME, key_name)
-                    val_issues += ErrorHandler.format_error(SidecarErrors.WRONG_HED_DATA_TYPE,
-                                                            given_type=type(hed_string),
-                                                            expected_type="str")
-                    error_handler.pop_error_context()
-        error_handler.add_context_to_issues(val_issues)
+            column_refs(list): A list of unique column refs found
+        """
+        found_vals = set()
+        for column_data in self:
+            if column_data.column_type == ColumnType.Ignore:
+                continue
+            hed_strings = column_data.get_hed_strings()
+            matches = hed_strings.str.findall(r"\{([a-z_\-0-9]+)\}", re.IGNORECASE)
+            u_vals = [match for sublist in matches for match in sublist]
+
+            found_vals.update(u_vals)
 
-        return val_issues
+        return list(found_vals)
```

### Comparing `hedtools-0.2.0/hed/models/sidecar_base.py` & `hedtools-0.3.0/hed/validator/sidecar_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,252 +1,246 @@
 import copy
+import re
+from hed.errors import ErrorHandler, ErrorContext, SidecarErrors, DefinitionErrors, ColumnErrors
+from hed.models import ColumnType
+from hed import HedString
+from hed import Sidecar
 from hed.models.column_metadata import ColumnMetadata
-from hed.errors.error_types import ErrorContext
-from hed.errors import error_reporter
-from hed.errors import ErrorHandler
-from hed.models.hed_string import HedString
-from hed.models.def_mapper import DefMapper
-from hed.models.hed_ops import translate_ops, apply_ops
-from hed.models.definition_dict import DefinitionDict
-from functools import partial
-
-
-class SidecarBase:
-    """ Baseclass for specialized spreadsheet sidecars
-
-        To subclass this class, you'll want to override at the minimum:
-        _hed_string_iter
-        _set_hed_string
-        validate_structure
-        column_data property <- This is the only truly mandatory one
-
-    """
-    def __init__(self, name=None, hed_schema=None):
-        """ Initialize a sidecar baseclass
+from hed.errors.error_reporter import sort_issues
+from hed.models.model_constants import DefTagNames
+from hed.errors.error_reporter import check_for_any_errors
 
-        Parameters:
-            name (str or None): Optional name identifying this sidecar, generally a filename.
-            hed_schema(HedSchema or None): The schema to use by default in identifying tags
-        """
-        self.name = name
-        self._schema = hed_schema
-        # Expected to be called in subclass after data is loaded
-        # self.def_dict = self.extract_definitions()
 
-    @property
-    def column_data(self):
-        """ Generates the list of ColumnMetadata for this sidecar
+# todo: Add/improve validation for definitions being in known columns(right now it just assumes they aren't)
+class SidecarValidator:
+    reserved_column_names = ["HED"]
+    reserved_category_values = ["n/a"]
 
-        Returns:
-            list(ColumnMetadata): the list of column metadata defined by this sidecar
+    def __init__(self, hed_schema):
         """
-        return []
-
-    def _hed_string_iter(self, tag_funcs, error_handler):
-        """ Low level function to retrieve hed string in sidecar
+        Constructor for the HedValidator class.
 
         Parameters:
-            tag_funcs(list): A list of functions to apply to returned strings
-            error_handler(ErrorHandler): Error handler to use for context
-
-        Yields:
-            tuple:
-                string(HedString): The retrieved and modified string
-                position(tuple): The location of this hed string.  Black box.
-                issues(list): A list of issues running the tag_funcs.
+            hed_schema (HedSchema): HED schema object to use for validation.
         """
-        yield
-
-    def _set_hed_string(self, new_hed_string, position):
-        """ Low level function to update hed string in sidecar
+        self._schema = hed_schema
 
-        Parameters:
-            new_hed_string (str or HedString): The new hed_string to replace the value at position.
-            position (tuple):   The value returned from hed_string_iter.
-        """
-        return
-
-    def validate_structure(self, error_handler):
-        """ Validate the raw structure of this sidecar.
+    def validate(self, sidecar, extra_def_dicts=None, name=None, error_handler=None):
+        """Validate the input data using the schema
 
         Parameters:
-            error_handler(ErrorHandler): The error handler to use for error context
-
+            sidecar (Sidecar): Input data to be validated.
+            extra_def_dicts(list or DefinitionDict): extra def dicts in addition to sidecar
+            name(str): The name to report this sidecar as
+            error_handler (ErrorHandler): Error context to use.  Creates a new one if None
         Returns:
-            issues(list): A list of issues found with the structure
-        """
-        return []
-
-    def __iter__(self):
-        """ An iterator to go over the individual column metadata.
-
-        Returns:
-            iterator: An iterator over the column metadata values.
-
-        """
-        return iter(self.column_data)
-
-    def hed_string_iter(self, hed_ops=None, error_handler=None, expand_defs=False, remove_definitions=False,
-                        allow_placeholders=True, extra_def_dicts=None, **kwargs):
-        """ Iterator over hed strings in columns.
-
-        Parameters:
-            hed_ops (func, HedOps, list):  A HedOps, funcs or list of these to apply to the hed strings
-                                            before returning
-            error_handler (ErrorHandler): The error handler to use for context, uses a default one if none.
-            expand_defs (bool): If True, expand all def tags located in the strings.
-            remove_definitions (bool): If True, remove all definitions found in the string.
-            allow_placeholders (bool): If False, placeholders will be marked as validation warnings.
-            extra_def_dicts (DefinitionDict, list, None): Extra dicts to add to the list.
-            kwargs: See models.hed_ops.translate_ops or the specific hed_ops for additional options.
-
-        Yields:
-            tuple:
-                - HedString: A HedString at a given column and key position.
-                - tuple: Indicates where hed_string was loaded from so it can be later set by the user
-                - list: A list of issues found performing ops. Each issue is a dictionary.
-
+            issues (list of dict): A list of issues associated with each level in the HED string.
         """
+        from hed.validator import HedValidator
+        issues = []
         if error_handler is None:
             error_handler = ErrorHandler()
-        hed_ops = self._standardize_ops(hed_ops)
-        if expand_defs or remove_definitions:
-            self._add_definition_mapper(hed_ops, extra_def_dicts)
-        tag_funcs = translate_ops(hed_ops, hed_schema=self._schema, error_handler=error_handler,
-                                  expand_defs=expand_defs, allow_placeholders=allow_placeholders,
-                                  remove_definitions=remove_definitions, **kwargs)
-
-        return self._hed_string_iter(tag_funcs, error_handler)
 
-    def set_hed_string(self, new_hed_string, position):
-        """ Set a provided column/category key/etc.
+        error_handler.push_error_context(ErrorContext.FILE_NAME, name)
+        issues += self.validate_structure(sidecar, error_handler=error_handler)
+        issues += self._validate_refs(sidecar, error_handler)
 
-        Parameters:
-            new_hed_string (str or HedString): The new hed_string to replace the value at position.
-            position (tuple):   The (HedString, str, list) tuple returned from hed_string_iter.
+        # only allowed early out, something is very wrong with structure or refs
+        if check_for_any_errors(issues):
+            error_handler.pop_error_context()
+            return issues
+        sidecar_def_dict = sidecar.get_def_dict(hed_schema=self._schema, extra_def_dicts=extra_def_dicts)
+        hed_validator = HedValidator(self._schema,
+                                     def_dicts=sidecar_def_dict,
+                                     run_full_onset_checks=False,
+                                     definitions_allowed=True)
+
+        issues += sidecar._extract_definition_issues
+        issues += sidecar_def_dict.issues
+
+        definition_checks = {}
+        for column_data in sidecar:
+            column_name = column_data.column_name
+            hed_strings = column_data.get_hed_strings()
+            error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, column_name)
+            for key_name, hed_string in hed_strings.items():
+                new_issues = []
+                if len(hed_strings) > 1:
+                    error_handler.push_error_context(ErrorContext.SIDECAR_KEY_NAME, key_name)
+                hed_string_obj = HedString(hed_string, hed_schema=self._schema, def_dict=sidecar_def_dict)
+                hed_string_obj.remove_refs()
+
+                error_handler.push_error_context(ErrorContext.HED_STRING, hed_string_obj)
+                new_issues += hed_validator.run_basic_checks(hed_string_obj, allow_placeholders=True)
+                new_issues += hed_validator.run_full_string_checks(hed_string_obj)
+
+                def_check_list = definition_checks.setdefault(column_name, [])
+                def_check_list.append(hed_string_obj.find_tags({DefTagNames.DEFINITION_KEY}, recursive=True,
+                                                               include_groups=0))
+                # Might refine this later - for now just skip checking placeholder counts in definition columns.
+                if not def_check_list[-1]:
+                    new_issues += self._validate_pound_sign_count(hed_string_obj, column_type=column_data.column_type)
+
+                if len(hed_strings) > 1:
+                    error_handler.pop_error_context()
+                error_handler.add_context_and_filter(new_issues)
+                issues += new_issues
+            error_handler.pop_error_context()
+        error_handler.pop_error_context()
+        issues += self._check_definitions_bad_spot(definition_checks, error_handler)
+        issues = sort_issues(issues)
 
-        """
-        return self._set_hed_string(new_hed_string, position)
+        return issues
 
-    def _add_definition_mapper(self, hed_ops, extra_def_dicts=None):
-        """ Add a DefMapper if the hed_ops list doesn't have one.
+    def validate_structure(self, sidecar, error_handler):
+        """ Validate the raw structure of this sidecar.
 
         Parameters:
-            hed_ops (list):  A list of HedOps
-            extra_def_dicts (list):  DefDicts from outside.
+            sidecar(Sidecar): the sidecar to validate
+            error_handler(ErrorHandler): The error handler to use for error context
 
         Returns:
-            DefMapper:  A shallow copy of the hed_ops list with a DefMapper added if there wasn't one.
-
+            issues(list): A list of issues found with the structure
         """
-        def_mapper_list = [hed_op for hed_op in hed_ops if isinstance(hed_op, DefMapper)]
-
-        if not def_mapper_list:
-            def_dicts = self.get_def_dicts(extra_def_dicts)
-            def_mapper = DefMapper(def_dicts)
-            hed_ops.append(def_mapper)
-            return def_mapper
-        return def_mapper_list[0]
-
-    @staticmethod
-    def _standardize_ops(hed_ops):
-        if not isinstance(hed_ops, list):
-            hed_ops = [hed_ops]
-        return hed_ops.copy()
+        all_validation_issues = []
+        for column_name, dict_for_entry in sidecar.loaded_dict.items():
+            error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, column_name)
+            all_validation_issues += self._validate_column_structure(column_name, dict_for_entry, error_handler)
+            error_handler.pop_error_context()
+        return all_validation_issues
 
-    def get_def_dicts(self, extra_def_dicts=None):
-        """ Returns the definition dict for this sidecar.
+    def _validate_refs(self, sidecar, error_handler):
+        possible_column_refs = sidecar.all_hed_columns
 
-        Parameters:
-            extra_def_dicts (list, DefinitionDict, or None): Extra dicts to add to the list.
+        issues = []
+        found_column_references = {}
+        for column_data in sidecar:
+            column_name = column_data.column_name
+            hed_strings = column_data.get_hed_strings()
+            error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, column_name)
+            matches = []
+            for key_name, hed_string in hed_strings.items():
+                new_issues = []
+                if len(hed_strings) > 1:
+                    error_handler.push_error_context(ErrorContext.SIDECAR_KEY_NAME, key_name)
+
+                error_handler.push_error_context(ErrorContext.HED_STRING, HedString(hed_string))
+                invalid_locations = self._find_non_matching_braces(hed_string)
+                for loc in invalid_locations:
+                    bad_symbol = hed_string[loc]
+                    new_issues += error_handler.format_error_with_context(ColumnErrors.MALFORMED_COLUMN_REF,
+                                                                          column_name, loc, bad_symbol)
+
+                sub_matches = re.findall(r"\{([a-z_\-0-9]+)\}", hed_string, re.IGNORECASE)
+                matches.append(sub_matches)
+                for match in sub_matches:
+                    if match not in possible_column_refs:
+                        new_issues += error_handler.format_error_with_context(ColumnErrors.INVALID_COLUMN_REF, match)
+
+                error_handler.pop_error_context()
+                if len(hed_strings) > 1:
+                    error_handler.pop_error_context()
+                error_handler.add_context_and_filter(new_issues)
+                issues += new_issues
+            error_handler.pop_error_context()
+            references = [match for sublist in matches for match in sublist]
+            if references:
+                found_column_references[column_name] = references
+            if column_name in references:
+                issues += error_handler.format_error_with_context(ColumnErrors.SELF_COLUMN_REF, column_name)
+
+        for column_name, refs in found_column_references.items():
+            for ref in refs:
+                if ref in found_column_references and ref != column_name:
+                    issues += error_handler.format_error_with_context(ColumnErrors.NESTED_COLUMN_REF, column_name, ref)
 
-        Returns:
-            list: A list with the sidecar def_dict plus any found in extra_def_dicts.
+        return issues
 
-        """
-        def_dicts = [self.def_dict]
-        if extra_def_dicts:
-            if not isinstance(extra_def_dicts, list):
-                extra_def_dicts = [extra_def_dicts]
-            def_dicts += extra_def_dicts
-        return def_dicts
-
-    def validate_entries(self, hed_ops=None, name=None, extra_def_dicts=None,
-                         error_handler=None, **kwargs):
-        """ Run the given hed_ops on all columns in this sidecar.
+    @staticmethod
+    def _find_non_matching_braces(hed_string):
+        issues = []
+        open_brace_index = -1
+
+        for i, char in enumerate(hed_string):
+            if char == '{':
+                if open_brace_index >= 0:  # Nested brace detected
+                    issues.append(open_brace_index)
+                open_brace_index = i
+            elif char == '}':
+                if open_brace_index >= 0:
+                    open_brace_index = -1
+                else:
+                    issues.append(i)
 
-        Parameters:
-            hed_ops (list, func, or HedOps): A HedOps, func or list of these to apply to hed strings in this sidecar.
-            name (str): If present, will use this as the filename for context, rather than using the actual filename
-                Useful for temp filenames.
-            extra_def_dicts (DefinitionDict, list, or None): If present use these in addition to sidecar's def dicts.
-            error_handler (ErrorHandler or None): Used to report errors.  Uses a default one if none passed in.
-            kwargs: See models.hed_ops.translate_ops or the specific hed_ops for additional options.
+        if open_brace_index >= 0:
+            issues.append(open_brace_index)
 
-        Returns:
-            list: The list of validation issues found. Individual issues are in the form of a dict.
+        return issues
 
-        """
-        if error_handler is None:
-            error_handler = error_reporter.ErrorHandler()
-        if not name:
-            name = self.name
-        if name:
-            error_handler.push_error_context(ErrorContext.FILE_NAME, name, False)
-
-        all_validation_issues = self.validate_structure(error_handler)
-
-        # Early out major errors so the rest of our code can assume they won't happen.
-        if all_validation_issues:
-            return all_validation_issues
-
-        hed_ops = self._standardize_ops(hed_ops)
-        def_mapper = self._add_definition_mapper(hed_ops, extra_def_dicts)
-        all_validation_issues += def_mapper.issues
-
-        for hed_string, key_name, issues in self.hed_string_iter(hed_ops=hed_ops, allow_placeholders=True,
-                                                                 error_handler=error_handler, **kwargs):
-            self.set_hed_string(hed_string, key_name)
-            all_validation_issues += issues
-
-        # Finally check what requires the final mapped data to check
-        for column_data in self.column_data:
-            validate_pound_func = partial(self._validate_pound_sign_count, column_type=column_data.column_type)
-            _, issues = apply_ops(column_data.hed_dict, validate_pound_func)
-            all_validation_issues += issues
-        all_validation_issues += self.def_dict.get_definition_issues()
-        if name:
-            error_handler.pop_error_context()
-        return all_validation_issues
+    @staticmethod
+    def _check_for_key(key, data):
+        if isinstance(data, dict):
+            if key in data:
+                return bool(data[key])
+            else:
+                for sub_data in data.values():
+                    result = SidecarValidator._check_for_key(key, sub_data)
+                    if result is not None:
+                        return result
+        elif isinstance(data, list):
+            for sub_data in data:
+                result = SidecarValidator._check_for_key(key, sub_data)
+                if result is not None:
+                    return result
+        return None
 
-    def extract_definitions(self, hed_schema=None, error_handler=None):
-        """ Gather and validate definitions in metadata.
+    def _validate_column_structure(self, column_name, dict_for_entry, error_handler):
+        """ Checks primarily for type errors such as expecting a string and getting a list in a json sidecar.
 
         Parameters:
-            error_handler (ErrorHandler): The error handler to use for context, uses a default one if None.
-            hed_schema (HedSchema or None): The schema to used to identify tags.
+            error_handler (ErrorHandler)  Sets the context for the error reporting. Cannot be None.
 
         Returns:
-            DefinitionDict: Contains all the definitions located in the column.
-            issues: List of issues encountered in extracting the definitions. Each issue is a dictionary.
+            list:  Issues in performing the operations. Each issue is a dictionary.
 
         """
-        if error_handler is None:
-            error_handler = ErrorHandler()
-        new_def_dict = DefinitionDict()
-        hed_ops = []
-        hed_ops.append(hed_schema)
-        hed_ops.append(new_def_dict)
-
-        all_issues = []
-        for hed_string, key_name, issues in self.hed_string_iter(hed_ops=hed_ops, allow_placeholders=True,
-                                                                 error_handler=error_handler):
-            all_issues += issues
+        val_issues = []
+        if column_name in self.reserved_column_names:
+            val_issues += error_handler.format_error_with_context(SidecarErrors.SIDECAR_HED_USED_COLUMN)
+            return val_issues
+
+        column_type = ColumnMetadata._detect_column_type(dict_for_entry=dict_for_entry)
+        if column_type is None:
+            val_issues += error_handler.format_error_with_context(SidecarErrors.UNKNOWN_COLUMN_TYPE,
+                                                                  column_name=column_name)
+        elif column_type == ColumnType.Ignore:
+            found_hed = self._check_for_key("HED", dict_for_entry)
+            if found_hed:
+                val_issues += error_handler.format_error_with_context(SidecarErrors.SIDECAR_HED_USED)
+        elif column_type == ColumnType.Categorical:
+            raw_hed_dict = dict_for_entry["HED"]
+            if not raw_hed_dict:
+                val_issues += error_handler.format_error_with_context(SidecarErrors.BLANK_HED_STRING)
+            if not isinstance(raw_hed_dict, dict):
+                val_issues += error_handler.format_error_with_context(SidecarErrors.WRONG_HED_DATA_TYPE,
+                                                                      given_type=type(raw_hed_dict),
+                                                                      expected_type="dict")
+            for key_name, hed_string in raw_hed_dict.items():
+                error_handler.push_error_context(ErrorContext.SIDECAR_KEY_NAME, key_name)
+                if not isinstance(hed_string, str):
+                    val_issues += error_handler.format_error_with_context(SidecarErrors.WRONG_HED_DATA_TYPE,
+                                                                          given_type=type(hed_string),
+                                                                          expected_type="str")
+                if not hed_string:
+                    val_issues += error_handler.format_error_with_context(SidecarErrors.BLANK_HED_STRING)
+                if key_name in self.reserved_category_values:
+                    val_issues += error_handler.format_error_with_context(SidecarErrors.SIDECAR_NA_USED, column_name)
+                error_handler.pop_error_context()
 
-        return new_def_dict
+        return val_issues
 
     def _validate_pound_sign_count(self, hed_string, column_type):
         """ Check if a given hed string in the column has the correct number of pound signs.
 
         Parameters:
             hed_string (str or HedString): HED string to be checked.
 
@@ -258,12 +252,27 @@
             presence of definition tags.
 
         """
         # Make a copy without definitions to check placeholder count.
         expected_count, error_type = ColumnMetadata.expected_pound_sign_count(column_type)
         hed_string_copy = copy.deepcopy(hed_string)
         hed_string_copy.remove_definitions()
+        hed_string_copy.shrink_defs()
 
         if hed_string_copy.lower().count("#") != expected_count:
             return ErrorHandler.format_error(error_type, pound_sign_count=str(hed_string_copy).count("#"))
 
         return []
+
+    def _check_definitions_bad_spot(self, definition_checks, error_handler):
+        issues = []
+        # This could be simplified now
+        for col_name, has_def in definition_checks.items():
+            error_handler.push_error_context(ErrorContext.SIDECAR_COLUMN_NAME, col_name)
+            def_check = set(bool(d) for d in has_def)
+            if len(def_check) != 1:
+                flat_def_list = [d for defs in has_def for d in defs]
+                for d in flat_def_list:
+                    issues += error_handler.format_error_with_context(DefinitionErrors.BAD_DEFINITION_LOCATION, d)
+            error_handler.pop_error_context()
+
+        return issues
```

### Comparing `hedtools-0.2.0/hed/models/timeseries_input.py` & `hedtools-0.3.0/hed/models/timeseries_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,8 +18,8 @@
 
         Notes:
              - The extra_def_dicts are external definitions that override the ones in the object.
 
         """
 
         super().__init__(file, file_type=".tsv", worksheet_name=None, has_column_names=False, mapper=None,
-                         def_mapper=None, name=name)
+                         name=name)
```

### Comparing `hedtools-0.2.0/hed/schema/__init__.py` & `hedtools-0.3.0/hed/schema/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ Data structures for handling the HED schema. """
 from .hed_schema import HedSchema
 from .hed_schema_entry import HedSchemaEntry, UnitClassEntry, UnitEntry, HedTagEntry
 from .hed_schema_group import HedSchemaGroup
 from .hed_schema_section import HedSchemaSection
-from .hed_schema_io import load_schema, load_schema_version, from_string, get_hed_xml_version, get_schema, \
-    get_schema_versions
+from .hed_schema_io import load_schema, load_schema_version, from_string, get_hed_xml_version, get_schema
 from .hed_schema_constants import HedKey, HedSectionKey
 from .hed_cache import cache_xml_versions, get_hed_versions, \
     get_path_from_hed_version, set_cache_directory, get_cache_directory
```

### Comparing `hedtools-0.2.0/hed/schema/hed_cache.py` & `hedtools-0.3.0/hed/schema/hed_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import shutil
 import os
 
 import json
 from hashlib import sha1
 from shutil import copyfile
+import urllib
 import re
 from semantic_version import Version
 import portalocker
 import time
 from hed.schema.schema_io.schema_util import url_to_file, make_url_request
 from pathlib import Path
 
@@ -84,15 +85,15 @@
     except FileNotFoundError:
         hed_files = []
     for hed_file in hed_files:
         expression_match = version_pattern.match(hed_file)
         if expression_match is not None:
             version = expression_match.group(3)
             found_library_name = expression_match.group(2)
-            if found_library_name != library_name:
+            if not get_libraries and found_library_name != library_name:
                 continue
             if found_library_name not in all_hed_versions:
                 all_hed_versions[found_library_name] = []
             all_hed_versions[found_library_name].append(version)
     for name, hed_versions in all_hed_versions.items():
         all_hed_versions[name] = _sort_version_list(hed_versions)
     if get_libraries:
@@ -265,15 +266,15 @@
                 all_hed_versions = _get_hed_xml_versions_from_url(hed_base_url, skip_folders=skip_folders,
                                                                   get_libraries=True)
                 for library_name, hed_versions in all_hed_versions.items():
                     for version, version_info in hed_versions.items():
                         _cache_hed_version(version, library_name, version_info, cache_folder=cache_folder)
 
             _write_last_cached_time(current_timestamp, cache_folder)
-    except portalocker.exceptions.LockException:
+    except portalocker.exceptions.LockException or ValueError:
         return -1
 
     return 0
 
 
 def _read_last_cached_time(cache_folder):
     """ Check the given cache folder to see when it was last updated.
@@ -298,14 +299,16 @@
 def _write_last_cached_time(new_time, cache_folder):
     """ Set the time of last cache update.
 
     Parameters:
         new_time (float): The time this was updated.
         cache_folder (str): The folder used for caching the hed schema.
 
+    :raises ValueError:
+        - something went wrong writing to the file
     """
     timestamp_filename = os.path.join(cache_folder, TIMESTAMP_FILENAME)
     try:
         with open(timestamp_filename, "w") as f:
             f.write(str(new_time))
     except Exception:
         raise ValueError("Error writing timestamp to hed cache")
@@ -367,17 +370,21 @@
     all_hed_versions = {}
     for file_entry in loaded_json:
         if file_entry['type'] == "dir":
             if hed_base_url.endswith(hedxml_suffix):
                 continue
             if file_entry['name'] in skip_folders:
                 continue
-            sub_folder_versions = \
-                _get_hed_xml_versions_from_url(hed_base_url + "/" + file_entry['name'] + hedxml_suffix,
-                                               skip_folders=skip_folders, get_libraries=True)
+            try:
+                sub_folder_versions = \
+                    _get_hed_xml_versions_from_url(hed_base_url + "/" + file_entry['name'] + hedxml_suffix,
+                                                   skip_folders=skip_folders, get_libraries=True)
+            except urllib.error.HTTPError as e:
+                # Silently ignore ones without a hedxml section for now.
+                continue
             _merge_in_versions(all_hed_versions, sub_folder_versions)
         expression_match = version_pattern.match(file_entry["name"])
         if expression_match is not None:
             version = expression_match.group(3)
             found_library_name = expression_match.group(2)
             if not get_libraries and found_library_name != library_name:
                 continue
```

### Comparing `hedtools-0.2.0/hed/schema/hed_schema.py` & `hedtools-0.3.0/hed/schema/hed_schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,182 +1,234 @@
+import os
+import shutil
 
 from hed.schema.hed_schema_constants import HedKey, HedSectionKey
+from hed.schema import hed_schema_constants as constants
 from hed.schema.schema_io import schema_util
 from hed.schema.schema_io.schema2xml import HedSchema2XML
 from hed.schema.schema_io.schema2wiki import HedSchema2Wiki
 
 from hed.schema import schema_validation_util
-from hed.schema.hed_schema_section import HedSchemaSection, HedSchemaTagSection
+from hed.schema.hed_schema_section import HedSchemaSection, HedSchemaTagSection, HedSchemaUnitClassSection
 from hed.errors import ErrorHandler
 from hed.errors.error_types import ValidationErrors
 
 
 class HedSchema:
     """ A HED schema suitable for processing. """
 
     def __init__(self):
         """ Constructor for the HedSchema class.
 
             A HedSchema can be used for validation, checking tag attributes, parsing tags, etc.
         """
         self._has_duplicate_tags = False
         self.header_attributes = {}
-        self._filename = None
+        self.filename = None
         self.prologue = ""
         self.epilogue = ""
 
         self._is_hed3_schema = None
-        # This is the specified library name_prefix - tags will be {schema_prefix}:{tag_name}
-        self._schema_prefix = ""
+        # This is the specified library name_prefix - tags will be {schema_namespace}:{tag_name}
+        self._namespace = ""
 
         self._sections = self._create_empty_sections()
 
     # ===============================================
     # Basic schema properties
     # ===============================================
     @property
-    def filename(self):
-        """ The filename if one is known.
-
-        Returns:
-            str: The filename of this schema.
-        """
-        return self._filename
-
-    @filename.setter
-    def filename(self, value):
-        """ Set the filename, if one has not already been set.
-
-        Parameters:
-            value (str): The source filename for this file
-        """
-        if self._filename is None:
-            self._filename = value
-
-    @property
     def version(self):
         """ The HED version of this schema.
 
         Returns:
             str: The version of this schema.
 
         """
         return self.header_attributes['version']
 
-    def get_formatted_version(self, as_string=True):
-        """ The HED version string including prefix and library name if any of this schema.
+    def get_formatted_version(self, as_string=False):
+        """ The HED version string including namespace and library name if any of this schema.
 
         Returns:
-            str: The complete version of this schema including library name and prefix.
+            str: The complete version of this schema including library name and namespace.
 
         """
-        library = self.header_attributes.get('library', '')
+        library = self.library
         if library:
             library = library + '_'
-        return self._schema_prefix + library + self.header_attributes.get('version', '')
+        return self._namespace + library + self.version
 
     @property
     def library(self):
         """ The name of this library schema if one exists.
 
         Returns:
-            str or None: Library name if any.
+            str: Library name if any.
 
         """
-        return self.header_attributes.get('library')
+        return self.header_attributes.get(constants.LIBRARY_ATTRIBUTE, "")
+
+    @property
+    def with_standard(self):
+        """ The version of the base schema this is extended from, if it exists..
+
+        Returns:
+            str: HED version or ""
+
+        """
+        return self.header_attributes.get(constants.WITH_STANDARD_ATTRIBUTE, "")
+
+    @property
+    def merged(self):
+        """ Returns if this schema was loaded from a merged file
+
+        Returns:
+            bool: True if file was loaded from a merged file
 
-    def schema_for_prefix(self, prefix):
-        """ Return HedSchema object for this prefix.
+
+        """
+        return not self.header_attributes.get(constants.UNMERGED_ATTRIBUTE, "")
+
+    def get_save_header_attributes(self, save_merged=False):
+        """ returns the attributes that should be saved.
+
+        """
+        sort_to_start = "!!!!!!!!!!!!!!"
+        header_attributes = dict(sorted(self.header_attributes.items(),
+                                        key=lambda x: sort_to_start if x[0] == constants.VERSION_ATTRIBUTE else x[0],
+                                        reverse=False))
+        if save_merged:
+            header_attributes.pop(constants.UNMERGED_ATTRIBUTE, None)
+        else:
+            # make sure it's the last attribute(just to make sure it's in an order)
+            header_attributes.pop(constants.UNMERGED_ATTRIBUTE, None)
+            header_attributes[constants.UNMERGED_ATTRIBUTE] = "True"
+
+        return header_attributes
+
+    def schema_for_namespace(self, namespace):
+        """ Return HedSchema object for this namespace.
 
         Parameters:
-            prefix (str): The schema library name prefix.
+            namespace (str): The schema library name namespace.
 
         Returns:
             HedSchema: The HED schema object for this schema.
 
         Notes:
             -This is mostly a placeholder for HedSchemaGroup and may be refactored out later.
 
         """
-        if self._schema_prefix != prefix:
+        if self._namespace != namespace:
             return None
         return self
 
     @property
     def valid_prefixes(self):
         """ Return a list of all prefixes this schema will accept
 
         Returns:
             list:   A list of valid tag prefixes for this schema.
 
         Notes:
             - The return value is always length 1 if using a HedSchema.
         """
-        return [self._schema_prefix]
+        return [self._namespace]
 
     # ===============================================
     # Creation and saving functions
     # ===============================================
-    def get_as_mediawiki_string(self):
+    def get_as_mediawiki_string(self, save_merged=False):
         """ Return the schema to a mediawiki string.
 
+        Parameters:
+            save_merged (bool): If true, this will save the schema as a merged schema if it is a "withStandard" schema.
+                                If it is not a "withStandard" schema, this setting has no effect.
+
         Returns:
             str:  The schema as a string in mediawiki format.
 
         """
         schema2wiki = HedSchema2Wiki()
-        output_strings = schema2wiki.process_schema(self)
+        output_strings = schema2wiki.process_schema(self, save_merged)
         return '\n'.join(output_strings)
 
-    def get_as_xml_string(self):
+    def get_as_xml_string(self, save_merged=True):
         """ Return the schema to an XML string.
 
+        Parameters:
+            save_merged (bool):
+            If true, this will save the schema as a merged schema if it is a "withStandard" schema.
+            If it is not a "withStandard" schema, this setting has no effect.
         Returns:
             str: Return the schema as an XML string.
 
         """
         schema2xml = HedSchema2XML()
-        xml_tree = schema2xml.process_schema(self)
+        xml_tree = schema2xml.process_schema(self, save_merged)
         return schema_util._xml_element_2_str(xml_tree)
 
-    def save_as_xml(self):
-        """ Save as XML to a temporary file.
-
-        Returns:
-            str: The name of the newly created schema file.
-
-        """
-        schema2xml = HedSchema2XML()
-        xml_tree = schema2xml.process_schema(self)
-        local_xml_file = schema_util.write_xml_tree_2_xml_file(xml_tree, ".xml")
-        return local_xml_file
-
-    def save_as_mediawiki(self):
+    def save_as_mediawiki(self, filename=None, save_merged=False):
         """ Save as mediawiki to a temporary file.
 
+        filename: str
+            If present, move the resulting file to this location.
+        save_merged: bool
+            If true, this will save the schema as a merged schema if it is a "withStandard" schema.
+            If it is not a "withStandard" schema, this setting has no effect.
+
         Returns:
             str:    The newly created schema filename.
-
         """
         schema2wiki = HedSchema2Wiki()
-        output_strings = schema2wiki.process_schema(self)
+        output_strings = schema2wiki.process_schema(self, save_merged)
         local_wiki_file = schema_util.write_strings_to_file(output_strings, ".mediawiki")
+        if filename:
+            directory = os.path.dirname(filename)
+            if directory and not os.path.exists(directory):
+                os.makedirs(directory)
+            shutil.move(local_wiki_file, filename)
+            return filename
         return local_wiki_file
 
-    def set_schema_prefix(self, schema_prefix):
-        """ Set library prefix associated for this schema.
+    def save_as_xml(self, filename=None, save_merged=True):
+        """ Save as XML to a temporary file.
+
+        filename: str
+            If present, move the resulting file to this location.
+        save_merged: bool
+            If true, this will save the schema as a merged schema if it is a "withStandard" schema.
+            If it is not a "withStandard" schema, this setting has no effect.
+
+        Returns:
+            str: The name of the newly created schema file.
+        """
+        schema2xml = HedSchema2XML()
+        xml_tree = schema2xml.process_schema(self, save_merged)
+        local_xml_file = schema_util.write_xml_tree_2_xml_file(xml_tree, ".xml")
+        if filename:
+            directory = os.path.dirname(filename)
+            if directory and not os.path.exists(directory):
+                os.makedirs(directory)
+            shutil.move(local_xml_file, filename)
+            return filename
+        return local_xml_file
+
+    def set_schema_prefix(self, schema_namespace):
+        """ Set library namespace associated for this schema.
 
         Parameters:
-            schema_prefix (str): Should be empty, or end with a colon.(Colon will be automated added if missing).
+            schema_namespace (str): Should be empty, or end with a colon.(Colon will be automated added if missing).
 
         """
-        if schema_prefix and schema_prefix[-1] != ":":
-            schema_prefix += ":"
+        if schema_namespace and schema_namespace[-1] != ":":
+            schema_namespace += ":"
 
-        self._schema_prefix = schema_prefix
+        self._namespace = schema_namespace
 
     def check_compliance(self, check_for_warnings=True, name=None, error_handler=None):
         """ Check for HED3 compliance of this schema.
 
         Parameters:
             check_for_warnings (bool): If True, also checks for formatting issues
             name (str): If present, use this as the filename for context
@@ -198,15 +250,15 @@
         """ Find all tags that are not unique.
 
         Returns:
             dict: A dictionary of all duplicate short tags
 
         Notes:
             - The returned dictionary has the short-form tags as keys and lists
-            of long tags sharing the short form as the values.
+              of long tags sharing the short form as the values.
 
         """
         return self.all_tags.duplicate_names
 
     def __getitem__(self, section_key):
         return self._sections[section_key]
 
@@ -257,14 +309,34 @@
         Returns:
             HedSchemaSection: The value classes section.
 
         """
         return self._sections[HedSectionKey.ValueClasses]
 
     @property
+    def attributes(self):
+        """ Return the attributes schema section.
+
+        Returns:
+            HedSchemaSection: The attributes section.
+
+        """
+        return self._sections[HedSectionKey.Attributes]
+
+    @property
+    def properties(self):
+        """ Return the properties schema section.
+
+        Returns:
+            HedSchemaSection: The properties section.
+
+        """
+        return self._sections[HedSectionKey.Properties]
+
+    @property
     def is_hed3_schema(self):
         """ Return true if this is at least version HED3.
 
         Returns:
             bool: True if this is a hed3 schema.
 
         Notes:
@@ -287,15 +359,15 @@
 
         Notes:
             - Matches must include attributes, tag names, etc.
 
         """
         if other is None:
             return False
-        if self.header_attributes != other.header_attributes:
+        if self.get_save_header_attributes() != other.get_save_header_attributes():
             return False
         if self._has_duplicate_tags != other._has_duplicate_tags:
             return False
         if self.prologue != other.prologue:
             return False
         if self.epilogue != other.epilogue:
             return False
@@ -312,18 +384,18 @@
             #                 if key not in dict1:
             #                     print(f"{key} not in dict1")
             #                     continue
             #                 if key not in dict2:
             #                     print(f"{key} not in dict2")
             #                     continue
             #                 if dict1[key] != dict2[key]:
-            #                     s = f"{key} unmatched: '{str(dict1[key].long_name)}' vs '{str(dict2[key].long_name)}'"
+            #                     s = f"{key} unmatched: '{str(dict1[key].name)}' vs '{str(dict2[key].name)}'"
             #                     print(s)
             return False
-        if self._schema_prefix != other._schema_prefix:
+        if self._namespace != other._namespace:
             return False
         return True
 
     def get_unit_class_units(self, unit_class_type):
         """ Get the list of unit class units this type will accept.
 
         Parameters:
@@ -334,53 +406,53 @@
 
         Examples:
             Eg 'time' returns ['second', 's', 'day', 'minute', 'hour']
 
         """
         unit_class_entry = self.get_tag_entry(unit_class_type, HedSectionKey.UnitClasses)
         if unit_class_entry:
-            return unit_class_entry.unit_class_units
+            return unit_class_entry.units
         return []
 
     def get_tags_with_attribute(self, key, section_key=HedSectionKey.AllTags):
         """ Return tag entries with the given attribute.
 
         Parameters:
             key (str): A tag attribute.  Eg HedKey.ExtensionAllowed
-            section_key (str): The HedSectionKey for the section to retrieve from.
+            section_key (HedSectionKey): The HedSectionKey for the section to retrieve from.
 
         Returns:
             list: A list of all tags with this attribute.
 
         Notes:
             - The result is cached so will be fast after first call.
 
         """
         return self._sections[section_key].get_entries_with_attribute(key, return_name_only=True,
-                                                                      schema_prefix=self._schema_prefix)
+                                                                      schema_namespace=self._namespace)
 
-    def get_tag_entry(self, name, key_class=HedSectionKey.AllTags, schema_prefix=""):
+    def get_tag_entry(self, name, key_class=HedSectionKey.AllTags, schema_namespace=""):
         """ Return the schema entry for this tag, if one exists.
 
         Parameters:
             name (str): Any form of basic tag(or other section entry) to look up.
                 This will not handle extensions or similar.
-                If this is a tag, it can have a schema prefix, but it's not required
+                If this is a tag, it can have a schema namespace, but it's not required
             key_class (HedSectionKey or str):  The type of entry to return.
-            schema_prefix (str): Only used on AllTags.  If incorrect, will return None.
+            schema_namespace (str): Only used on AllTags.  If incorrect, will return None.
 
         Returns:
             HedSchemaEntry: The schema entry for the given tag.
 
         """
         if key_class == HedSectionKey.AllTags:
-            if schema_prefix != self._schema_prefix:
+            if schema_namespace != self._namespace:
                 return None
-            if name.startswith(self._schema_prefix):
-                name = name[len(self._schema_prefix):]
+            if name.startswith(self._namespace):
+                name = name[len(self._namespace):]
 
         return self._get_tag_entry(name, key_class)
 
     def _get_tag_entry(self, name, key_class=HedSectionKey.AllTags):
         """ Return the schema entry for this tag, if one exists.
 
         Parameters:
@@ -390,58 +462,58 @@
 
         Returns:
             HedSchemaEntry: The schema entry for the given tag.
 
         """
         return self._sections[key_class].get(name)
 
-    def find_tag_entry(self, tag, schema_prefix=""):
+    def find_tag_entry(self, tag, schema_namespace=""):
         """ Find the schema entry for a given source tag.
 
-            Note: Will not identify tags if schema_prefix is set incorrectly
+            Note: Will not identify tags if schema_namespace is set incorrectly
 
         Parameters:
             tag (str, HedTag):     Any form of tag to look up.  Can have an extension, value, etc.
-            schema_prefix (str):  The schema prefix of the tag, if any.
+            schema_namespace (str):  The schema namespace of the tag, if any.
 
         Returns:
             HedTagEntry: The located tag entry for this tag.
             str: The remainder of the tag that isn't part of the base tag.
             list: A list of errors while converting.
 
         Notes:
             Works left to right (which is mostly relevant for errors).
 
         """
-        if schema_prefix != self._schema_prefix:
+        if schema_namespace != self._namespace:
             validation_issues = ErrorHandler.format_error(ValidationErrors.HED_LIBRARY_UNMATCHED, tag,
-                                                          schema_prefix, self.valid_prefixes)
+                                                          schema_namespace, self.valid_prefixes)
             return None, None, validation_issues
-        return self._find_tag_entry(tag, schema_prefix)
+        return self._find_tag_entry(tag, schema_namespace)
 
-    def _find_tag_entry(self, tag, schema_prefix=""):
+    def _find_tag_entry(self, tag, schema_namespace=""):
         """ Find the schema entry for a given source tag.
 
         Parameters:
             tag (str, HedTag):     Any form of tag to look up.  Can have an extension, value, etc.
-            schema_prefix (str):  The schema prefix of the tag, if any.
+            schema_namespace (str):  The schema namespace of the tag, if any.
 
         Returns:
             HedTagEntry: The located tag entry for this tag.
             str: The remainder of the tag that isn't part of the base tag.
             list: A list of errors while converting.
 
         Notes:
             Works left to right (which is mostly relevant for errors).
 
         """
         clean_tag = str(tag)
-        prefix = schema_prefix
-        clean_tag = clean_tag[len(prefix):]
-        prefix_tag_adj = len(prefix)
+        namespace = schema_namespace
+        clean_tag = clean_tag[len(namespace):]
+        prefix_tag_adj = len(namespace)
         working_tag = clean_tag.lower()
 
         # Most tags are in the schema directly, so test that first
         found_entry = self._get_tag_entry(working_tag)
         if found_entry:
             # this handles the one special case where the actual tag contains "/#" instead of something specific.
             if working_tag.endswith("/#"):
@@ -507,23 +579,23 @@
         """ Call to finish loading. """
         self._is_hed3_schema = self.is_hed3_schema
         self._has_duplicate_tags = bool(self.all_tags.duplicate_names)
         self._update_all_entries()
 
     def _update_all_entries(self):
         """ Call finalize_entry on every schema entry(tag, unit, etc). """
-        for section in self._sections.values():
-            for entry in section.values():
-                entry.finalize_entry(self)
+        for key_class, section in self._sections.items():
+            self._initialize_attributes(key_class)
+            section._finalize_section(self)
 
     def _initialize_attributes(self, key_class):
         """ Set the valid attributes for a section.
 
         Parameters:
-            key_class (str): The section key for the section to update.
+            key_class (HedSectionKey): The section key for the section to update.
 
         """
         self._sections[key_class].valid_attributes = self._get_attributes_for_section(key_class)
 
     # ===============================================
     # Getters used to write out schema primarily.
     # ===============================================
@@ -569,26 +641,26 @@
         """
         final_list = []
         for lower_tag, tag_entry in self.all_tags.items():
             if return_last_term:
                 final_list.append(tag_entry.name.split('/')[-1])
             else:
                 final_list.append(tag_entry.name)
+
         return final_list
 
     def get_unknown_attributes(self):
         """ Retrieve the current list of unknown attributes.
 
         Returns:
             dict: The keys are attribute names and the values are lists of tags with this attribute.
 
         Notes:
-            This includes attributes found in the wrong section for example
-                unitClass attribute found on a Tag.
-            The return tag list is in long form.
+            - This includes attributes found in the wrong section for example unitClass attribute found on a Tag.
+            - The return tag list is in long form.
 
         """
         unknown_attributes = {}
         for section in self._sections.values():
             for entry in section.values():
                 if entry._unknown_attributes:
                     for attribute_name in entry._unknown_attributes:
@@ -637,15 +709,15 @@
     def _create_empty_sections():
         dictionaries = {}
         # Add main sections
         dictionaries[HedSectionKey.Properties] = HedSchemaSection(HedSectionKey.Properties)
         dictionaries[HedSectionKey.Attributes] = HedSchemaSection(HedSectionKey.Attributes)
         dictionaries[HedSectionKey.UnitModifiers] = HedSchemaSection(HedSectionKey.UnitModifiers)
         dictionaries[HedSectionKey.Units] = HedSchemaSection(HedSectionKey.Units)
-        dictionaries[HedSectionKey.UnitClasses] = HedSchemaSection(HedSectionKey.UnitClasses)
+        dictionaries[HedSectionKey.UnitClasses] = HedSchemaUnitClassSection(HedSectionKey.UnitClasses)
         dictionaries[HedSectionKey.ValueClasses] = HedSchemaSection(HedSectionKey.ValueClasses)
         dictionaries[HedSectionKey.AllTags] = HedSchemaTagSection(HedSectionKey.AllTags, case_sensitive=False)
 
         return dictionaries
 
     def get_modifiers_for_unit(self, unit):
         """ Return the valid modifiers for the given unit
@@ -670,44 +742,62 @@
         if is_unit_symbol:
             modifier_attribute_name = HedKey.SIUnitSymbolModifier
         else:
             modifier_attribute_name = HedKey.SIUnitModifier
         valid_modifiers = self.unit_modifiers.get_entries_with_attribute(modifier_attribute_name)
         return valid_modifiers
 
+    def _add_element_property_attributes(self, attribute_dict):
+        attributes = {attribute: entry for attribute, entry in self._sections[HedSectionKey.Attributes].items()
+                      if entry.has_attribute(HedKey.ElementProperty)}
+
+        attribute_dict.update(attributes)
+
     def _get_attributes_for_section(self, key_class):
         """ Return the valid attributes for this section.
 
         Parameters:
-            key_class (str): The HedKey for this section.
+            key_class (HedSectionKey): The HedKey for this section.
 
         Returns:
             dict or HedSchemaSection: A dict of all the attributes and this section.
 
         """
         if key_class == HedSectionKey.AllTags:
             return self.get_tag_attribute_names()
         elif key_class == HedSectionKey.Attributes:
-            return self._sections[HedSectionKey.Properties]
+            prop_added_dict = {key: value for key, value in self._sections[HedSectionKey.Properties].items()}
+            self._add_element_property_attributes(prop_added_dict)
+            return prop_added_dict
+        elif key_class == HedSectionKey.Properties:
+            prop_added_dict = {}
+            self._add_element_property_attributes(prop_added_dict)
+            return prop_added_dict
         else:
             attrib_classes = {
                 HedSectionKey.UnitClasses: HedKey.UnitClassProperty,
                 HedSectionKey.Units: HedKey.UnitProperty,
                 HedSectionKey.UnitModifiers: HedKey.UnitModifierProperty,
                 HedSectionKey.ValueClasses: HedKey.ValueClassProperty
             }
             attrib_class = attrib_classes.get(key_class, None)
             if attrib_class is None:
                 return []
 
             attributes = {attribute: entry for attribute, entry in self._sections[HedSectionKey.Attributes].items()
-                          if entry.has_attribute(attrib_class)}
+                          if entry.has_attribute(attrib_class) or entry.has_attribute(HedKey.ElementProperty)}
             return attributes
 
     # ===============================================
     # Semi private function used to create a schema in memory(usually from a source file)
     # ===============================================
-    def _add_tag_to_dict(self, long_tag_name, key_class):
+    def _add_tag_to_dict(self, long_tag_name, new_entry, key_class):
+        # No reason we can't add this here always
+        if self.library and not self.merged and self.with_standard:
+            new_entry.set_attribute_value(HedKey.InLibrary, self.library)
+
         section = self._sections[key_class]
-        if not section:
-            self._initialize_attributes(key_class)
-        return section._add_to_dict(long_tag_name)
+        return section._add_to_dict(long_tag_name, new_entry)
+
+    def _create_tag_entry(self, long_tag_name, key_class):
+        section = self._sections[key_class]
+        return section._create_tag_entry(long_tag_name)
```

### Comparing `hedtools-0.2.0/hed/schema/hed_schema_constants.py` & `hedtools-0.3.0/hed/schema/hed_schema_constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
+from enum import Enum
 
-class HedSectionKey:
+class HedSectionKey(Enum):
     """ Kegs designating specific sections in a HedSchema object.
     """
     # overarching category listing all tags
     AllTags = 'tags'
     # Overarching category listing all unit classes
     UnitClasses = 'unitClasses'
     # Overarching category listing all units(not divided by type)
@@ -34,29 +35,37 @@
     TakesValue = 'takesValue'
     TopLevelTagGroup = 'topLevelTagGroup'
     Unique = 'unique'
     UnitClass = 'unitClass'
     ValueClass = "valueClass"
     RelatedTag = "relatedTag"
     SuggestedTag = "suggestedTag"
+    Rooted = "rooted"
 
     # All known properties
     BoolProperty = 'boolProperty'
     UnitClassProperty = 'unitClassProperty'
     UnitProperty = 'unitProperty'
     UnitModifierProperty = 'unitModifierProperty'
     ValueClassProperty = 'valueClassProperty'
+    ElementProperty = 'elementProperty'
 
     SIUnit = 'SIUnit'
     UnitSymbol = 'unitSymbol'
     # Default Units for Type
     DefaultUnits = 'defaultUnits'
     UnitPrefix = 'unitPrefix'
 
     SIUnitModifier = 'SIUnitModifier'
     SIUnitSymbolModifier = 'SIUnitSymbolModifier'
 
     # value class attributes
     AllowedCharacter = 'allowedCharacter'
 
+    # Node attributes
+    InLibrary = "inLibrary"
+
 
 VERSION_ATTRIBUTE = 'version'
+LIBRARY_ATTRIBUTE = 'library'
+WITH_STANDARD_ATTRIBUTE = "withStandard"
+UNMERGED_ATTRIBUTE = "unmerged"
```

### Comparing `hedtools-0.2.0/hed/schema/hed_schema_entry.py` & `hedtools-0.3.0/hed/schema/hed_schema_entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,15 +34,23 @@
     def finalize_entry(self, schema):
         """ Called once after loading to set internal state.
 
         Parameters:
             schema (HedSchema): The schema that holds the rules.
 
         """
-        pass
+        # Clear out any known attributes from the unknown section
+        to_remove = []
+        if self._unknown_attributes:
+            for attribute in self._unknown_attributes:
+                if attribute in self._section.valid_attributes:
+                    to_remove.append(attribute)
+
+            for item in to_remove:
+                self._unknown_attributes.pop(item)
 
     def set_attribute_value(self, attribute_name, attribute_value):
         """ Add attribute and set its value.
 
         Parameters:
             attribute_name (str): The name of the schema entry attribute.
             attribute_value (bool or str):  The value of the attribute.
@@ -50,14 +58,16 @@
         Notes:
             - If this an invalid attribute name, it will be also added as an unknown attribute.
 
         """
         if not attribute_value:
             return
 
+        # todo: remove this patch and redo the code
+        # This check doesn't need to be done if the schema is valid.
         if attribute_name not in self._section.valid_attributes:
             # print(f"Unknown attribute {attribute_name}")
             if self._unknown_attributes is None:
                 self._unknown_attributes = {}
             self._unknown_attributes[attribute_name] = attribute_value
         self.attributes[attribute_name] = attribute_value
 
@@ -91,14 +101,18 @@
             bool: Returns True if this entry has the property.
 
         """
         attr_entry = self._section.valid_attributes.get(attribute_name)
         if attr_entry and attr_entry.has_attribute(property_name):
             return True
 
+    @property
+    def section_key(self):
+        return self._section.section_key
+
     def __eq__(self, other):
         if self.name != other.name:
             return False
         if self.attributes != other.attributes:
             # We only want to compare known attributes
             self_attr = {key: value for key, value in self.attributes.items()
                          if not self._unknown_attributes or key not in self._unknown_attributes}
@@ -107,29 +121,28 @@
             if self_attr != other_attr:
                 return False
         if self.description != other.description:
             return False
         return True
 
     def __hash__(self):
-        return hash((self.name, self._section._section_key))
+        return hash(self.name)
 
     def __str__(self):
         return self.name
 
 
 class UnitClassEntry(HedSchemaEntry):
     """ A single unit class entry in the HedSchema. """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self._units = []
-        self.unit_class_units = []
+        self.units = []
         self.derivative_units = []
-        self.unit_class_entry = None
 
     def add_unit(self, unit_entry):
         """ Add the given unit entry to this unit class.
 
         Parameters:
             unit_entry (HedSchemaEntry): Unit entry to add.
 
@@ -140,26 +153,32 @@
         """ Called once after schema load to set state.
 
         Parameters:
             schema (HedSchema): The object with the schema rules.
 
         """
         derivative_units = {}
-        self.unit_class_units = {unit_entry.name: unit_entry for unit_entry in self._units}
-        for unit_name, unit_entry in self.unit_class_units.items():
+        self.units = {unit_entry.name: unit_entry for unit_entry in self._units}
+        for unit_name, unit_entry in self.units.items():
             new_derivative_units = [unit_name]
             if not unit_entry.has_attribute(HedKey.UnitSymbol):
                 new_derivative_units.append(pluralize.plural(unit_name))
 
             for derived_unit in new_derivative_units:
                 derivative_units[derived_unit] = unit_entry
                 for modifier in unit_entry.unit_modifiers:
                     derivative_units[modifier.name + derived_unit] = unit_entry
         self.derivative_units = derivative_units
 
+    def __eq__(self, other):
+        if not super().__eq__(other):
+            return False
+        if self.units != other.units:
+            return False
+        return True
 
 class UnitEntry(HedSchemaEntry):
     """ A single unit entry with modifiers in the HedSchema. """
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.unit_class_name = None
@@ -170,58 +189,27 @@
 
         Parameters:
             schema (HedSchema): The schema rules come from.
 
         """
         self.unit_modifiers = schema.get_modifiers_for_unit(self.name)
 
-
 class HedTagEntry(HedSchemaEntry):
     """ A single tag entry in the HedSchema. """
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.unit_classes = {}
         self.value_classes = {}
         # These always have any /# stripped off the end, so they can easily be used with normal code.
         self.long_tag_name = None
         self.short_tag_name = None
         self.takes_value_child_entry = None  # this is a child takes value tag, if one exists
         self._parent_tag = None
         self.tag_terms = tuple()
 
-    @staticmethod
-    def get_fake_tag_entry(tag, tags_to_identify):
-        """ Create a tag entry if a given a tag has a match in a list of possible short tags.
-
-        Parameters:
-            tag (str): The short/mid/long form tag to identify.
-            tags_to_identify (list): A list of lowercase short tags to identify.
-
-        Returns:
-            tuple:
-                - HedTagEntry or None: The fake entry showing the short tag name as the found tag.
-                - str: The remaining text after the located short tag, which may be empty.
-
-        Notes:
-             - The match is done left to right.
-
-        """
-        split_names = tag.split("/")
-        index = 0
-        for name in split_names:
-            if name.lower() in tags_to_identify:
-                fake_entry = HedTagEntry(name=tag[:index + len(name)], section=None)
-                fake_entry.long_tag_name = fake_entry.name
-                fake_entry.short_tag_name = name
-                return fake_entry, tag[index + len(name):]
-
-            index += len(name) + 1
-
-        return None, ""
-
     def any_parent_has_attribute(self, attribute):
         """ Check if tag (or parents) has the attribute.
 
         Parameters:
             attribute (str): The name of the attribute to check for.
 
         Returns:
@@ -253,14 +241,27 @@
         """
         base_entry = self
         if self.has_attribute(HedKey.TakesValue):
             base_entry = base_entry._parent_tag
 
         return base_entry.has_attribute(tag_attribute)
 
+    @property
+    def parent(self):
+        """Get the parent entry of this tag"""
+        return self._parent_tag
+
+    @property
+    def parent_name(self):
+        """Gets the parent tag entry name"""
+        if self._parent_tag:
+            return self._parent_tag.name
+        parent_name, _, child_name = self.name.rpartition("/")
+        return parent_name
+
     def finalize_entry(self, schema):
         """ Called once after schema loading to set state.
 
         Parameters:
             schema (HedSchema): The schema that the rules come from.
 
         """
```

### Comparing `hedtools-0.2.0/hed/schema/hed_schema_group.py` & `hedtools-0.3.0/hed/schema/hed_schema_group.py`

 * *Files 27% similar despite different names*

```diff
@@ -22,27 +22,27 @@
 
         Parameters:
             schema_list (list): A list of HedSchema for the container.
 
         Returns:
             HedSchemaGroup: the container created.
 
-        Raises:
-            HedFileError:  If multiple schemas have the same library prefixes.
-
+        :raises HedFileError:
+            - Multiple schemas have the same library prefixes.
+            - Empty list passed
         """
         if len(schema_list) == 0:
             raise HedFileError(HedExceptions.BAD_PARAMETERS, "Empty list passed to HedSchemaGroup constructor.",
                                filename="Combined Schema")
-        schema_prefixes = [hed_schema._schema_prefix for hed_schema in schema_list]
+        schema_prefixes = [hed_schema._namespace for hed_schema in schema_list]
         if len(set(schema_prefixes)) != len(schema_prefixes):
             raise HedFileError(HedExceptions.SCHEMA_DUPLICATE_PREFIX,
                                "Multiple schema share the same tag name_prefix.  This is not allowed.",
                                filename="Combined Schema")
-        self._schemas = {hed_schema._schema_prefix: hed_schema for hed_schema in schema_list}
+        self._schemas = {hed_schema._namespace: hed_schema for hed_schema in schema_list}
 
     # ===============================================
     # General schema properties/functions
     # ===============================================
 
     def get_formatted_version(self, as_string=True):
         x = [schema.get_formatted_version() for schema in self._schemas.values()]
@@ -83,25 +83,25 @@
     @property
     def value_classes(self):
         return all([schema.value_classes for schema in self._schemas.values()])
 
     def __eq__(self, other):
         return self._schemas == other._schemas
 
-    def schema_for_prefix(self, prefix):
-        """ Return the HedSchema for the library prefix.
+    def schema_for_namespace(self, namespace):
+        """ Return the HedSchema for the library namespace.
 
         Parameters:
-            prefix (str): A schema library name prefix.
+            namespace (str): A schema library name namespace.
 
         Returns:
-            HedSchema or None: The specific schema for this library name prefix if exists.
+            HedSchema or None: The specific schema for this library name namespace if exists.
 
         """
-        schema = self._schemas.get(prefix)
+        schema = self._schemas.get(namespace)
         return schema
 
     @property
     def valid_prefixes(self):
         """ Return a list of all prefixes this group will accept.
 
         Returns:
@@ -138,53 +138,53 @@
 
         """
         all_tags = set()
         for schema in self._schemas.values():
             all_tags.update(schema.get_tags_with_attribute(key))
         return all_tags
 
-    # todo: maybe tweak this API so you don't have to pass in library prefix?
-    def get_tag_entry(self, name, key_class=HedSectionKey.AllTags, schema_prefix=""):
+    # todo: maybe tweak this API so you don't have to pass in library namespace?
+    def get_tag_entry(self, name, key_class=HedSectionKey.AllTags, schema_namespace=""):
         """ Return the schema entry for this tag, if one exists.
 
         Parameters:
             name (str): Any form of basic tag(or other section entry) to look up.
             key_class (HedSectionKey): The tag section to search.
-            schema_prefix (str or None): An optional prefix associated with this tag.
+            schema_namespace (str or None): An optional namespace associated with this tag.
 
         Returns:
             HedSchemaEntry:  The schema entry for the given tag.
 
         Notes:
             - This will not handle extensions or similar.
 
         """
-        specific_schema = self.schema_for_prefix(schema_prefix)
+        specific_schema = self.schema_for_namespace(schema_namespace)
         if not specific_schema:
             return None
 
-        return specific_schema.get_tag_entry(name, key_class, schema_prefix)
+        return specific_schema.get_tag_entry(name, key_class, schema_namespace)
 
-    def find_tag_entry(self, tag, schema_prefix=""):
+    def find_tag_entry(self, tag, schema_namespace=""):
         """ Find a schema entry for a source tag.
 
         Parameters:
             tag (str or HedTag): Any form of tag to look up.  Can have an extension, value, etc.
-            schema_prefix (str): The prefix the library, if any.
+            schema_namespace (str): The namespace the library, if any.
 
         Returns:
             tuple:
                 - HedTagEntry: The located tag entry for this tag.
                 - str: The remainder of the tag that isn't part of the base tag.
                 - list: A list of errors while converting.
 
         Notes:
             - Works right to left.(mostly relevant for errors).
 
         """
-        specific_schema = self.schema_for_prefix(schema_prefix)
+        specific_schema = self.schema_for_namespace(schema_namespace)
         if not specific_schema:
             validation_issues = ErrorHandler.format_error(ValidationErrors.HED_LIBRARY_UNMATCHED, tag,
-                                                          schema_prefix, self.valid_prefixes)
+                                                          schema_namespace, self.valid_prefixes)
             return None, None, validation_issues
 
-        return specific_schema._find_tag_entry(tag, schema_prefix)
+        return specific_schema._find_tag_entry(tag, schema_namespace)
```

### Comparing `hedtools-0.2.0/hed/schema/hed_schema_io.py` & `hedtools-0.3.0/hed/schema/hed_schema_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 from hed.errors.exceptions import HedFileError, HedExceptions
 from hed.schema.hed_schema import HedSchema
 from hed.schema.schema_io import schema_util
 from hed.schema.hed_schema_group import HedSchemaGroup
 from hed.schema.schema_validation_util import validate_version_string
 
 
-def from_string(schema_string, file_type=".xml", schema_prefix=None):
+def from_string(schema_string, file_type=".xml", schema_namespace=None):
     """ Create a schema from the given string.
 
     Parameters:
         schema_string (str):         An XML or mediawiki file as a single long string.
         file_type (str):             The extension(including the .) corresponding to a file source.
-        schema_prefix (str, None):  The name_prefix all tags in this schema will accept.
+        schema_namespace (str, None):  The name_prefix all tags in this schema will accept.
 
     Returns:
         (HedSchema):  The loaded schema.
 
-    Raises:
-        HedFileError:  If empty string or invalid extension is passed.
+    :raises HedFileError:
+        - If empty string or invalid extension is passed.
+        - Other fatal formatting issues with file
 
     Notes:
         - The loading is determined by file type.
 
     """
     if not schema_string:
         raise HedFileError(HedExceptions.BAD_PARAMETERS, "Empty string passed to HedSchema.from_string",
@@ -36,16 +37,16 @@
     if file_type.endswith(".xml"):
         hed_schema = HedSchemaXMLParser.load_xml(schema_as_string=schema_string)
     elif file_type.endswith(".mediawiki"):
         hed_schema = HedSchemaWikiParser.load_wiki(schema_as_string=schema_string)
     else:
         raise HedFileError(HedExceptions.INVALID_EXTENSION, "Unknown schema extension", filename=file_type)
 
-    if schema_prefix:
-        hed_schema.set_schema_prefix(schema_prefix=schema_prefix)
+    if schema_namespace:
+        hed_schema.set_schema_prefix(schema_namespace=schema_namespace)
 
     return hed_schema
 
 
 def get_schema(hed_versions):
     if not hed_versions:
         return None
@@ -53,37 +54,28 @@
         return load_schema_version(hed_versions)
     elif isinstance(hed_versions, HedSchema) or isinstance(hed_versions, HedSchemaGroup):
         return hed_versions
     else:
         raise ValueError("InvalidHedSchemaOrSchemaVersion", "Expected schema or schema version")
 
 
-def get_schema_versions(hed_schema, as_string=True):
-    if not hed_schema and as_string:
-        return ''
-    elif not hed_schema:
-        return None
-    elif isinstance(hed_schema, HedSchema) or isinstance(hed_schema, HedSchemaGroup):
-        return hed_schema.get_formatted_version(as_string=as_string)
-    else:
-        raise ValueError("InvalidHedSchemaOrHedSchemaGroup", "Expected schema or schema group")
-
-
-def load_schema(hed_path=None, schema_prefix=None):
+def load_schema(hed_path=None, schema_namespace=None):
     """ Load a schema from the given file or URL path.
 
     Parameters:
         hed_path (str or None): A filepath or url to open a schema from.
-        schema_prefix (str or None): The name_prefix all tags in this schema will accept.
+        schema_namespace (str or None): The name_prefix all tags in this schema will accept.
 
     Returns:
         HedSchema: The loaded schema.
 
-    Raises:
-         HedFileError: If there are any fatal issues when loading the schema.
+    :raises HedFileError:
+        - Empty path passed
+        - Unknown extension
+        - Any fatal issues when loading the schema.
 
     """
     if not hed_path:
         raise HedFileError(HedExceptions.FILE_NOT_FOUND, "Empty file path passed to HedSchema.load_file",
                            filename=hed_path)
 
     is_url = hed_cache._check_if_url(hed_path)
@@ -94,79 +86,80 @@
     elif hed_path.lower().endswith(".xml"):
         hed_schema = HedSchemaXMLParser.load_xml(hed_path)
     elif hed_path.lower().endswith(".mediawiki"):
         hed_schema = HedSchemaWikiParser.load_wiki(hed_path)
     else:
         raise HedFileError(HedExceptions.INVALID_EXTENSION, "Unknown schema extension", filename=hed_path)
 
-    if schema_prefix:
-        hed_schema.set_schema_prefix(schema_prefix=schema_prefix)
+    if schema_namespace:
+        hed_schema.set_schema_prefix(schema_namespace=schema_namespace)
 
     return hed_schema
 
 
 # todo: this could be updated to also support .mediawiki format.
 def get_hed_xml_version(xml_file_path):
     """ Get the version number from a HED XML file.
 
     Parameters:
         xml_file_path (str): The path to a HED XML file.
 
     Returns:
         str: The version number of the HED XML file.
 
+    :raises HedFileError:
+        - There is an issue loading the schema
     """
     root_node = HedSchemaXMLParser._parse_hed_xml(xml_file_path)
     return root_node.attrib[hed_schema_constants.VERSION_ATTRIBUTE]
 
 
 def _load_schema_version(xml_version=None, xml_folder=None):
     """ Return specified version or latest if not specified.
 
     Parameters:
         xml_folder (str): Path to a folder containing schema.
-        xml_version (str or list): HED version format string. Expected format: '[schema_prefix:][library_name_]X.Y.Z'.
+        xml_version (str or list): HED version format string. Expected format: '[schema_namespace:][library_name_]X.Y.Z'.
 
     Returns:
         HedSchema or HedSchemaGroup: The requested HedSchema object.
 
-    Raises:
-        HedFileError: If the xml_version is not valid.
-
-    Notes:
-        - The library schema files have names of the form HED_(LIBRARY_NAME)_(version).xml.
+    :raises HedFileError:
+        - The xml_version is not valid.
+        - The specified version cannot be found or loaded
+        - Other fatal errors loading the schema (These are unlikely if you are not editing them locally)
     """
-    schema_prefix = ""
+    schema_namespace = ""
     library_name = None
     if xml_version:
         if ":" in xml_version:
-            schema_prefix, _, xml_version = xml_version.partition(":")
+            schema_namespace, _, xml_version = xml_version.partition(":")
         if "_" in xml_version:
             library_name, _, xml_version = xml_version.rpartition("_")
         elif validate_version_string(xml_version):
             library_name = xml_version
             xml_version = None
     try:
         final_hed_xml_file = hed_cache.get_hed_version_path(xml_version, library_name, xml_folder)
         if not final_hed_xml_file:
             hed_cache.cache_local_versions(xml_folder)
             final_hed_xml_file = hed_cache.get_hed_version_path(xml_version, library_name, xml_folder)
         hed_schema = load_schema(final_hed_xml_file)
     except HedFileError as e:
-        if e.error_type == HedExceptions.FILE_NOT_FOUND:
+        if e.code == HedExceptions.FILE_NOT_FOUND:
             hed_cache.cache_xml_versions(cache_folder=xml_folder)
             final_hed_xml_file = hed_cache.get_hed_version_path(xml_version, library_name, xml_folder)
             if not final_hed_xml_file:
                 raise HedFileError(HedExceptions.FILE_NOT_FOUND, f"HED version '{xml_version}' not found in cache: {hed_cache.get_cache_directory()}", filename=xml_folder)
             hed_schema = load_schema(final_hed_xml_file)
         else:
             raise e
 
-    if schema_prefix:
-        hed_schema.set_schema_prefix(schema_prefix=schema_prefix)
+    if schema_namespace:
+        hed_schema.set_schema_prefix(schema_namespace=schema_namespace)
 
     return hed_schema
 
 
 def load_schema_version(xml_version=None, xml_folder=None):
     """ Return a HedSchema or HedSchemaGroup extracted from xml_version field.
 
@@ -174,19 +167,17 @@
         xml_version (str or list or None): List or str specifying which official HED schemas to use.
                                            An empty string returns the latest version
         xml_folder (str): Path to a folder containing schema.
 
     Returns:
         HedSchema or HedSchemaGroup: The schema or schema group extracted.
 
-    Raises:
-        HedFileError: If the xml_version is not valid.
-
-    Notes:
-        - Loads the latest schema value if an empty version is given (string or list).
+    :raises HedFileError:
+        - The xml_version is not valid.
+        - A fatal error was encountered in parsing
     """
     if xml_version and isinstance(xml_version, list):
         schemas = [_load_schema_version(xml_version=version, xml_folder=xml_folder) for version in xml_version]
         if len(schemas) == 1:
             return schemas[0]
 
         return HedSchemaGroup(schemas)
```

### Comparing `hedtools-0.2.0/hed/schema/hed_schema_section.py` & `hedtools-0.3.0/hed/schema/hed_schema_section.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from hed.schema.hed_schema_entry import HedSchemaEntry, UnitClassEntry, UnitEntry, HedTagEntry
-from hed.schema.hed_schema_constants import HedSectionKey
+from hed.schema.hed_schema_constants import HedSectionKey, HedKey
 
 
 entries_by_section = {
     HedSectionKey.Properties: HedSchemaEntry,
     HedSectionKey.Attributes: HedSchemaEntry,
     HedSectionKey.UnitModifiers: HedSchemaEntry,
     HedSectionKey.Units: UnitEntry,
@@ -16,67 +16,85 @@
 class HedSchemaSection:
     """Container with entries in one section of the schema. """
 
     def __init__(self, section_key, case_sensitive=True):
         """ Construct schema section.
 
         Parameters:
-            section_key (str):  Name of the schema section.
-            case_sensitive (bool): If True, names are case sensitive.
+            section_key (HedSectionKey):  Name of the schema section.
+            case_sensitive (bool): If True, names are case-sensitive.
 
         """
         # {lower_case_name: HedSchemaEntry}
         self.all_names = {}
         self._section_key = section_key
         self.case_sensitive = case_sensitive
 
         # Points to the entries in attributes
         self.valid_attributes = {}
         self._attribute_cache = {}
 
         self._section_entry = entries_by_section.get(section_key)
-        self.duplicate_names = {}
+        self._duplicate_names = {}
+
         self.all_entries = []
 
-    def _add_to_dict(self, name):
-        """ Add a name to the dictionary for this section. """
-        name_key = name
-        if not self.case_sensitive:
-            name_key = name.lower()
+    @property
+    def section_key(self):
+        return self._section_key
+
+    @property
+    def duplicate_names(self):
+        return self._duplicate_names
 
+    def _create_tag_entry(self, name):
         new_entry = self._section_entry(name, self)
+        return new_entry
+
+    def _check_if_duplicate(self, name_key, new_entry):
+        return_entry = new_entry
         if name_key in self.all_names:
-            if name_key not in self.duplicate_names:
-                self.duplicate_names[name_key] = [self.all_names[name_key]]
-            self.duplicate_names[name_key].append(new_entry)
+            if name_key not in self._duplicate_names:
+                self._duplicate_names[name_key] = [self.all_names[name_key]]
+            self._duplicate_names[name_key].append(new_entry)
         else:
             self.all_names[name_key] = new_entry
 
+        return return_entry
+
+    def _add_to_dict(self, name, new_entry):
+        """ Add a name to the dictionary for this section. """
+        name_key = name
+        if not self.case_sensitive:
+            name_key = name.lower()
+
+        return_entry = self._check_if_duplicate(name_key, new_entry)
+
         self.all_entries.append(new_entry)
-        return new_entry
+        return return_entry
 
-    def get_entries_with_attribute(self, attribute_name, return_name_only=False, schema_prefix=""):
+    def get_entries_with_attribute(self, attribute_name, return_name_only=False, schema_namespace=""):
         """ Return entries or names with given attribute.
 
         Parameters:
             attribute_name (str): The name of the attribute(generally a HedKey entry).
             return_name_only (bool): If true, return the name as a string rather than the tag entry.
-            schema_prefix (str): Prepends given prefix to each name if returning names.
+            schema_namespace (str): Prepends given namespace to each name if returning names.
 
         Returns:
             list: List of HedSchemaEntry or strings representing the names.
 
         """
         if attribute_name not in self._attribute_cache:
             new_val = [tag_entry for tag_entry in self.values() if tag_entry.has_attribute(attribute_name)]
             self._attribute_cache[attribute_name] = new_val
 
         cache_val = self._attribute_cache[attribute_name]
         if return_name_only:
-            return [f"{schema_prefix}{tag_entry.name}" for tag_entry in cache_val]
+            return [f"{schema_namespace}{tag_entry.name}" for tag_entry in cache_val]
         return cache_val
 
     # ===============================================
     # Simple wrapper functions to make this class primarily function as a dict
     # ===============================================
     def __iter__(self):
         return iter(self.all_names)
@@ -122,51 +140,80 @@
         if self.duplicate_names != other.duplicate_names:
             return False
         return True
 
     def __bool__(self):
         return bool(self.all_names)
 
+    def _finalize_section(self, hed_schema):
+        for entry in self.values():
+            entry.finalize_entry(hed_schema)
+
+
+class HedSchemaUnitClassSection(HedSchemaSection):
+    def _check_if_duplicate(self, name_key, new_entry):
+        if name_key in self and len(new_entry.attributes) == 1\
+                    and HedKey.InLibrary in new_entry.attributes:
+            return self.all_names[name_key]
+        return super()._check_if_duplicate(name_key, new_entry)
+
 
 class HedSchemaTagSection(HedSchemaSection):
     """ A section of the schema. """
 
     def __init__(self, *args, case_sensitive=False, **kwargs):
         super().__init__(*args, **kwargs, case_sensitive=case_sensitive)
         # This dict contains all forms of all tags.  The .all_names variable has ONLY the long forms.
         self.long_form_tags = {}
 
-    def _add_to_dict(self, name):
+    @staticmethod
+    def _get_tag_forms(name):
         name_key = name
         tag_forms = []
         while name_key:
             tag_forms.append(name_key)
             slash_index = name_key.find("/")
             if slash_index == -1:
-                name_key = None
+                break
             else:
                 name_key = name_key[slash_index + 1:]
 
         # We can't add value tags by themselves
         if tag_forms[-1] == "#":
             tag_forms = tag_forms[:-1]
-        new_entry = super()._add_to_dict(name)
 
+        return name_key, tag_forms
+
+    def _create_tag_entry(self, name):
+        new_entry = super()._create_tag_entry(name)
+
+        _, tag_forms = self._get_tag_forms(name)
         # remove the /# if present, but only from the entry, not from the lookups
         # This lets us easily use source_tag + remainder instead of having to strip off the /# later.
         short_name = tag_forms[-1]
         long_tag_name = name
         if long_tag_name.endswith("/#"):
             long_tag_name = long_tag_name[:-2]
             short_name = short_name[:-2]
         new_entry.long_tag_name = long_tag_name
         new_entry.short_tag_name = short_name
 
-        for tag_key in tag_forms:
-            self.long_form_tags[tag_key.lower()] = new_entry
+        return new_entry
+
+    def _check_if_duplicate(self, name, new_entry):
+        name_key, tag_forms = self._get_tag_forms(name)
+        if name_key in self:
+            if name_key not in self._duplicate_names:
+                self._duplicate_names[name_key] = [self.get(name_key)]
+            self._duplicate_names[name_key].append(new_entry)
+        else:
+            self.all_names[name] = new_entry
+            for tag_key in tag_forms:
+                name_key = tag_key.lower()
+                self.long_form_tags[name_key] = new_entry
 
         return new_entry
 
     def get(self, key):
         if not self.case_sensitive:
             key = key.lower()
         return self.long_form_tags.get(key)
@@ -176,7 +223,40 @@
             key = key.lower()
         return self.long_form_tags[key]
 
     def __contains__(self, key):
         if not self.case_sensitive:
             key = key.lower()
         return key in self.long_form_tags
+
+    @staticmethod
+    def _divide_tags_into_dict(divide_list):
+        result = {}
+        for item in divide_list:
+            key, _, value = item.long_tag_name.partition('/')
+            if key not in result:
+                result[key] = []
+            result[key].append(item)
+
+        return list(result.values())
+
+    def _finalize_section(self, hed_schema):
+        split_list = self._divide_tags_into_dict(self.all_entries)
+
+        # Sort the extension allowed lists
+        extension_allowed_node = 0
+        for values in split_list:
+            node = values[0]
+            if node.has_attribute(HedKey.ExtensionAllowed):
+                # Make sure we sort / characters to the front.
+                values.sort(key=lambda x: x.long_tag_name.replace("/", "\0"))
+                extension_allowed_node += 1
+
+        # sort the top level nodes so extension allowed is at the bottom
+        split_list.sort(key=lambda x: x[0].has_attribute(HedKey.ExtensionAllowed))
+
+        # sort the extension allowed top level nodes
+        if extension_allowed_node:
+            split_list[extension_allowed_node:] = sorted(split_list[extension_allowed_node:], key=lambda x: x[0].long_tag_name)
+        self.all_entries = [subitem for tag_list in split_list for subitem in tag_list]
+        super()._finalize_section(hed_schema)
+
```

### Comparing `hedtools-0.2.0/hed/schema/schema_compliance.py` & `hedtools-0.3.0/hed/schema/schema_compliance.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,17 +17,16 @@
         check_for_warnings (bool): If True, check for formatting issues like invalid characters, capitalization, etc.
         name (str): If present, will use as filename for context.
         error_handler (ErrorHandler or None): Used to report errors. Uses a default one if none passed in.
 
     Returns:
         list: A list of all warnings and errors found in the file. Each issue is a dictionary.
 
-    Notes:
-        - Useful for temp filenames in support of web services.
-
+    :raises ValueError:
+        - Trying to validate a HedSchemaGroup directly
     """
     if not isinstance(hed_schema, HedSchema):
         raise ValueError("To check compliance of a HedGroupSchema, call self.check_compliance on the schema itself.")
 
     if error_handler is None:
         error_handler = error_reporter.ErrorHandler()
     issues_list = []
@@ -36,46 +35,53 @@
         name = hed_schema.filename
     error_handler.push_error_context(ErrorContext.FILE_NAME, name)
 
     unknown_attributes = hed_schema.get_unknown_attributes()
     if unknown_attributes:
         for attribute_name, source_tags in unknown_attributes.items():
             for tag in source_tags:
-                issues_list += error_handler.format_error_with_context(SchemaErrors.HED_SCHEMA_ATTRIBUTE_INVALID,
+                issues_list += error_handler.format_error_with_context(SchemaErrors.SCHEMA_ATTRIBUTE_INVALID,
                                                                        attribute_name,
                                                                        source_tag=tag)
 
     schema_attribute_validators = {
         HedKey.SuggestedTag: tag_exists_check,
         HedKey.RelatedTag: tag_exists_check,
         HedKey.UnitClass: tag_is_placeholder_check,
         HedKey.ValueClass: tag_is_placeholder_check,
+        HedKey.Rooted: tag_exists_base_schema_check,
     }
 
     # Check attributes
     for section_key in hed_schema._sections:
         error_handler.push_error_context(ErrorContext.SCHEMA_SECTION, section_key)
         # Check attributes
         for tag_entry in hed_schema[section_key].values():
             error_handler.push_error_context(ErrorContext.SCHEMA_TAG, tag_entry.name)
             for attribute_name in tag_entry.attributes:
                 validator = schema_attribute_validators.get(attribute_name)
                 if validator:
-                    error_handler.push_error_context(ErrorContext.SCHEMA_ATTRIBUTE, attribute_name, False)
-                    new_issues = validator(hed_schema, tag_entry, tag_entry.attributes[attribute_name])
-                    error_handler.add_context_to_issues(new_issues)
+                    error_handler.push_error_context(ErrorContext.SCHEMA_ATTRIBUTE, attribute_name)
+                    new_issues = validator(hed_schema, tag_entry, attribute_name)
+                    # if force_issues_as_warnings:
+                    for issue in new_issues:
+                        issue['severity'] = ErrorSeverity.WARNING
+                    error_handler.add_context_and_filter(new_issues)
                     issues_list += new_issues
                     error_handler.pop_error_context()
             error_handler.pop_error_context()
 
         # Check duplicate names
         for name, duplicate_entries in hed_schema[section_key].duplicate_names.items():
-            issues_list += error_handler.format_error_with_context(SchemaErrors.HED_SCHEMA_DUPLICATE_NODE, name,
-                                                                   duplicate_tag_list=[entry.name for entry in
-                                                                                       duplicate_entries],
+            values = set(entry.has_attribute(HedKey.InLibrary) for entry in duplicate_entries)
+            error_code = SchemaErrors.HED_SCHEMA_DUPLICATE_NODE
+            if len(values) == 2:
+                error_code = SchemaErrors.HED_SCHEMA_DUPLICATE_FROM_LIBRARY
+            issues_list += error_handler.format_error_with_context(error_code, name,
+                                                                   duplicate_tag_list=[entry.name for entry in duplicate_entries],
                                                                    section=section_key)
 
         error_handler.pop_error_context()
 
     if check_for_warnings:
         hed_terms = hed_schema.get_all_schema_tags(True)
         for hed_term in hed_terms:
@@ -83,65 +89,84 @@
 
         for tag_name, desc in hed_schema.get_desc_iter():
             issues_list += validate_schema_description(tag_name, desc)
 
     error_handler.pop_error_context()
     return issues_list
 
+# attribute_checker_template(hed_schema, tag_entry, attribute_name, possible_values):
+#     hed_schema (HedSchema): The schema to use for validation
+#     tag_entry (HedSchemaEntry): The schema entry for this tag.
+#     attribute_name (str): The name of this attribute
+
 
-def tag_is_placeholder_check(hed_schema, tag_entry, possible_tags, force_issues_as_warnings=True):
+def tag_is_placeholder_check(hed_schema, tag_entry, attribute_name):
     """ Check if comma separated list has valid HedTags.
 
     Parameters:
-        hed_schema (HedSchema): The schema to check if the tag exists.
+        hed_schema (HedSchema): The schema to use for validation
         tag_entry (HedSchemaEntry): The schema entry for this tag.
-        possible_tags (str): Comma separated list of tags.  Short long or mixed form valid.
-        force_issues_as_warnings (bool): If True sets all the severity levels to warning.
+        attribute_name (str): The name of this attribute
 
     Returns:
         list: A list of issues. Each issue is a dictionary.
 
     """
     issues = []
     if not tag_entry.name.endswith("/#"):
         issues += ErrorHandler.format_error(SchemaWarnings.NON_PLACEHOLDER_HAS_CLASS, tag_entry.name,
-                                            possible_tags)
-
-    if force_issues_as_warnings:
-        for issue in issues:
-            issue['severity'] = ErrorSeverity.WARNING
+                                            attribute_name)
 
     return issues
 
 
-def tag_exists_check(hed_schema, tag_entry, possible_tags, force_issues_as_warnings=True):
-    """ Check if comma separated list are valid HedTags.
+def tag_exists_check(hed_schema, tag_entry, attribute_name):
+    """ Check if the list of possible tags exists in the schema.
 
     Parameters:
-        hed_schema (HedSchema): The schema to check if the tag exists.
+        hed_schema (HedSchema): The schema to use for validation
         tag_entry (HedSchemaEntry): The schema entry for this tag.
-        possible_tags (str): Comma separated list of tags.  Short long or mixed form valid.
-        force_issues_as_warnings (bool): If True, set all the severity levels to warning.
+        attribute_name (str): The name of this attribute
 
     Returns:
         list: A list of issues. Each issue is a dictionary.
 
     """
     issues = []
+    possible_tags = tag_entry.attributes.get(attribute_name, "")
     split_tags = possible_tags.split(",")
     for org_tag in split_tags:
-        if org_tag not in hed_schema.all_tags:
+        if org_tag and org_tag not in hed_schema.all_tags:
             issues += ErrorHandler.format_error(ValidationErrors.NO_VALID_TAG_FOUND,
                                                 org_tag,
                                                 index_in_tag=0,
                                                 index_in_tag_end=len(org_tag))
 
-    if force_issues_as_warnings:
-        for issue in issues:
-            issue['severity'] = ErrorSeverity.WARNING
+    return issues
+
+
+def tag_exists_base_schema_check(hed_schema, tag_entry, attribute_name):
+    """ Check if the single tag is a partnered schema tag
+
+    Parameters:
+        hed_schema (HedSchema): The schema to use for validation
+        tag_entry (HedSchemaEntry): The schema entry for this tag.
+        attribute_name (str): The name of this attribute
+
+    Returns:
+        list: A list of issues. Each issue is a dictionary.
+    """
+    issues = []
+    rooted_tag = tag_entry.attributes.get(attribute_name, "")
+    if rooted_tag and rooted_tag not in hed_schema.all_tags:
+        issues += ErrorHandler.format_error(ValidationErrors.NO_VALID_TAG_FOUND,
+                                            rooted_tag,
+                                            index_in_tag=0,
+                                            index_in_tag_end=len(rooted_tag))
+
     return issues
 
 
 def validate_schema_term(hed_term):
     """ Check short tag for capitalization and illegal characters.
 
     Parameters:
```

### Comparing `hedtools-0.2.0/hed/schema/schema_data/HED8.0.0.xml` & `hedtools-0.3.0/hed/schema/schema_data/HED8.0.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/schema/schema_data/HED8.1.0.xml` & `hedtools-0.3.0/hed/schema/schema_data/HED8.1.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/schema/schema_data/HED_score_1.0.0.xml` & `hedtools-0.3.0/hed/schema/schema_data/HED_score_1.0.0.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/schema/schema_data/HED_testlib_1.0.2.xml` & `hedtools-0.3.0/hed/schema/schema_data/HED_testlib_1.0.2.xml`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/schema/schema_io/schema_util.py` & `hedtools-0.3.0/hed/schema/schema_io/schema_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,24 +20,23 @@
     try:
         return os.environ["HED_GITHUB_TOKEN"]
     except KeyError:
         return github_api_access_token
 
 
 def make_url_request(resource_url, try_authenticate=True):
-    """
-        Make sa request and adds the above Github access credentials
-    Args:
-        resource_url: str
-            The url to retrieve
-        try_authenticate: bool
-            If true add the above credentials
+    """ Make a request and adds the above Github access credentials.
+
+    Parameters:
+        resource_url (str): The url to retrieve.
+        try_authenticate (bool): If true add the above credentials.
 
     Returns:
         url_request
+
     """
     request = urllib.request.Request(resource_url)
     if try_authenticate and get_api_key():
         request.add_header('Authorization', 'token %s' % get_api_key())
     return urllib.request.urlopen(request)
```

### Comparing `hedtools-0.2.0/hed/schema/schema_io/wiki2schema.py` & `hedtools-0.3.0/hed/schema/schema_io/wiki2schema.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 This module is used to create a HedSchema object from a .mediawiki file.
 """
 import re
-from hed.schema.hed_schema_constants import HedSectionKey
+
+from hed.schema.hed_schema_constants import HedSectionKey, HedKey
 from hed.errors.exceptions import HedFileError, HedExceptions
+from hed.errors import ErrorContext, error_reporter
 from hed.schema import HedSchema
 from hed.schema import schema_validation_util
 from hed.schema.schema_io import wiki_constants
 
 header_attr_expression = "([^ ]+?)=\"(.*?)\""
 attr_re = re.compile(header_attr_expression)
 extend_here_line = 'extend here'
@@ -70,14 +72,15 @@
 
 class HedSchemaWikiParser:
     def __init__(self, wiki_file_path, schema_as_string):
         self.filename = wiki_file_path
         self.fatal_errors = []
         self._schema = HedSchema()
         self._schema.filename = wiki_file_path
+        self._loading_merged = True
 
         try:
             if wiki_file_path and schema_as_string:
                 raise HedFileError(HedExceptions.BAD_PARAMETERS, "Invalid parameters to schema creation.",
                                    wiki_file_path)
             if wiki_file_path:
                 with open(wiki_file_path, 'r', encoding='utf-8', errors='replace') as wiki_file:
@@ -87,15 +90,15 @@
                 wiki_lines = [line + "\n" for line in schema_as_string.split("\n")]
 
             self._read_wiki(wiki_lines)
         except FileNotFoundError as e:
             raise HedFileError(HedExceptions.FILE_NOT_FOUND, e.strerror, wiki_file_path)
 
         if self.fatal_errors:
-            self.fatal_errors.sort(key = lambda x: x.get("line_number", -1))
+            self.fatal_errors = error_reporter.sort_issues(self.fatal_errors)
             raise HedFileError(HedExceptions.HED_WIKI_DELIMITERS_INVALID,
                                f"{len(self.fatal_errors)} issues found when parsing schema.  See the .issues "
                                f"parameter on this exception for more details.", self.filename,
                                issues=self.fatal_errors)
         self._schema.finalize_dictionaries()
 
     @staticmethod
@@ -109,15 +112,29 @@
 
         Parameters
         ----------
         wiki_lines : iter(str)
             An opened .mediawiki file
         """
         # Read header line as we need it to determine if this is a hed3 schema or not before locating sections
-        self._read_header_line(wiki_lines[0])
+        self._read_header_line(wiki_lines)
+
+        if self._schema.with_standard and not self._schema.merged:
+            from hed.schema.hed_schema_io import load_schema_version
+            saved_attr = self._schema.header_attributes
+            try:
+                base_version = load_schema_version(self._schema.with_standard)
+            except HedFileError as e:
+                raise HedFileError(HedExceptions.BAD_WITH_STANDARD_VERSION,
+                                   message=f"Cannot load withStandard schema '{self._schema.with_standard}'",
+                                   filename=e.filename)
+            self._schema = base_version
+            self._schema.filename = self.filename
+            self._schema.header_attributes = saved_attr
+            self._loading_merged = False
 
         wiki_lines_by_section = self._split_lines_into_sections(wiki_lines)
         parse_order = {
             HedWikiSection.HeaderLine: self._read_header_section,
             HedWikiSection.Prologue: self._read_prologue,
             HedWikiSection.Epilogue: self._read_epilogue,
             HedWikiSection.Properties: self._read_properties,
@@ -199,21 +216,23 @@
 
     def _parse_sections(self, wiki_lines_by_section, parse_order):
         for section in parse_order:
             lines_for_section = wiki_lines_by_section.get(section, [])
             parse_func = parse_order[section]
             parse_func(lines_for_section)
 
-    def _read_header_line(self, line):
-        if line.startswith(wiki_constants.HEADER_LINE_STRING):
-            hed_attributes = self._get_header_attributes(line[len(wiki_constants.HEADER_LINE_STRING):])
-            schema_validation_util.validate_attributes(hed_attributes, filename=self.filename)
-            self.header_attributes = hed_attributes
-            self._schema.header_attributes = hed_attributes
-            return
+    def _read_header_line(self, lines):
+        line = ""
+        if lines:
+            line = lines[0]
+            if line.startswith(wiki_constants.HEADER_LINE_STRING):
+                hed_attributes = self._get_header_attributes(line[len(wiki_constants.HEADER_LINE_STRING):])
+                schema_validation_util.validate_attributes(hed_attributes, filename=self.filename)
+                self._schema.header_attributes = hed_attributes
+                return
         msg = f"First line of file should be HED, instead found: {line}"
         raise HedFileError(HedExceptions.SCHEMA_HEADER_MISSING, msg, filename=self.filename)
 
     def _read_header_section(self, lines):
         """Ensures the header has no content other than the initial line.
 
         Parameters
@@ -261,86 +280,108 @@
         """Adds the main schema section
 
         Parameters
         ----------
         lines: [(int, str)]
             Lines for this section
         """
+        self._schema._initialize_attributes(HedSectionKey.AllTags)
         parent_tags = []
+        level_adj = 0
         for line_number, line in lines:
             if line.startswith(wiki_constants.ROOT_TAG):
                 parent_tags = []
+                level_adj = 0
             else:
-                level = self._get_tag_level(line)
+                level = self._get_tag_level(line) + level_adj
                 if level < len(parent_tags):
                     parent_tags = parent_tags[:level]
                 elif level > len(parent_tags):
-                    self._add_fatal_error(line, "Line has too many *'s at the front.  You cannot skip a level.")
+                    self._add_fatal_error(line_number, line, "Line has too many *'s at the front.  You cannot skip a level.")
                     continue
-            new_tag_name = self._add_tag_line(parent_tags, line_number, line)
-            if not new_tag_name:
-                if new_tag_name != "":
-                    self._add_fatal_error(line_number, line)
+            # Create the entry
+            tag_entry = self._add_tag_line(parent_tags, line_number, line)
+
+            if not tag_entry:
+                # This will have already raised an error
                 continue
 
-            parent_tags.append(new_tag_name)
+            try:
+                rooted_entry = schema_validation_util.find_rooted_entry(tag_entry, self._schema, self._loading_merged)
+                if rooted_entry:
+                    parent_tags = rooted_entry.long_tag_name.split("/")
+                    level_adj = len(parent_tags)
+                    # Create the entry again for rooted tags, to get the full name.
+                    tag_entry = self._add_tag_line(parent_tags, line_number, line)
+            except HedFileError as e:
+                self._add_fatal_error(line_number, line, e.message, e.code)
+                continue
+
+            tag_entry = self._add_to_dict(line_number, line, tag_entry, HedSectionKey.AllTags)
+
+            parent_tags.append(tag_entry.short_tag_name)
 
     def _read_unit_classes(self, lines):
         """Adds the unit classes section
 
         Parameters
         ----------
         lines: [(int, str)]
             Lines for this section
         """
+        self._schema._initialize_attributes(HedSectionKey.UnitClasses)
+        self._schema._initialize_attributes(HedSectionKey.Units)
         unit_class_entry = None
         for line_number, line in lines:
-            unit_class_unit, _ = self._get_tag_name(line)
-            if unit_class_unit is None:
+            unit, _ = self._get_tag_name(line)
+            if unit is None:
                 self._add_fatal_error(line_number, line)
                 continue
             level = self._get_tag_level(line)
             # This is a unit class
             if level == 1:
-                unit_class_entry = self._add_single_line(line_number, line, HedSectionKey.UnitClasses)
+                unit_class_entry = self._create_entry(line_number, line, HedSectionKey.UnitClasses)
+                unit_class_entry = self._add_to_dict(line_number, line, unit_class_entry, HedSectionKey.UnitClasses)
             # This is a unit class unit
             else:
-                unit_class_unit_entry = self._add_single_line(line_number, line, HedSectionKey.Units)
+                unit_class_unit_entry = self._create_entry(line_number, line, HedSectionKey.Units)
+                self._add_to_dict(line_number, line, unit_class_unit_entry, HedSectionKey.Units)
                 unit_class_entry.add_unit(unit_class_unit_entry)
 
+    def _read_section(self, lines, section_key):
+        self._schema._initialize_attributes(section_key)
+        for line_number, line in lines:
+            new_entry = self._create_entry(line_number, line, section_key)
+            self._add_to_dict(line_number, line, new_entry, section_key)
+
     def _read_unit_modifiers(self, lines):
         """Adds the unit modifiers section
 
         Parameters
         ----------
         lines: [(int, str)]
             Lines for this section
         """
-        for line_number, line in lines:
-            self._add_single_line(line_number, line, HedSectionKey.UnitModifiers)
+        self._read_section(lines, HedSectionKey.UnitModifiers)
 
     def _read_value_classes(self, lines):
         """Adds the unit modifiers section
 
         Parameters
         ----------
         lines: [(int, str)]
             Lines for this section
         """
-        for line_number, line in lines:
-            self._add_single_line(line_number, line, HedSectionKey.ValueClasses)
+        self._read_section(lines, HedSectionKey.ValueClasses)
 
     def _read_properties(self, lines):
-        for line_number, line in lines:
-            self._add_single_line(line_number, line, HedSectionKey.Properties)
+        self._read_section(lines, HedSectionKey.Properties)
 
     def _read_attributes(self, lines):
-        self.attributes = {}
-        for line_number, line in lines:
-            self._add_single_line(line_number, line, HedSectionKey.Attributes)
+        self._read_section(lines, HedSectionKey.Attributes)
 
     def _get_header_attributes(self, version_line):
         """Extracts all valid attributes like version from the HED line in .mediawiki format.
 
         Parameters
         ----------
         version_line: string
@@ -384,14 +425,21 @@
             key, value = pair[:divider_index], pair[divider_index + 1:]
             key = key.strip()
             value = value.strip()
             final_attributes[key] = value
 
         return final_attributes
 
+    def _add_to_dict(self, line_number, line, entry, key_class):
+        if entry.has_attribute(HedKey.InLibrary) and not self._loading_merged:
+            self._add_fatal_error(line_number, line,
+                                  f"Library tag in unmerged schema has InLibrary attribute",
+                                  HedExceptions.IN_LIBRARY_IN_UNMERGED)
+        return self._schema._add_tag_to_dict(entry.name, entry, key_class)
+
     @staticmethod
     def _get_tag_level(tag_line):
         """ Get the tag level from a line in a wiki file.
 
         Parameters:
             tag_line (str): A tag line.
 
@@ -536,19 +584,20 @@
         """
         tag_name, _ = self._get_tag_name(tag_line)
         if tag_name:
             if parent_tags:
                 long_tag_name = "/".join(parent_tags) + "/" + tag_name
             else:
                 long_tag_name = tag_name
-            self._add_single_line(line_number, tag_line, HedSectionKey.AllTags, long_tag_name)
+            return self._create_entry(line_number, tag_line, HedSectionKey.AllTags, long_tag_name)
 
-        return tag_name
+        self._add_fatal_error(line_number, tag_line)
+        return None
 
-    def _add_single_line(self, line_number, tag_line, key_class, element_name=None):
+    def _create_entry(self, line_number, tag_line, key_class, element_name=None):
         node_name, index = self._get_tag_name(tag_line)
         if node_name is None:
             self._add_fatal_error(line_number, tag_line)
             return
         if element_name:
             node_name = element_name
 
@@ -558,21 +607,26 @@
             return
 
         node_desc, _ = self._get_line_section(tag_line, index)
         if node_desc is None:
             self._add_fatal_error(line_number, tag_line, "Description has mismatched delimiters")
             return
 
-        tag_entry = self._schema._add_tag_to_dict(node_name, key_class)
+        tag_entry = self._schema._create_tag_entry(node_name, key_class)
+
         if node_desc:
             tag_entry.description = node_desc.strip()
 
         for attribute_name, attribute_value in node_attributes.items():
             tag_entry.set_attribute_value(attribute_name, attribute_value)
 
         return tag_entry
 
-    def _add_fatal_error(self, line_number, line, warning_message="Schema term is empty or the line is malformed"):
+    def _add_fatal_error(self, line_number, line, warning_message="Schema term is empty or the line is malformed",
+                         error_code=HedExceptions.HED_WIKI_DELIMITERS_INVALID):
         self.fatal_errors.append(
-            {"line_number": line_number,
-             "line": line,
-             "message": warning_message})
+            {'code': error_code,
+             ErrorContext.ROW: line_number,
+             ErrorContext.LINE: line,
+             "message": f"ERROR: {warning_message}"
+             }
+        )
```

### Comparing `hedtools-0.2.0/hed/schema/schema_io/wiki_constants.py` & `hedtools-0.3.0/hed/schema/schema_io/wiki_constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ATTRIBUTE_PROPERTY_STRING = "'''Properties'''"
 VALUE_CLASS_STRING = "'''Value classes'''"
 PROLOGUE_SECTION_ELEMENT = "'''Prologue'''"
 EPILOGUE_SECTION_ELEMENT = "'''Epilogue'''"
 OLD_SYNTAX_SECTION_NAME = "'''Syntax'''"
 
 wiki_section_headers = {
-    HedSectionKey.AllTags: None,
+    HedSectionKey.AllTags: START_HED_STRING,
     HedSectionKey.UnitClasses: UNIT_CLASS_STRING,
     HedSectionKey.Units: None,
     HedSectionKey.UnitModifiers: UNIT_MODIFIER_STRING,
     HedSectionKey.ValueClasses: VALUE_CLASS_STRING,
     HedSectionKey.Attributes: ATTRIBUTE_DEFINITION_STRING,
     HedSectionKey.Properties: ATTRIBUTE_PROPERTY_STRING,
 }
```

### Comparing `hedtools-0.2.0/hed/schema/schema_io/xml_constants.py` & `hedtools-0.3.0/hed/schema/schema_io/xml_constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,57 +12,56 @@
 VALUE_ELEMENT = "value"
 
 # These should mostly match the HedKey values
 # These are repeated here for clarification primarily
 ATTRIBUTE_ELEMENT = "attribute"
 ATTRIBUTE_PROPERTY_ELEMENT = "property"
 UNIT_CLASS_UNIT_ELEMENT = 'unit'
-UNIT_CLASS_UNITS_ELEMENT = "units"
 PROLOGUE_ELEMENT = "prologue"
 SCHEMA_ELEMENT = "schema"
 EPILOGUE_ELEMENT = "epilogue"
 
 TAG_DEF_ELEMENT = "node"
 
-TRUE_ATTRIBUTE = "true"
-
 
 UNIT_CLASS_SECTION_ELEMENT = "unitClassDefinitions"
 UNIT_CLASS_DEF_ELEMENT = "unitClassDefinition"
 UNIT_MODIFIER_SECTION_ELEMENT = "unitModifierDefinitions"
 UNIT_MODIFIER_DEF_ELEMENT = "unitModifierDefinition"
 SCHEMA_ATTRIBUTES_SECTION_ELEMENT = "schemaAttributeDefinitions"
 SCHEMA_ATTRIBUTES_DEF_ELEMENT = "schemaAttributeDefinition"
 SCHEMA_PROPERTIES_SECTION_ELEMENT = "propertyDefinitions"
 SCHEMA_PROPERTIES_DEF_ELEMENT = "propertyDefinition"
 SCHEMA_VALUE_CLASSES_SECTION_ELEMENT = "valueClassDefinitions"
 SCHEMA_VALUE_CLASSES_DEF_ELEMENT = "valueClassDefinition"
 
 
 SECTION_NAMES = {
+    HedSectionKey.AllTags: SCHEMA_ELEMENT,
     HedSectionKey.UnitClasses: UNIT_CLASS_SECTION_ELEMENT,
     HedSectionKey.UnitModifiers: UNIT_MODIFIER_SECTION_ELEMENT,
     HedSectionKey.ValueClasses: SCHEMA_VALUE_CLASSES_SECTION_ELEMENT,
     HedSectionKey.Attributes: SCHEMA_ATTRIBUTES_SECTION_ELEMENT,
     HedSectionKey.Properties: SCHEMA_PROPERTIES_SECTION_ELEMENT,
 }
 
 
 ELEMENT_NAMES = {
     HedSectionKey.AllTags: TAG_DEF_ELEMENT,
     HedSectionKey.UnitClasses: UNIT_CLASS_DEF_ELEMENT,
+    HedSectionKey.Units: UNIT_CLASS_UNIT_ELEMENT,
     HedSectionKey.UnitModifiers: UNIT_MODIFIER_DEF_ELEMENT,
     HedSectionKey.ValueClasses: SCHEMA_VALUE_CLASSES_DEF_ELEMENT,
     HedSectionKey.Attributes: SCHEMA_ATTRIBUTES_DEF_ELEMENT,
     HedSectionKey.Properties: SCHEMA_PROPERTIES_DEF_ELEMENT,
 }
 
 
 ATTRIBUTE_PROPERTY_ELEMENTS = {
     HedSectionKey.AllTags: ATTRIBUTE_ELEMENT,
     HedSectionKey.UnitClasses: ATTRIBUTE_ELEMENT,
     HedSectionKey.Units: ATTRIBUTE_ELEMENT,
     HedSectionKey.UnitModifiers: ATTRIBUTE_ELEMENT,
     HedSectionKey.ValueClasses: ATTRIBUTE_ELEMENT,
     HedSectionKey.Attributes: ATTRIBUTE_PROPERTY_ELEMENT,
-    HedSectionKey.Properties: None
+    HedSectionKey.Properties: ATTRIBUTE_PROPERTY_ELEMENT
 }
```

### Comparing `hedtools-0.2.0/hed/tools/__init__.py` & `hedtools-0.3.0/hed/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from .bids.bids_file_group import BidsFileGroup
 from .bids.bids_sidecar_file import BidsSidecarFile
 from .bids.bids_tabular_dictionary import BidsTabularDictionary
 from .bids.bids_tabular_file import BidsTabularFile
 
 from .remodeling.dispatcher import Dispatcher
 from .remodeling.backup_manager import BackupManager
-from .remodeling.operations.base_context import BaseContext
+from .remodeling.operations.base_summary import BaseSummary
 from .remodeling.operations.base_op import BaseOp
 from .remodeling.operations.factor_column_op import FactorColumnOp
 from .remodeling.operations.factor_hed_tags_op import FactorHedTagsOp
 from .remodeling.operations.factor_hed_type_op import FactorHedTypeOp
 from .remodeling.operations.merge_consecutive_op import MergeConsecutiveOp
 from .remodeling.operations.number_groups_op import NumberGroupsOp
 from .remodeling.operations.number_rows_op import NumberRowsOp
@@ -36,19 +36,20 @@
 from .remodeling.operations.split_rows_op import SplitRowsOp
 from .remodeling.operations.summarize_column_names_op import SummarizeColumnNamesOp
 from .remodeling.operations.summarize_column_values_op import SummarizeColumnValuesOp
 from .remodeling.operations.summarize_hed_type_op import SummarizeHedTypeOp
 
 from .util.hed_logger import HedLogger
 from .util.data_util import get_new_dataframe, get_value_dict, replace_values, reorder_columns
-from .util.io_util import check_filename, generate_filename, extract_suffix_path, get_file_list, make_path
+from .util.io_util import check_filename, clean_filename, extract_suffix_path, get_file_list, make_path
 from .util.io_util import get_dir_dictionary, get_file_list, get_path_components, parse_bids_filename
 
 from .analysis import annotation_util
 from .analysis.annotation_util import \
     check_df_columns, extract_tags, generate_sidecar_entry, hed_to_df, df_to_hed, merge_hed_dict
 from .analysis import analysis_util
-from .analysis.analysis_util import assemble_hed, search_tabular, get_assembled_strings
+from .analysis.analysis_util import assemble_hed
+# from .analysis.analysis_util import search_tabular, get_assembled_strings
 
 from .remodeling.cli import run_remodel
 from .remodeling.cli import run_remodel_backup
 from .remodeling.cli import run_remodel_restore
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/annotation_util.py` & `hedtools-0.3.0/hed/tools/analysis/annotation_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/analysis/column_name_summary.py` & `hedtools-0.3.0/hed/tools/analysis/tabular_column_name_summary.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """ Summarizes the unique column names in a dataset. """
 
 import json
 
 
-class ColumnNameSummary:
+class TabularColumnNameSummary:
     def __init__(self, name=''):
         self.name = name
         self.file_dict = {}
         self.unique_headers = []
 
     def update(self, name, columns):
         position = self.update_headers(columns)
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/file_dictionary.py` & `hedtools-0.3.0/hed/tools/analysis/file_dictionary.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/analysis/hed_context_manager.py` & `hedtools-0.3.0/hed/tools/analysis/hed_context_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Manages context and events of temporal extent. """
 
 from hed.errors.exceptions import HedFileError
 from hed.models import HedGroup, HedString
 from hed.schema import HedSchema, HedSchemaGroup
 from hed.tools.analysis.analysis_util import hed_to_str
 
+#TODO: [Refactor] clean up distinction between hed as strings versus objects -- maybe replace by event manager.
 
 class OnsetGroup:
     def __init__(self, name, contents, start_index, end_index=None):
         self.name = name
         self.start_index = start_index
         self.end_index = end_index
         self.contents = hed_to_str(contents, remove_parentheses=True)
@@ -19,37 +20,44 @@
 
 class HedContextManager:
 
     def __init__(self, hed_strings, hed_schema):
         """ Create an context manager for an events file.
 
         Parameters:
-            hed_strings (list): A list of hed_strings to be managed.
+            hed_strings (list): A list of HedString objects to be managed.
+            hed_schema (HedSchema):  A HedSchema
 
-        Raises:
-            HedFileError: if there are any unmatched offsets.
+        :raises HedFileError:
+            - If there are any unmatched offsets.
 
         Notes:
             The constructor has the side-effect of splitting each element of the hed_strings list into two
             by removing the Offset groups and the Onset tags. The context has the temporal extent information.
             For users wanting to use only Onset events, self.hed_strings contains the information.
 
         """
 
-        self.hed_strings = [HedString(str(hed), hed_schema=hed_schema) for hed in hed_strings]
+        self.hed_strings = hed_strings
         if not isinstance(hed_schema, HedSchema) and not isinstance(hed_schema, HedSchemaGroup):
             raise ValueError("ContextRequiresSchema", f"Context manager must have a valid HedSchema of HedSchemaGroup")
         self.hed_schema = hed_schema
         self.onset_list = []
         self.onset_count = 0
         self.offset_count = 0
         self.contexts = []
         self._create_onset_list()
         self._set_event_contexts()
 
+    # def _extract_hed_objs(self, assembled):
+    #     hed_objs = [None for _ in range(len(assembled))]
+    #     for index, value in assembled["HED_assembled"].items():
+    #         hed_objs[index] = HedString(value, hed_schema=self.hed_schema)
+    #     return hed_objs
+    
     def iter_context(self):
         """ Iterate rows of context.
 
         Yields:
             HedString:  The HedString.
             HedStringGroup: Context
 
@@ -57,30 +65,30 @@
 
         for index in range(len(self.hed_strings)):
             yield self.hed_strings[index], self.contexts[index]
 
     def _create_onset_list(self):
         """ Create a list of events of extended duration.
 
-        Raises:
-            HedFileError: If the hed_strings contain unmatched offsets.
+        :raises HedFileError:
+            - If the hed_strings contain unmatched offsets.
 
         """
 
         self.onset_list = []
         onset_dict = {}
         for event_index, hed in enumerate(self.hed_strings):
             to_remove = []  # tag_tuples = hed.find_tags(['Onset'], recursive=False, include_groups=1)
-            onset_tuples = hed.find_tags(["onset"], recursive=True, include_groups=2)
+            onset_tuples = hed.find_top_level_tags(["onset"], include_groups=2)
             self.onset_count += len(onset_tuples)
             for tup in onset_tuples:
                 group = tup[1]
                 group.remove([tup[0]])
                 self._update_onset_list(group, onset_dict, event_index, is_offset=False)
-            offset_tuples = hed.find_tags(["offset"], recursive=True, include_groups=2)
+            offset_tuples = hed.find_top_level_tags(["offset"], include_groups=2)
             self.offset_count += len(offset_tuples)
             for tup in offset_tuples:
                 group = tup[1]
                 to_remove.append(group)
                 self._update_onset_list(group, onset_dict, event_index, is_offset=True)
             hed.remove(to_remove)
 
@@ -110,22 +118,22 @@
 
         Parameters:
             group (HedGroup):  The HedGroup containing the onset or offset.
             onset_dict (dict): A dictionary of OnsetGroup objects that keep track of span of an event.
             event_index (int): The event number in the list.
             is_offset (bool):  True if processing an offset.
 
-        Raises:
-            HedFileError if an unmatched offset is encountered.
+        :raises HedFileError:
+            - If an unmatched offset is encountered.
 
         Notes:
             - Modifies onset_dict and onset_list.
         """
         def_tags = group.find_def_tags(recursive=False, include_groups=0)
-        name = def_tags[0].extension_or_value_portion
+        name = def_tags[0].extension
         onset_element = onset_dict.pop(name, None)
         if onset_element:
             onset_element.end_index = event_index
             self.onset_list.append(onset_element)
         elif is_offset:
             raise HedFileError("UnmatchedOffset", f"Unmatched {name} offset at event {event_index}", " ")
         if not is_offset:
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/hed_type_counts.py` & `hedtools-0.3.0/hed/tools/analysis/hed_type_counts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """ Manages the counts of tags such as Condition-variable and task. """
 
 
 class HedTypeCount:
     """ Keeps a summary of one value of one type of variable.
 
     Parameters:
-        type_value (str)  The value of the variable to be counted
-        type_tag (str)   The type of variable.
+        type_value (str):  The value of the variable to be counted
+        type_tag (str):   The type of variable.
 
     Examples:
         HedTypeCounts('SymmetricCond', 'condition-variable') keeps counts of Condition-variable/Symmetric
 
     """
 
     def __init__(self, type_value, type_tag, file_name=None):
@@ -143,8 +143,8 @@
             self.files[file_id] = ''
 
     def get_summary(self):
         details = {}
         for type_value, count in self.type_dict.items():
             details[type_value] = count.get_summary()
         return {'name': str(self.name), 'type_tag': self.type_tag, 'files': list(self.files.keys()),
-                'total_events': self.total_events, 'details': details}
+                'total_events': self.total_events, 'details': details}
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/hed_type_definitions.py` & `hedtools-0.3.0/hed/tools/analysis/hed_type_definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """ Manages definitions associated with a type such as condition-variable. """
 
 from hed.models.hed_tag import HedTag
-from hed.models.def_mapper import DefMapper
+from hed.models.definition_dict import DefinitionDict
 
 
 class HedTypeDefinitions:
 
     def __init__(self, definitions, hed_schema, type_tag='condition-variable'):
         """ Create a definition manager for a type of variable.
 
         Parameters:
-            definitions (dict or DefMapper): A dictionary of DefinitionEntry objects.
+            definitions (dict or DefinitionDict): A dictionary of DefinitionEntry objects.
             hed_schema (Hedschema or HedSchemaGroup): The schema used for parsing.
             type_tag (str): Lower-case HED tag string representing the type managed.
 
+        # TODO: [Refactor] - should dict be allowed for definitions.
+
         """
 
         self.type_tag = type_tag.lower()
         self.hed_schema = hed_schema
-        if isinstance(definitions, DefMapper):
-            self.definitions = definitions.gathered_defs
+        if isinstance(definitions, DefinitionDict):
+            self.definitions = definitions.defs
         elif isinstance(definitions, dict):
             self.definitions = definitions
         else:
             self.definitions = {}
         self.def_map = self._extract_def_map()   # maps def names to conditions.
         self.type_map = self._extract_type_map()
 
@@ -83,19 +85,19 @@
         tag_list = entry.contents.get_all_tags()
         type_tag_values = []
         description = ''
         other_tags = []
         for hed_tag in tag_list:
             hed_tag.convert_to_canonical_forms(self.hed_schema)
             if hed_tag.short_base_tag.lower() == 'description':
-                description = hed_tag.extension_or_value_portion
+                description = hed_tag.extension
             elif hed_tag.short_base_tag.lower() != self.type_tag:
                 other_tags.append(hed_tag.short_base_tag)
             else:
-                value = hed_tag.extension_or_value_portion.lower()
+                value = hed_tag.extension.lower()
                 if value:
                     type_tag_values.append(value)
                 else:
                     type_tag_values.append(entry.name)
         return type_tag_values, description, other_tags
 
     @staticmethod
@@ -107,17 +109,17 @@
                no_value (bool):  If True, strip off extra values after the definition name.
 
            Returns:
                list:  A list of definition names (as strings).
 
            """
         if isinstance(item, HedTag) and 'def' in item.tag_terms:
-            names = [item.extension_or_value_portion.lower()]
+            names = [item.extension.lower()]
         else:
-            names = [tag.extension_or_value_portion.lower() for tag in item.get_all_tags() if 'def' in tag.tag_terms]
+            names = [tag.extension.lower() for tag in item.get_all_tags() if 'def' in tag.tag_terms]
         if no_value:
             for index, name in enumerate(names):
                 name, name_value = HedTypeDefinitions.split_name(name)
                 names[index] = name
         return names
 
     @staticmethod
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/hed_type_factors.py` & `hedtools-0.3.0/hed/tools/analysis/hed_type_factors.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/analysis/hed_type_manager.py` & `hedtools-0.3.0/hed/tools/analysis/hed_type_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,16 +12,17 @@
         """ Create a variable manager for one tabular file for all type variables.
 
         Parameters:
             hed_strings (list): A list of HED strings.
             hed_schema (HedSchema or HedSchemaGroup): The HED schema to use for processing.
             definitions (dict): A dictionary of DefinitionEntry objects.
 
-        Raises:
-            HedFileError:  On errors such as unmatched onsets or missing definitions.
+        :raises HedFileError:
+            - On errors such as unmatched onsets or missing definitions.
+
         """
 
         self.definitions = definitions
         self.context_manager = HedContextManager(hed_strings, hed_schema)
         self._type_tag_map = {}   # a map of type tag into HedTypeValues objects
 
     @property
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/hed_type_values.py` & `hedtools-0.3.0/hed/tools/analysis/hed_type_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
         Parameters:
             context_manager (HedContextManager): A list of HED strings.
             definitions (dict): A dictionary of DefinitionEntry objects.
             name (str): Name of the tabular file as a unique identifier.
             type_tag (str): Lowercase short form of the tag to be managed.
 
-        Raises:
-            HedFileError:  On errors such as unmatched onsets or missing definitions.
+        :raises HedFileError:
+            - On errors such as unmatched onsets or missing definitions.
 
         """
         self.name = name
         self.type_tag = type_tag.lower()
         self.definitions = HedTypeDefinitions(definitions, context_manager.hed_schema, type_tag=type_tag)
         hed_strings = context_manager.hed_strings
         hed_contexts = context_manager.contexts
@@ -137,15 +137,15 @@
             hed_vars (list): A list of names of the hed type_variables
             index (ind):  The event number associated with this.
 
         Notes:
             This modifies the HedTypeFactors map.
 
         """
-        level = tag.extension_or_value_portion.lower()
+        level = tag.extension.lower()
         for var_name in hed_vars:
             hed_var = self._type_value_map.get(var_name, None)
             if hed_var is None:
                 hed_var = HedTypeFactors(self.type_tag, var_name, self.total_events)
                 self._type_value_map[var_name] = hed_var
             var_levels = hed_var.levels.get(level, {index: 0})
             var_levels[index] = 0
@@ -181,15 +181,15 @@
 
         Parameters:
             tag_list (list): A list of Condition-variable HedTags.
             index (int):  An integer representing the position in an array
 
         """
         for tag in tag_list:
-            tag_value = tag.extension_or_value_portion.lower()
+            tag_value = tag.extension.lower()
             if not tag_value:
                 tag_value = self.type_tag
             hed_var = self._type_value_map.get(tag_value, None)
             if hed_var is None:
                 hed_var = HedTypeFactors(self.type_tag, tag_value, self.total_events)
             self._type_value_map[tag_value] = hed_var
             hed_var.direct_indices[index] = ''
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/key_map.py` & `hedtools-0.3.0/hed/tools/analysis/key_map.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,16 +59,16 @@
 
         Parameters:
             additional_cols (list or None): Optional list of additional columns to append to the returned dataframe.
 
         Returns:
             DataFrame:  A dataframe containing the template.
 
-        Raises:
-            HedFileError: If additional columns are not disjoint from the key columns.
+        :raises HedFileError:
+            - If additional columns are not disjoint from the key columns.
 
         Notes:
             -  The template consists of the unique key columns in this map plus additional columns.
 
         """
         if additional_cols and set(self.key_cols).intersection(additional_cols):
             raise HedFileError("AdditionalColumnsNotDisjoint",
@@ -86,16 +86,16 @@
             data (DataFrame, str):  Columnar data (either DataFrame or filename) whose columns are to be remapped.
 
         Returns:
             tuple:
                 - DataFrame: New dataframe with columns remapped.
                 - list:  List of row numbers that had no correspondence in the mapping.
 
-        Raises:
-            HedFileError:  If data is missing some of the key columns.
+        :raises HedFileError:
+            - If data is missing some of the key columns.
 
         """
 
         df_new = get_new_dataframe(data)
         present_keys, missing_keys = separate_values(df_new.columns.values.tolist(), self.key_cols)
         if missing_keys:
             raise HedFileError("MissingKeys", f"File must have key columns {str(self.key_cols)}", "")
@@ -141,16 +141,16 @@
             data (DataFrame or str):     DataFrame or filename of an events file or event map.
             allow_missing (bool):        If true allow missing keys and add as n/a columns.
             keep_counts (bool):          If true keep a count of the times each key is present.
 
         Returns:
             list: The indices of duplicates.
 
-        Raises:
-            HedFileError:  If there are missing keys and allow_missing is False.
+        :raises HedFileError:
+            - If there are missing keys and allow_missing is False.
 
         """
         df = get_new_dataframe(data)
         col_list = df.columns.values.tolist()
         keys_present, keys_missing = separate_values(col_list, self.key_cols)
         if keys_missing and not allow_missing:
             raise HedFileError("MissingKeyColumn",
```

### Comparing `hedtools-0.2.0/hed/tools/analysis/tabular_summary.py` & `hedtools-0.3.0/hed/tools/analysis/tabular_summary.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,14 +109,15 @@
         return counts
 
     def update(self, data, name=None):
         """ Update the counts based on data.
 
         Parameters:
             data (DataFrame, str, or list):    DataFrame containing data to update.
+            name (str): Name of the summary
 
         """
 
         if isinstance(data, list):
             for filename in data:
                 self._update_dataframe(filename, filename)
         elif isinstance(data, str):
```

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_dataset.py` & `hedtools-0.3.0/hed/tools/bids/bids_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,26 +75,22 @@
             types (list):  A list of strings indicating the file group types to be validated.
             check_for_warnings (bool):  If True, check for warnings.
 
         Returns:
             list:  List of issues encountered during validation. Each issue is a dictionary.
 
         """
-        validator = HedValidator(hed_schema=self.schema)
-        error_handler = ErrorHandler()
+
         if not types:
             types = list(self.tabular_files.keys())
         issues = []
         for tab_type in types:
             files = self.tabular_files[tab_type]
-            issues += files.validate_sidecars(hed_ops=[validator],
-                                              check_for_warnings=check_for_warnings, error_handler=error_handler)
-            issues += files.validate_datafiles(hed_ops=[validator],
-                                               check_for_warnings=check_for_warnings,
-                                               error_handler=error_handler)
+            issues += files.validate_sidecars(self.schema, check_for_warnings=check_for_warnings)
+            issues += files.validate_datafiles(self.schema, check_for_warnings=check_for_warnings)
         return issues
 
     def get_summary(self):
         """ Return an abbreviated summary of the dataset. """
         summary = {"dataset": self.dataset_description['Name'],
                    "hed_schema_versions": self.get_schema_versions(),
                    "file_group_types": f"{str(list(self.tabular_files.keys()))}"}
```

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_file.py` & `hedtools-0.3.0/hed/tools/bids/bids_file.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_file_dictionary.py` & `hedtools-0.3.0/hed/tools/bids/bids_file_dictionary.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,16 +16,16 @@
         """ Create the dictionary keyed to entities.
 
         Parameters:
             collection_name (str):      Name of this collection.
             files (list or dict):   Full paths of files to include.
             entities (tuple):  Entity names to use in creating the keys.
 
-        Raises:
-            HedFileError: If files has inappropriate values.
+        :raises HedFileError:
+            - If files has inappropriate values.
 
         Notes:
             - This function is used for cross listing BIDS style files for different studies.
 
         Examples:
             If entities is ('sub', 'ses', 'task', 'run'), a typical key might be sub-001_ses-01_task-memory_run-01.
 
@@ -113,16 +113,16 @@
         Parameters:
             files (list or dict):  List or dictionary of file-like objs to use.
             entities (tuple):   Tuple of entity names to use as keys, e.g. ('sub', 'run').
 
         Returns:
             dict:  A dictionary whose keys are entity keys and values are BidsFile objects.
 
-        Raises:
-            HedFileError: If incorrect format is passed or something not recognizable as a Bids file.
+        :raises HedFileError:
+            - If incorrect format is passed or something not recognizable as a Bids file.
 
         """
         file_dict = {}
 
         if isinstance(files, dict):
             files = files.values()
         elif not isinstance(files, list):
@@ -240,16 +240,16 @@
 
         Parameters:
             the_file (str or BidsFile): If a str, create a new BidsFile object, otherwise pass the original on.
 
         Returns:
             BidsFile:  Either the original file or a newly created BidsTabularFile.
 
-        Raises:
-            HedFileError: If the_file isn't str or BidsFile.
+        :raises HedFileError:
+            - If the_file isn't str or BidsFile.
 
         """
         if isinstance(the_file, str):
             the_file = BidsFile(the_file)
         elif not isinstance(the_file, BidsFile):
             raise HedFileError("BadBidsFileArgument",
                                f"_correct_file expects file path or BidsFile but found {str(the_file)}", [])
```

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_file_group.py` & `hedtools-0.3.0/hed/tools/bids/bids_file_group.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """ A group of BIDS files with specified suffix name. """
 
 import os
 from hed.errors.error_reporter import ErrorContext, ErrorHandler
+from hed.validator.sidecar_validator import SidecarValidator
+from hed.validator.spreadsheet_validator import SpreadsheetValidator
 from hed.tools.analysis.tabular_summary import TabularSummary
 from hed.tools.bids.bids_tabular_file import BidsTabularFile
 from hed.tools.bids.bids_sidecar_file import BidsSidecarFile
 from hed.tools.util.io_util import get_dir_dictionary, get_file_list, get_path_components
 
 
 class BidsFileGroup:
@@ -107,66 +109,60 @@
         """
         if self.obj_type != 'tabular':
             return None
         info = TabularSummary(value_cols=value_cols, skip_cols=skip_cols)
         info.update(list(self.datafile_dict.keys()))
         return info
 
-    def validate_sidecars(self, hed_ops, check_for_warnings=True, error_handler=None):
+    def validate_sidecars(self, hed_schema, extra_def_dicts=None, check_for_warnings=True):
         """ Validate merged sidecars.
 
         Parameters:
-            hed_ops ([func or HedOps], func, HedOps):  Validation functions to apply.
+            hed_schema (HedSchema):  HED schema for validation.
+            extra_def_dicts (DefinitionDict): Extra definitions
             check_for_warnings (bool):  If True, include warnings in the check.
-            error_handler (ErrorHandler): The common error handler for the dataset.
 
         Returns:
             list:   A list of validation issues found. Each issue is a dictionary.
 
         """
 
-        if not error_handler:
-            error_handler = ErrorHandler()
+        error_handler = ErrorHandler(check_for_warnings)
         issues = []
+        validator = SidecarValidator(hed_schema)
+        
         for sidecar in self.sidecar_dict.values():
-            error_handler.push_error_context(ErrorContext.FILE_NAME, sidecar.file_path)
-            if sidecar.has_hed:
-                issues += sidecar.contents.validate_entries(hed_ops=hed_ops,
-                                                            name=sidecar.file_path,
-                                                            check_for_warnings=check_for_warnings)
-                error_handler.pop_error_context()
+            name = os.path.basename(sidecar.file_path)
+            issues += validator.validate(sidecar.contents, extra_def_dicts=extra_def_dicts, name=name, 
+                                         error_handler=error_handler)
         return issues
 
-    def validate_datafiles(self, hed_ops, check_for_warnings=True, keep_contents=False, error_handler=None):
+    def validate_datafiles(self, hed_schema, extra_def_dicts=None, check_for_warnings=True, keep_contents=False):
         """ Validate the datafiles and return an error list.
 
         Parameters:
-            hed_ops ([func or HedOps], func, HedOps):  Validation functions to apply.
+            hed_schema (HedSchema):  Schema to apply to the validation.
+            extra_def_dicts (DefinitionDict):  Extra definitions that come from outside.
             check_for_warnings (bool):  If True, include warnings in the check.
             keep_contents (bool):       If True, the underlying data files are read and their contents retained.
-            error_handler (ErrorHandler): The common error handler to use for the dataset.
 
         Returns:
             list:    A list of validation issues found. Each issue is a dictionary.
 
         """
 
-        if not error_handler:
-            error_handler = ErrorHandler()
+        error_handler = ErrorHandler(check_for_warnings)
         issues = []
         for data_obj in self.datafile_dict.values():
-            error_handler.push_error_context(ErrorContext.FILE_NAME, data_obj.file_path)
             data_obj.set_contents(overwrite=False)
-            if not data_obj.has_hed:
-                continue
-            data = data_obj.contents
-            issues += data.validate_file(hed_ops=hed_ops, check_for_warnings=check_for_warnings)
+            name = os.path.basename(data_obj.file_path)
+            issues += data_obj.contents.validate(hed_schema, extra_def_dicts=None, name=name, 
+                                                 error_handler=error_handler)
             if not keep_contents:
                 data_obj.clear_contents()
-            error_handler.pop_error_context()
         return issues
 
     def _make_datafile_dict(self):
         """ Get a dictionary of objects  corresponding to the underlying obj_type with underlying contents unset.
 
         Returns:
             dict:   A dictionary of BidsTabularFile or BidsTimeseriesFile objects keyed by real path.
```

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_sidecar_file.py` & `hedtools-0.3.0/hed/tools/bids/bids_sidecar_file.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_tabular_dictionary.py` & `hedtools-0.3.0/hed/tools/bids/bids_tabular_dictionary.py`

 * *Files 1% similar despite different names*

```diff
@@ -186,16 +186,16 @@
 
         Parameters:
             the_file (str or BidsFile): If a str, create a new BidsTabularFile object,
                                         otherwise pass the original on.
         Returns:
             BidsTabularFile:  Either the original file or a newly created BidsTabularFile.
 
-        Raises:
-            HedFileError: If the_file isn't str or BidsTabularFile.
+        :raises HedFileError:
+            - If the_file isn't str or BidsTabularFile.
 
         """
         if isinstance(the_file, str):
             the_file = BidsTabularFile(the_file)
         elif not isinstance(the_file, BidsFile):
             raise HedFileError("BadArgument",
                                f"_correct_file needs file path or BidsFile type but found {str(the_file)}", [])
```

### Comparing `hedtools-0.2.0/hed/tools/bids/bids_tabular_file.py` & `hedtools-0.3.0/hed/tools/bids/bids_tabular_file.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/remodeling/backup_manager.py` & `hedtools-0.3.0/hed/tools/remodeling/backup_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,84 +6,96 @@
 from datetime import datetime
 from hed.errors.exceptions import HedFileError
 from hed.tools.util.io_util import get_file_list, get_path_components
 
 
 class BackupManager:
     DEFAULT_BACKUP_NAME = 'default_back'
-    RELATIVE_BACKUP_LOCATION = 'derivatives/remodel/backups'
+    RELATIVE_BACKUP_LOCATION = 'derivatives/remodel'
     BACKUP_DICTIONARY = 'backup_lock.json'
     BACKUP_ROOT = 'backup_root'
 
-    def __init__(self, data_root):
+    def __init__(self, data_root, backups_root=None):
         """ Constructor for the backup manager.
 
         Parameters:
-            data_root (str): full path of the root of the data directory.
+            data_root (str): Full path of the root of the data directory.
+            backups_root (str or None):  Full path to the root where backups subdirectory is located.
 
-        Raises:
-            - HedFileError:
-                - If the data_root does not correspond to a real directory.
+        :raises HedFileError:
+            - If the data_root does not correspond to a real directory.
 
         """
         if not os.path.isdir(data_root):
             raise HedFileError('NonExistentData', f"{data_root} is not an existing directory", "")
         self.data_root = data_root
-        self.backups_root = os.path.join(data_root, self.RELATIVE_BACKUP_LOCATION)
-        os.makedirs(self.backups_root, exist_ok=True)
+        if backups_root:
+            self.backups_path = os.path.join(backups_root, 'backups')
+        else:
+            self.backups_path = os.path.join(data_root, self.RELATIVE_BACKUP_LOCATION, 'backups')
+        self.backups_path = os.path.realpath(self.backups_path)
+        os.makedirs(self.backups_path, exist_ok=True)
         self.backups_dict = self._get_backups()
 
-    def create_backup(self, file_list, backup_name=None, verbose=True):
+    def create_backup(self, file_list, backup_name=None, verbose=False):
         """ Create a new backup from file_list.
 
         Parameters:
             file_list (list):   Full paths of the files to be in the backup.
             backup_name (str or None):  Name of the backup. If None, uses the default
             verbose (bool):     If True, print out the files that are being backed up.
 
         Returns:
             bool:  True if the backup was successful. False if a backup of that name already exists.
 
-        Raises:
-            Exceptions when file errors of any kind occur during the creation of a backup.
+        :raises HedFileError:
+            - For missing or incorrect files.
+
+        :raises OS-related error:
+            - OS-related error when file copying occurs.
 
         """
         if not backup_name:
             backup_name = self.DEFAULT_BACKUP_NAME
         if self.backups_dict and backup_name in self.backups_dict:
             return False
         backup = {}
         time_stamp = f"{str(datetime.now())}"
         if verbose:
             print(f"Creating backup {backup_name}")
-        backup_dir_path = os.path.realpath(os.path.join(self.backups_root, backup_name, BackupManager.BACKUP_ROOT))
+        backup_dir_path = os.path.realpath(os.path.join(self.backups_path, backup_name, BackupManager.BACKUP_ROOT))
         os.makedirs(backup_dir_path, exist_ok=True)
         for file in file_list:
             backup_file = self.get_backup_path(backup_name, file)
             os.makedirs(os.path.dirname(backup_file), exist_ok=True)
             if verbose:
                 print(f"Copying {file} to {backup_file}")
             shutil.copy2(file, backup_file)
             backup[self.get_file_key(file)] = time_stamp
         self.backups_dict[backup_name] = backup
-        backup_dict_path = os.path.realpath(os.path.join(self.backups_root, backup_name,
+        backup_dict_path = os.path.realpath(os.path.join(self.backups_path, backup_name,
                                                          self.BACKUP_DICTIONARY))
         with open(backup_dict_path, 'w') as fp:
             json.dump(backup, fp, indent=4)
         return True
 
     def get_backup(self, backup_name):
         """ Return the dictionary corresponding to backup_name.
 
         Parameters:
             backup_name (str): Name of the backup to be retrieved.
 
         Returns:
             The dictionary with the backup info.
 
+        Notes:
+            The dictionary with backup information has keys that are the paths of
+            the backed up files relative to the backup root. The values in this
+            dictionary are the dates on which the particular file was backed up.
+
         """
         if backup_name not in self.backups_dict:
             return None
         return self.backups_dict[backup_name]
 
     def get_backup_files(self, backup_name, original_paths=False):
         """ Returns a list of full paths of files contained in the backup.
@@ -91,39 +103,39 @@
         Parameters:
             backup_name (str):       Name of the backup.
             original_paths (bool):   If true return the original paths.
 
         Returns:
             list:  Full paths of the original files backed (original_paths=True) or the paths in the backup.
 
-        Raises:
-            HedFileError - if not backup named backup_name exists.
+        :raises HedFileError:
+            - If not backup named backup_name exists.
 
         """
 
         backup_dict = self.backups_dict.get(backup_name, None)
         if not backup_dict:
             raise HedFileError("NoBackup", f"{backup_name} is not a valid backup", "")
         if original_paths:
             return [os.path.realpath(os.path.join(self.data_root, backup_key)) for backup_key in backup_dict.keys()]
-        return [os.path.realpath(os.path.join(self.backups_root, backup_name, self.BACKUP_ROOT, backup_key))
+        return [os.path.realpath(os.path.join(self.backups_path, backup_name, self.BACKUP_ROOT, backup_key))
                 for backup_key in backup_dict.keys()]
 
     def get_backup_path(self, backup_name, file_name):
         """ Retrieve the file from the backup or throw an error.
 
         Parameters:
             backup_name (str): Name of the backup.
             file_name (str): Full path of the file to be retrieved.
 
         Returns:
             str:  Full path of the corresponding file in the backup.
 
         """
-        return os.path.realpath(os.path.join(self.backups_root, backup_name, self.BACKUP_ROOT,
+        return os.path.realpath(os.path.join(self.backups_path, backup_name, self.BACKUP_ROOT,
                                              self.get_file_key(file_name)))
 
     def get_file_key(self, file_name):
         file_comp = get_path_components(self.data_root, file_name) + [os.path.basename(file_name)]
         return '/'.join(file_comp)
 
     def restore_backup(self, backup_name=DEFAULT_BACKUP_NAME, task_names=[], verbose=True):
@@ -146,20 +158,21 @@
             if verbose:
                 print(f"Copying {file} to {data_files[index]}")
             shutil.copy2(file, data_files[index])
 
     def _get_backups(self):
         """ Set the manager's backup-dictionary based on backup directory contents.
 
-        Raises:
-            HedFileError - if a backup is inconsistent for any reason.
+        :raises HedFileError:
+            - If a backup is inconsistent for any reason.
+            
         """
         backups = {}
-        for backup in os.listdir(self.backups_root):
-            backup_root = os.path.realpath(os.path.join(self.backups_root, backup))
+        for backup in os.listdir(self.backups_path):
+            backup_root = os.path.realpath(os.path.join(self.backups_path, backup))
             if not os.path.isdir(backup_root):
                 raise HedFileError('BadBackupPath', f"{backup_root} is not a backup directory.", "")
             if len(os.listdir(backup_root)) != 2:
                 raise HedFileError("BadBackupFormat",
                                    f"Backup {backup_root} must only contain backup_root and backup_lock.json file.", "")
             backup_dict, files_not_in_backup, backups_not_in_directory = self._check_backup_consistency(backup)
             if files_not_in_backup:
@@ -182,20 +195,20 @@
             list:  Files in backup dictionary not in backup directory
 
         Notes:
             If file_path is None, this checks against consistency in the backup dictionary.
 
         """
 
-        backup_dict_path = os.path.realpath(os.path.join(self.backups_root, backup_name, self.BACKUP_DICTIONARY))
+        backup_dict_path = os.path.realpath(os.path.join(self.backups_path, backup_name, self.BACKUP_DICTIONARY))
         if not os.path.exists(backup_dict_path):
             raise HedFileError("BadBackupDictionaryPath",
                                f"Backup dictionary path {backup_dict_path} for backup "
                                f"{backup_name} does not exist so backup invalid", "")
-        backup_root_path = os.path.realpath(os.path.join(self.backups_root, backup_name, self.BACKUP_ROOT))
+        backup_root_path = os.path.realpath(os.path.join(self.backups_path, backup_name, self.BACKUP_ROOT))
         if not os.path.isdir(backup_root_path):
             raise HedFileError("BadBackupRootPath",
                                f"Backup root path {backup_root_path} for {backup_name} "
                                f"does not exist so backup invalid", "")
         with open(backup_dict_path, 'r') as fp:
             backup_dict = json.load(fp)
         backup_paths = set([os.path.realpath(os.path.join(backup_root_path, backup_key))
@@ -205,20 +218,20 @@
         backups_not_in_directory = list(backup_paths.difference(file_paths))
         return backup_dict, files_not_in_backup, backups_not_in_directory
 
     @staticmethod
     def get_task(task_names, file_path):
         """ Return the task if the file name contains a task_xxx where xxx is in task_names.
 
-        Args:
+        Parameters:
             task_names (list):  List of task names (without the task_ prefix).
             file_path (str):    Path of the filename to be tested.
 
         Returns:
-            str  the task name or '' if there is no task_xxx or xxx is not in task_names.
+            str:  the task name or '' if there is no task_xxx or xxx is not in task_names.
 
         """
 
         base = os.path.basename(file_path)
         for task in task_names:
             if ('task_' + task) in base:
                 return task
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/cli/run_remodel.py` & `hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,19 +7,19 @@
 from hed.tools.util.io_util import get_file_list
 from hed.tools.bids.bids_dataset import BidsDataset
 from hed.tools.remodeling.dispatcher import Dispatcher
 from hed.tools.remodeling.backup_manager import BackupManager
 
 
 def get_parser():
-    """ Create a parser for the run_remodel command-line arguments. 
-    
+    """ Create a parser for the run_remodel command-line arguments.
+
     Returns:
         argparse.ArgumentParser:  A parser for parsing the command line arguments.
-        
+
     """
     parser = argparse.ArgumentParser(description="Converts event files based on a json file specifying operations.")
     parser.add_argument("data_dir", help="Full path of dataset root directory.")
     parser.add_argument("remodel_path", help="Full path of the file with remodeling instructions.")
     parser.add_argument("-b", "--bids-format", action='store_true', dest="use_bids",
                         help="If present, the dataset is in BIDS format with sidecars. HED analysis is available.")
     parser.add_argument("-e", "--extensions", nargs="*", default=['.tsv'], dest="extensions",
@@ -29,39 +29,48 @@
     parser.add_argument("-i", "--individual-summaries", dest="individual_summaries", default="separate",
                         choices=["separate", "consolidated", "none"],
                         help="Controls individual file summaries ('none', 'separate', 'consolidated')")
     parser.add_argument("-j", "--json-sidecar", dest="json_sidecar", nargs="?",
                         help="Optional path to JSON sidecar with HED information")
     parser.add_argument("-n", "--backup-name", default=BackupManager.DEFAULT_BACKUP_NAME, dest="backup_name",
                         help="Name of the default backup for remodeling")
+    parser.add_argument("-nb", "--no-backup", action='store_true', dest="no_backup",
+                        help="If present, the operations are run directly on the files with no backup.")
+    parser.add_argument("-ns", "--no-summaries", action='store_true', dest="no_summaries",
+                        help="If present, the summaries are not saved, but rather discarded.")
+    parser.add_argument("-nu", "--no-update", action='store_true', dest="no_update",
+                        help="If present, the files are not saved, but rather discarded.")
     parser.add_argument("-r", "--hed-versions", dest="hed_versions", nargs="*", default=[],
                         help="Optional list of HED schema versions used for annotation, include prefixes.")
     parser.add_argument("-s", "--save-formats", nargs="*", default=['.json', '.txt'], dest="save_formats",
-                        help="Format for saving any summaries, if any. If empty, then no summaries are saved.")
+                        help="Format for saving any summaries, if any. If no summaries are to be written," +
+                             "use the -ns option.")
     parser.add_argument("-t", "--task-names", dest="task_names", nargs="*", default=[], help="The names of the task.")
     parser.add_argument("-v", "--verbose", action='store_true',
                         help="If present, output informative messages as computation progresses.")
+    parser.add_argument("-w", "--work-dir", default="", dest="work_dir",
+                        help="If given, is the path to directory for saving, otherwise derivatives/remodel is used.")
     parser.add_argument("-x", "--exclude-dirs", nargs="*", default=[], dest="exclude_dirs",
                         help="Directories names to exclude from search for files.")
     return parser
 
 
 def parse_arguments(arg_list=None):
-    """ Parse the command line arguments or arg_list if given. 
-    
+    """ Parse the command line arguments or arg_list if given.
+
     Parameters:
         arg_list (list):  List of command line arguments as a list.
-        
+
     Returns:
         Object:  Argument object
         List: A list of parsed operations (each operation is a dictionary).
-        
-    Raises:
-        ValueError  - If the operations were unable to be correctly parsed.
-    
+
+    :raises ValueError:
+        - If the operations were unable to be correctly parsed.
+
     """
     parser = get_parser()
     args = parser.parse_args(arg_list)
     if '*' in args.file_suffix:
         args.file_suffix = None
     if '*' in args.extensions:
         args.extensions = None
@@ -77,15 +86,15 @@
         raise ValueError("UnableToFullyParseOperations",
                          f"Fatal operation error, cannot continue:\n{Dispatcher.errors_to_str(errors)}")
     return args, operations
 
 
 def run_bids_ops(dispatch, args):
     """ Run the remodeler on a BIDS dataset.
-    
+
     Parameters:
         dispatch (Dispatcher): Manages the execution of the operations.
         args (Object): The command-line arguments as an object.
 
     """
     bids = BidsDataset(dispatch.data_root, tabular_types=['events'], exclude_dirs=args.exclude_dirs)
     dispatch.hed_schema = bids.schema
@@ -101,23 +110,24 @@
         if sidecar_list:
             sidecar = events.sidecar_dict[sidecar_list[-1]].contents
         else:
             sidecar = None
         if args.verbose:
             print(f"Events {events_obj.file_path}  sidecar {sidecar}")
         df = dispatch.run_operations(events_obj.file_path, sidecar=sidecar, verbose=args.verbose)
-        df.to_csv(events_obj.file_path, sep='\t', index=False, header=True)
+        if not args.no_update:
+            df.to_csv(events_obj.file_path, sep='\t', index=False, header=True)
 
 
 def run_direct_ops(dispatch, args):
     """ Run the remodeler on files of a specified form in a directory tree.
 
     Parameters:
         dispatch (Dispatcher):  Controls the application of the operations and backup.
-        args (dict): Dictionary of arguments and their values.
+        args (argparse.Namespace): Dictionary of arguments and their values.
 
     """
 
     tabular_files = get_file_list(dispatch.data_root, name_suffix=args.file_suffix, extensions=args.extensions,
                                   exclude_dirs=args.exclude_dirs)
     if args.verbose:
         print(f"Found {len(tabular_files)} files with suffix {args.file_suffix} and extensions {str(args.extensions)}")
@@ -125,43 +135,49 @@
         sidecar = args.json_sidecar
     else:
         sidecar = None
     for file_path in tabular_files:
         if args.task_names and not BackupManager.get_task(args.task_names, file_path):
             continue
         df = dispatch.run_operations(file_path, verbose=args.verbose, sidecar=sidecar)
-        df.to_csv(file_path, sep='\t', index=False, header=True)
+        if not args.no_update:
+            df.to_csv(file_path, sep='\t', index=False, header=True)
 
 
 def main(arg_list=None):
     """ The command-line program.
 
     Parameters:
         arg_list (list or None):   Called with value None when called from the command line.
                                    Otherwise, called with the command-line parameters as an argument list.
 
-    Raises:
-        HedFileError   
-            - if the data root directory does not exist.  
-            - if the specified backup does not exist.  
+    :raises HedFileError:
+        - if the data root directory does not exist.
+        - if the specified backup does not exist.
 
     """
     args, operations = parse_arguments(arg_list)
     if not os.path.isdir(args.data_dir):
         raise HedFileError("DataDirectoryDoesNotExist", f"The root data directory {args.data_dir} does not exist", "")
-    if args.backup_name:
+    if args.no_backup:
+        backup_name = None
+    else:
         backup_man = BackupManager(args.data_dir)
         if not backup_man.get_backup(args.backup_name):
             raise HedFileError("BackupDoesNotExist", f"Backup {args.backup_name} does not exist. "
                                f"Please run_remodel_backup first", "")
         backup_man.restore_backup(args.backup_name, args.task_names, verbose=args.verbose)
-    dispatch = Dispatcher(operations, data_root=args.data_dir, backup_name=args.backup_name,
-                          hed_versions=args.hed_versions)
+        backup_name = args.backup_name
+    dispatch = Dispatcher(operations, data_root=args.data_dir, backup_name=backup_name, hed_versions=args.hed_versions)
     if args.use_bids:
         run_bids_ops(dispatch, args)
     else:
         run_direct_ops(dispatch, args)
-    dispatch.save_summaries(args.save_formats, individual_summaries=args.individual_summaries)
+    save_dir = None
+    if args.work_dir:
+        save_dir = os.path.realpath(os.path.join(args.work_dir, Dispatcher.REMODELING_SUMMARY_PATH))
+    if not args.no_summaries:
+        dispatch.save_summaries(args.save_formats, individual_summaries=args.individual_summaries, summary_dir=save_dir)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/cli/run_remodel_backup.py` & `hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_backup.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,49 +17,58 @@
     parser.add_argument("data_dir", help="Full path of dataset root directory.")
     parser.add_argument("-e", "--extensions", nargs="*", default=['.tsv'], dest="extensions",
                         help="File extensions to allow in locating files. A * indicates all files allowed.")
     parser.add_argument("-f", "--file-suffix", dest="file_suffix", nargs="*", default=['events'],
                         help="Filename suffix of files to be backed up. A * indicates all files allowed.")
     parser.add_argument("-n", "--backup_name", default=BackupManager.DEFAULT_BACKUP_NAME, dest="backup_name",
                         help="Name of the default backup for remodeling")
+    parser.add_argument("-p", "--path-work", default="", dest="path_work",
+                        help="The root path for remodeling work if given, " +
+                             "otherwise [data_root]/derivatives/remodel is used.")
     parser.add_argument("-t", "--task-names", dest="task_names", nargs="*", default=[], help="The name of the task.")
     parser.add_argument("-v", "--verbose", action='store_true',
                         help="If present, output informative messages as computation progresses.")
+    parser.add_argument("-w", "--work-dir", default="", dest="work_dir",
+                        help="If given, is the path to directory for saving, " +
+                             "otherwise [data_root]derivatives/remodel is used.")
     parser.add_argument("-x", "--exclude-dirs", nargs="*", default=['derivatives'], dest="exclude_dirs",
                         help="Directories names to exclude from search for files. " +
                              "If omitted, no directories except the backup directory will be excluded." +
-                             "Note data_dir/remodel/backup will always be excluded.")
+                             "Note [data_root]/derivatives/remodel will always be excluded.")
     return parser
 
 
 def main(arg_list=None):
     """ The command-line program for making a remodel backup.
 
     Parameters:
         arg_list (list or None):   Called with value None when called from the command line.
                                    Otherwise, called with the command-line parameters as an argument list.
 
-    Raises:
-        HedFileError   
-            - if the specified backup already exists.  
+    :raises HedFileError:
+        - If the specified backup already exists.  
 
     """
 
     parser = get_parser()
     args = parser.parse_args(arg_list)
     if '*' in args.file_suffix:
         args.file_suffix = None
     if '*' in args.extensions:
         args.extensions = None
     exclude_dirs = args.exclude_dirs + ['remodeling']
     file_list = get_file_list(args.data_dir, name_suffix=args.file_suffix, extensions=args.extensions,
                               exclude_dirs=exclude_dirs)
     if args.task_names:
         file_list = get_filtered_by_element(file_list, args.task_names)
-    backup_man = BackupManager(args.data_dir)
+    if args.work_dir:
+        backups_root = args.work_dir
+    else:
+        backups_root = None
+    backup_man = BackupManager(args.data_dir, backups_root=backups_root)
     if backup_man.get_backup(args.backup_name):
         raise HedFileError("BackupExists", f"Backup {args.backup_name} already exists", "")
     else:
         backup_man.create_backup(file_list, backup_name=args.backup_name, verbose=args.verbose)
 
 
 if __name__ == '__main__':
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/cli/run_remodel_restore.py` & `hedtools-0.3.0/hed/tools/remodeling/cli/run_remodel_restore.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,35 +12,42 @@
         argparse.ArgumentParser:  A parser for parsing the command line arguments.
 
     """
     parser = argparse.ArgumentParser(description="Restores the backup files for the original data.")
     parser.add_argument("data_dir", help="Full path of dataset root directory.")
     parser.add_argument("-n", "--backup_name", default=BackupManager.DEFAULT_BACKUP_NAME, dest="backup_name",
                         help="Name of the default backup for remodeling")
+
     parser.add_argument("-t", "--task-names", dest="task_names", nargs="*", default=[], help="The names of the task.")
     parser.add_argument("-v", "--verbose", action='store_true',
                         help="If present, output informative messages as computation progresses.")
+    parser.add_argument("-w", "--work_dir", default="", dest="work_dir",
+                        help="The root path for remodeling work if given, " +
+                             "otherwise [data_root]/derivatives/remodel is used.")
     return parser
 
 
 def main(arg_list=None):
     """ The command-line program for restoring a remodel backup.
 
     Parameters:
         arg_list (list or None):   Called with value None when called from the command line.
                                    Otherwise, called with the command-line parameters as an argument list.
 
-    Raises:
-        HedFileError   
-            - if the specified backup does not exist.  
+    :raises HedFileError:
+        - if the specified backup does not exist.
 
     """
     parser = get_parser()
     args = parser.parse_args(arg_list)
-    backup_man = BackupManager(args.data_dir)
+    if args.work_dir:
+        backups_root = args.work_dir
+    else:
+        backups_root = None
+    backup_man = BackupManager(args.data_dir, backups_root=backups_root)
     if not backup_man.get_backup(args.backup_name):
         raise HedFileError("BackupDoesNotExist", f"{args.backup_name}", "")
     backup_man.restore_backup(args.backup_name, task_names=args.task_names, verbose=args.verbose)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/dispatcher.py` & `hedtools-0.3.0/hed/tools/remodeling/dispatcher.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 import numpy as np
 import pandas as pd
 import json
 from hed.errors.exceptions import HedFileError
 from hed.schema.hed_schema_io import get_schema
 from hed.tools.remodeling.backup_manager import BackupManager
 from hed.tools.remodeling.operations.valid_operations import valid_operations
-from hed.tools.util.io_util import generate_filename, extract_suffix_path, get_timestamp
+from hed.tools.util.io_util import clean_filename, extract_suffix_path, get_timestamp
 
 
 class Dispatcher:
     """ Controller for applying operations to tabular files and saving the results. """
 
-    REMODELING_SUMMARY_PATH = 'derivatives/remodel/summaries'
+    REMODELING_SUMMARY_PATH = 'remodel/summaries'
 
     def __init__(self, operation_list, data_root=None,
                  backup_name=BackupManager.DEFAULT_BACKUP_NAME, hed_versions=None):
         """ Constructor for the dispatcher.
 
         Parameters:
             operation_list (list): List of unparsed operations.
             data_root (str or None):  Root directory for the dataset. If none, then backups are not made.
             hed_versions (str, list, HedSchema, or HedSchemaGroup): The HED schema.
 
-        Raises:
-            HedFileError
-                - If the specified backup does not exist.
+        :raises HedFileError:
+            - If the specified backup does not exist.
+
+        :raises ValueError:
+            - If any of the operations cannot be parsed correctly.
 
-            - ValueError:
-                - If any of the operations cannot be parsed correctly.
         """
         self.data_root = data_root
         self.backup_name = backup_name
         self.backup_man = None
         if self.data_root and backup_name:
             self.backup_man = BackupManager(data_root)
             if not self.backup_man.get_backup(self.backup_name):
@@ -43,34 +43,34 @@
                                    f"{self.backup_name} backup for {self.data_root}", "")
         op_list, errors = self.parse_operations(operation_list)
         if errors:
             these_errors = self.errors_to_str(errors, 'Dispatcher failed due to invalid operations')
             raise ValueError("InvalidOperationList", f"{these_errors}")
         self.parsed_ops = op_list
         self.hed_schema = get_schema(hed_versions)
-        self.context_dict = {}
+        self.summary_dicts = {}
 
     def get_summaries(self, file_formats=['.txt', '.json']):
         """ Return the summaries in a dictionary of strings suitable for saving or archiving.
 
         Parameters:
             file_formats (list):  List of formats for the context files ('.json' and '.txt' are allowed).
 
         Returns:
             list: A list of dictionaries of summaries keyed to filenames.
 
         """
 
         summary_list = []
         time_stamp = '_' + get_timestamp()
-        for context_name, context_item in self.context_dict.items():
-            file_base = context_item.context_filename
+        for context_name, context_item in self.summary_dicts.items():
+            file_base = context_item.op.summary_filename
             if self.data_root:
                 file_base = extract_suffix_path(self.data_root, file_base)
-            file_base = generate_filename(file_base)
+            file_base = clean_filename(file_base)
             for file_format in file_formats:
                 if file_format == '.txt':
                     summary = context_item.get_text_summary(individual_summaries="consolidated")
                     summary = summary['Dataset']
                 elif file_format == '.json':
                     summary = json.dumps(context_item.get_summary(individual_summaries="consolidated"), indent=4)
 
@@ -85,24 +85,24 @@
 
         Parameters:
             file_designator (str, DataFrame ): A dataFrame or the full path of the dataframe in the original dataset.
 
         Returns:
             DataFrame:  DataFrame after reading the path.
 
-        Raises:
-            HedFileError:  If a valid file cannot be found.
+        :raises HedFileError:
+            - If a valid file cannot be found.
 
-        Note:
-        - If a string is passed and there is a backup manager,
-          the string must correspond to the full path of the file in the original dataset.
-          In this case, the corresponding backup file is read and returned.
-        - If a string is passed and there is no backup manager,
-          the data file corresponding to the file_designator is read and returned.
-        - If a Pandas DataFrame is passed, a copy is returned.
+        Notes:  
+            - If a string is passed and there is a backup manager,
+              the string must correspond to the full path of the file in the original dataset.
+              In this case, the corresponding backup file is read and returned.    
+            - If a string is passed and there is no backup manager,
+              the data file corresponding to the file_designator is read and returned.    
+            - If a Pandas DataFrame is passed, a copy is returned.    
 
         """
         if isinstance(file_designator, pd.DataFrame):
             return file_designator.copy()
         if self.backup_man:
             actual_path = self.backup_man.get_backup_path(self.backup_name, file_designator)
         else:
@@ -117,21 +117,21 @@
 
     def get_summary_save_dir(self):
         """ Return the directory in which to save the summaries.
 
         Returns:
             str: the data_root + remodeling summary path
 
-        Raises:
-            HedFileError  if this dispatcher does not have a data_root.
+        :raises HedFileError:
+            - If this dispatcher does not have a data_root.
 
         """
 
         if self.data_root:
-            return os.path.realpath(os.path.join(self.data_root, Dispatcher.REMODELING_SUMMARY_PATH))
+            return os.path.realpath(os.path.join(self.data_root, 'derivatives', Dispatcher.REMODELING_SUMMARY_PATH))
         raise HedFileError("NoDataRoot", f"Dispatcher must have a data root to produce directories", "")
 
     def run_operations(self, file_path, sidecar=None, verbose=False):
         """ Run the dispatcher operations on a file.
 
         Parameters:
             file_path (str or DataFrame):    Full path of the file to be remodeled or a DataFrame
@@ -155,25 +155,26 @@
 
     def save_summaries(self, save_formats=['.json', '.txt'], individual_summaries="separate", summary_dir=None):
         """ Save the summary files in the specified formats.
 
         Parameters:
             save_formats (list):  A list of formats [".txt", ."json"]
             individual_summaries (str): If True, include summaries of individual files.
-            summary_dir (str or None): Directory for saving summaries
+            summary_dir (str or None): Directory for saving summaries.
 
-        The summaries are saved in the dataset derivatives/remodeling folder if no save_dir is provided.
+        Notes:
+            The summaries are saved in the dataset derivatives/remodeling folder if no save_dir is provided.
 
         """
         if not save_formats:
             return
         if not summary_dir:
             summary_dir = self.get_summary_save_dir()
         os.makedirs(summary_dir, exist_ok=True)
-        for context_name, context_item in self.context_dict.items():
+        for context_name, context_item in self.summary_dicts.items():
             context_item.save(summary_dir, save_formats, individual_summaries=individual_summaries)
 
     @staticmethod
     def parse_operations(operation_list):
         errors = []
         operations = []
         for index, item in enumerate(operation_list):
@@ -198,15 +199,15 @@
                                "error_code": ex.args[0], "error_msg": ex.args[1]})
         if errors:
             return [], errors
         return operations, []
 
     @staticmethod
     def prep_data(df):
-        """ Replace all n/a entries in the data frame by np.NaN for processing.
+        """ Make a copy and replace all n/a entries in the data frame by np.NaN for processing.
 
         Parameters:
             df (DataFrame) - The DataFrame to be processed.
 
         """
         return df.replace('n/a', np.NaN)
 
@@ -217,14 +218,18 @@
         Parameters:
             df (DataFrame): The DataFrame to be processed.
 
         Returns:
             DataFrame: DataFrame with the 'np.NAN replaced by 'n/a'
 
         """
+        dtypes = df.dtypes.to_dict()
+        for col_name, typ in dtypes.items():
+            if typ == 'category':
+                df[col_name] = df[col_name].astype(str)
         return df.fillna('n/a')
 
     @staticmethod
     def errors_to_str(messages, title="", sep='\n'):
         error_list = [0]*len(messages)
         for index, message in enumerate(messages):
             error_list[index] = f"Operation[{message.get('index', None)}] " + \
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/base_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/base_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,24 +11,23 @@
     def __init__(self, op_spec, parameters):
         """ Base class constructor for operations.
 
         Parameters:
             op_spec (dict): Specification for required and optional parameters.
             parameters (dict):  Actual values of the parameters for the operation.
 
-        Raises:
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
-            ValueError   
-                - If the specification is missing a valid operation.   
+        :raises ValueError:
+            - If the specification is missing a valid operation.
 
         """
         self.operation = op_spec.get("operation", "")
         if not self.operation:
             raise ValueError("OpMustHaveOperation", "Op must have operation is empty")
         self.required_params = op_spec.get("required_parameters", {})
         self.optional_params = op_spec.get("optional_parameters", {})
@@ -36,22 +35,20 @@
 
     def check_parameters(self, parameters):
         """ Verify that the parameters meet the operation specification.
 
         Parameters:
             parameters (dict): Dictionary of parameters for this operation.
 
-        Raises:
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.    
-
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
 
         required = set(self.required_params.keys())
         required_missing = required.difference(set(parameters.keys()))
         if required_missing:
             raise KeyError("MissingRequiredParameters",
@@ -66,36 +63,36 @@
                                f"{param_name} not a required or optional parameter for {self.operation}")
             if isinstance(param_type, list):
                 self._check_list_type(param_value, param_type)
             elif not isinstance(param_value, param_type):
                 raise TypeError("BadType", f"{param_value} has type {type(param_value)} not {param_type}")
 
     def do_op(self, dispatcher, df, name, sidecar=None):
-        """ Base class method to be overridden with by each operation.
+        """ Base class method to be overridden by each operation.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The tabular file to be remodeled.
             name (str): Unique identifier for the data -- often the original file path.
             sidecar (Sidecar or file-like):  A JSON sidecar needed for HED operations.
 
         """
 
-        return df
+        return df.copy()
 
     @staticmethod
     def _check_list_type(param_value, param_type):
         """ Check a parameter value against its specified type.
 
         Parameters:
             param_value (any):   The value to be checked.
             param_type (any):    Class to check the param_value against.
 
-        Raises:
-            TypeError: If param_value is not an instance of param_type.
+        :raises TypeError:
+            - If param_value is not an instance of param_type.
 
         """
 
         for this_type in param_type:
             if isinstance(param_value, this_type):
                 return
         raise TypeError("BadType", f"{param_value} has type {type(param_value)} which is not in {str(param_type)}")
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/factor_column_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/factor_column_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,23 @@
 
     def __init__(self, parameters):
         """ Constructor for the factor column operation.
 
         Parameters:
             parameters (dict): Parameter values for required and optional parameters.
 
-        Raises:  
-            KeyError    
-                - If a required parameter is missing.    
-                - If an unexpected parameter is provided.    
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
-            ValueError   
-                - If factor_names is not empty and is not the same length as factor_values.   
+        :raises ValueError:
+            - If factor_names is not empty and is not the same length as factor_values.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.column_name = parameters['column_name']
         self.factor_values = parameters['factor_values']
         self.factor_names = parameters['factor_names']
         if self.factor_names and len(self.factor_values) != len(self.factor_names):
@@ -57,15 +56,15 @@
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Create factor columns based on values in a specified column.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like):  Only needed for HED operations.
+            sidecar (Sidecar or file-like): Not needed for this operation.
 
         Returns:
             DataFrame: A new DataFrame with the factor columns appended.
 
         """
 
         factor_values = self.factor_values
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/factor_hed_tags_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_tags_op.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ Create tabular file factors from tag queries. """
 
 
 import pandas as pd
 import numpy as np
 from hed.tools.remodeling.operations.base_op import BaseOp
 from hed.models.tabular_input import TabularInput
-from hed.models.expression_parser import QueryParser
-from hed.tools.analysis.analysis_util import get_assembled_strings
+from hed.models.sidecar import Sidecar
+from hed.models.df_util import get_assembled
+from hed.tools.analysis.analysis_util import get_expression_parsers, search_strings
 
 
 class FactorHedTagsOp(BaseOp):
     """ Create tabular file factors from tag queries.
 
     Required remodeling parameters:   
         - **queries** (*list*): Queries to be applied successively as filters.    
@@ -25,94 +26,74 @@
     """
 
     PARAMS = {
         "operation": "factor_hed_tags",
         "required_parameters": {
             "queries": list,
             "query_names": list,
-            "remove_types": list,
-            "expand_context": bool
+            "remove_types": list
         },
-        "optional_parameters": {}
+        "optional_parameters": {
+            "expand_context": bool
+        }
     }
 
     def __init__(self, parameters):
         """ Constructor for the factor HED tags operation.
 
         Parameters:
-            op_spec (dict): Specification for required and optional parameters.
             parameters (dict):  Actual values of the parameters for the operation.
 
-        Raises:
-
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
-
-            TypeError   
-                - If a parameter has the wrong type.   
-
-            ValueError  
-                - If the specification is missing a valid operation.   
-                - If the length of query names is not empty and not same length as queries.   
-                - If there are duplicate query names.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
+
+        :raises TypeError:
+            - If a parameter has the wrong type.
+
+        :raises ValueError:
+            - If the specification is missing a valid operation.
+            - If the length of query names is not empty and not same length as queries.
+            - If there are duplicate query names.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.queries = parameters['queries']
         self.query_names = parameters['query_names']
         self.remove_types = parameters['remove_types']
-        if not self.query_names:
-            self.query_names = [f"query_{index}" for index in range(len(self.queries))]
-        elif len(self.queries) != len(self.query_names):
-            raise ValueError("QueryNamesLengthBad",
-                             f"The query_names length {len(self.query_names)} must be empty or equal" +
-                             f"to the queries length {len(self.queries)} .")
-        elif len(set(self.query_names)) != len(self.query_names):
-            raise ValueError("DuplicateQueryNames",  f"The query names {str(self.query_names)} list has duplicates")
-        self.expression_parsers = []
-        for index, query in enumerate(self.queries):
-            try:
-                next_query = QueryParser(query)
-            except Exception:
-                raise ValueError("BadQuery", f"Query [{index}]: {query} cannot be parsed")
-            self.expression_parsers.append(next_query)
+        self.expression_parsers, self.query_names = get_expression_parsers(self.queries,
+                                                                           query_names=parameters['query_names'])
 
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Factor the column using HED tag queries.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
             sidecar (Sidecar or file-like):  Only needed for HED operations.
 
         Returns:
             Dataframe: A new dataframe after processing.
-        
-        Raises:
 
-            ValueError   
-                - If a name for a new query factor column is already a column.   
+        :raises ValueError:
+            - If a name for a new query factor column is already a column.
 
         """
 
-        input_data = TabularInput(df, hed_schema=dispatcher.hed_schema, sidecar=sidecar)
+        if sidecar and not isinstance(sidecar, Sidecar):
+            sidecar = Sidecar(sidecar)
+        input_data = TabularInput(df.copy(), sidecar=sidecar, name=name)
         column_names = list(df.columns)
-        for name in self.query_names:
-            if name in column_names:
+        for query_name in self.query_names:
+            if query_name in column_names:
                 raise ValueError("QueryNameAlreadyColumn",
-                                 f"Query [{name}]: is already a column name of the data frame")
-        df = input_data.dataframe.copy()
-        df_list = [df]
-        hed_strings = get_assembled_strings(input_data, hed_schema=dispatcher.hed_schema, expand_defs=True)
-        df_factors = pd.DataFrame(0, index=range(len(hed_strings)), columns=self.query_names)
-        for parse_ind, parser in enumerate(self.expression_parsers):
-            for index, next_item in enumerate(hed_strings):
-                match = parser.search(next_item)
-                if match:
-                    df_factors.at[index, self.query_names[parse_ind]] = 1
+                                 f"Query [{query_name}]: is already a column name of the data frame")
+        df_list = [input_data.dataframe]
+        hed_strings, _ = get_assembled(input_data, sidecar, dispatcher.hed_schema, extra_def_dicts=None,
+                                       join_columns=True, shrink_defs=False, expand_defs=True)
+        df_factors = search_strings(hed_strings, self.expression_parsers, query_names=self.query_names)
         if len(df_factors.columns) > 0:
             df_list.append(df_factors)
         df_new = pd.concat(df_list, axis=1)
         df_new.replace('n/a', np.NaN, inplace=True)
         return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/factor_hed_type_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/factor_hed_type_op.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """ Create tabular file factors from type variables. """
 
 import pandas as pd
 import numpy as np
 from hed.tools.remodeling.operations.base_op import BaseOp
 from hed.models.tabular_input import TabularInput
-from hed.tools.analysis.analysis_util import get_assembled_strings
+from hed.models.sidecar import Sidecar
+from hed.models.df_util import get_assembled
 from hed.tools.analysis.hed_type_manager import HedTypeManager
 
 # TODO: restricted factor values are not implemented yet.
 
 
 class FactorHedTypeOp(BaseOp):
     """ Create tabular file factors from type variables and append to tabular data.
@@ -28,27 +29,25 @@
         "optional_parameters": {}
     }
 
     def __init__(self, parameters):
         """ Constructor for the factor HED type operation.
 
         Parameters:
-            op_spec (dict): Specification for required and optional parameters.
             parameters (dict):  Actual values of the parameters for the operation.
 
-        Raises:
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
-            ValueError   
-                - If the specification is missing a valid operation.   
+        :raises ValueError:
+            - If the specification is missing a valid operation.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.type_tag = parameters["type_tag"]
         self.type_values = parameters["type_values"]
 
     def do_op(self, dispatcher, df, name, sidecar=None):
@@ -64,20 +63,22 @@
             DataFrame: A new DataFame with that includes the factors.
 
         Notes:
             - If column_name is not a column in df, df is just returned.
 
         """
 
-        input_data = TabularInput(df, hed_schema=dispatcher.hed_schema, sidecar=sidecar)
-        df = input_data.dataframe.copy()
-        df_list = [df]
-        hed_strings = get_assembled_strings(input_data, hed_schema=dispatcher.hed_schema, expand_defs=False)
+        if sidecar and not isinstance(sidecar, Sidecar):
+            sidecar = Sidecar(sidecar)
+        input_data = TabularInput(df, sidecar=sidecar, name=name)
+        df_list = [input_data.dataframe.copy()]
+        hed_strings, definitions = get_assembled(input_data, sidecar, dispatcher.hed_schema, 
+                                                 extra_def_dicts=None, join_columns=True,
+                                                 shrink_defs=True, expand_defs=False)
 
-        definitions = input_data.get_definitions()
         var_manager = HedTypeManager(hed_strings, dispatcher.hed_schema, definitions)
         var_manager.add_type_variable(self.type_tag.lower())
 
         df_factors = var_manager.get_factor_vectors(self.type_tag, [], factor_encoding="one-hot")
         if len(df_factors.columns) > 0:
             df_list.append(df_factors)
         df_new = pd.concat(df_list, axis=1)
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/merge_consecutive_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/merge_consecutive_op.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from hed.tools.remodeling.operations.base_op import BaseOp
 
 
 class MergeConsecutiveOp(BaseOp):
     """ Merge consecutive rows with same column value.
 
     Required remodeling parameters:
-        - **column_name** (*str*): the name of the column whose consecutive values are to be compared (the merge column).  
+        - **column_name** (*str*): name of column whose consecutive values are to be compared (the merge column).  
         - **event_code** (*str* or *int* or *float*): the particular value in the match column to be merged.  
         - **match_columns** (*list*):  A list of columns whose values have to be matched for two events to be the same.  
         - **set_durations** (*bool*): If true, set the duration of the merged event to the extent of the merged events.  
         - **ignore_missing** (*bool*):  If true, missing match_columns are ignored.  
 
     """
     PARAMS = {
@@ -27,29 +27,26 @@
         "optional_parameters": {}
     }
 
     def __init__(self, parameters):
         """ Constructor for the merge consecutive operation.
 
         Parameters:
-            op_spec (dict): Specification for required and optional parameters.
             parameters (dict): Actual values of the parameters for the operation.
 
-        Raises:
-
-            KeyError   
-            - If a required parameter is missing.   
-            - If an unexpected parameter is provided.   
- 
-            TypeError   
-            - If a parameter has the wrong type.   
-
-            ValueError   
-            - If the specification is missing a valid operation.   
-            - If one of the match column is the merge column.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
+
+        :raises TypeError:
+            - If a parameter has the wrong type.
+
+        :raises ValueError:
+            - If the specification is missing a valid operation.
+            - If one of the match column is the merge column.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.column_name = parameters["column_name"]
         self.event_code = parameters["event_code"]
         self.match_columns = parameters["match_columns"]
         if self.column_name in self.match_columns:
@@ -61,26 +58,24 @@
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Merge consecutive rows with the same column value.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like): Only needed for HED operations.
+            sidecar (Sidecar or file-like): Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
-        Raises:
-
-            ValueError   
-                - If dataframe does not have the anchor column and ignore_missing is False.   
-                - If a match column is missing and ignore_missing is false.   
-                - If the durations were to be set and the dataframe did not have an onset column.   
-                - If the durations were to be set and the dataframe did not have a duration column.   
+        :raises ValueError:
+            - If dataframe does not have the anchor column and ignore_missing is False.
+            - If a match column is missing and ignore_missing is false.
+            - If the durations were to be set and the dataframe did not have an onset column.
+            - If the durations were to be set and the dataframe did not have a duration column.
 
         """
 
         if not self.ignore_missing and self.column_name not in df.columns:
             raise ValueError("ColumnMissing",
                              f"{name}: {self.column_name} is not in data columns [{str(df.columns)}] "
                              f"and missing columns are not ignored")
@@ -117,15 +112,15 @@
         Parameters:
             match_df (DataFrame): DataFrame containing columns to be matched.
             code_mask (DataSeries):  Same length as match_df with the names.
 
         Returns:
             list:  Group numbers set (starting at 1).
 
-        # TODO: Handle roundoff in rows for comparison.
+        # TODO: Handle round off in rows for comparison.
         """
         in_group = False
         remove_groups = [0] * len(match_df)
         group_count = 0
         for index, row in match_df.iterrows():
             if not code_mask.iloc[index]:
                 in_group = False
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/number_groups_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/number_groups_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """ Implementation in progress. """
-import numpy as np
+
 from hed.tools.remodeling.operations.base_op import BaseOp
-from hed.tools.util.data_util import get_indices, tuple_to_range
-import itertools
 
-#TODO: This class is under development
+
+# TODO: This class is under development
 
 
 class NumberGroupsOp(BaseOp):
     """ Implementation in progress. """
 
     PARAMS = {
         "operation": "number_groups",
@@ -31,15 +30,16 @@
         self.inclusion_test = ["include", "exclude"]
 
         required = set(self.start_stop_test.keys())
         for param_to_test in [self.start, self.stop]:
             required_missing = required.difference(set(param_to_test.keys()))
             if required_missing:
                 raise KeyError("MissingRequiredParameters",
-                               f"Specified {param_to_test} for number_rows requires parameters {list(required_missing)}")
+                               f"Specified {param_to_test} for number_rows requires parameters"
+                               f"{list(required_missing)}")
             for param_name, param_value in param_to_test.items():
                 param_type = str
                 if param_name in required:
                     param_type = self.start_stop_test[param_name]
                 else:
                     raise KeyError("BadParameter",
                                    f"{param_name} not a required or optional parameter for {self.operation}")
@@ -89,18 +89,18 @@
             if element not in df[self.source_column].tolist():
                 missing.append(element)
         if len(missing) > 0:
             raise ValueError("MissingValue",
                              f"Start value(s) {missing} does not exist in {self.source_column} of event file {name}")
 
         df_new = df.copy()
-        # create number column
-        df_new[self.number_column_name] = np.nan
-
-        # find group indices
-        indices = tuple_to_range(
-            get_indices(df, self.source_column, self.start['values'], self.stop['values']),
-            [self.start['inclusion'], self.stop['inclusion']])
-        for i, group in enumerate(indices):
-            df_new.loc[group, self.number_column_name] = i + 1
+        # # create number column
+        # df_new[self.number_column_name] = np.nan
+        #
+        # # find group indices
+        # indices = tuple_to_range(
+        #     get_indices(df, self.source_column, self.start['values'], self.stop['values']),
+        #     [self.start['inclusion'], self.stop['inclusion']])
+        # for i, group in enumerate(indices):
+        #     df_new.loc[group, self.number_column_name] = i + 1
 
         return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/number_rows_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/number_rows_op.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """ Implementation in progress. """
 import numpy as np
 from hed.tools.remodeling.operations.base_op import BaseOp
 
-#TODO: This class is under development
+# TODO: This class is under development
 
 
 class NumberRowsOp(BaseOp):
     """ Implementation in progress. """
     PARAMS = {
         "operation": "number_rows",
         "required_parameters": {
@@ -61,16 +61,16 @@
                                  f"Column {self.match_value['column']} does not exist in event file.", "")
             if self.match_value['value'] not in df[self.match_value['column']].tolist():
                 raise ValueError("MissingMatchValue",
                                  f"Value {self.match_value['value']} does not exist in event file column"
                                  f"{self.match_value['column']}.", "")
 
         df_new = df.copy()
-        df_new[self.number_column_name] = np.nan
-        if self.match_value:
-            filter = df[self.match_value['column']] == self.match_value['value']
-            numbers = [*range(1, sum(filter)+1)]
-            df_new.loc[filter, self.number_column_name] = numbers
-        else:
-            df_new[self.number_column_name] = df_new.index + 1
+        # df_new[self.number_column_name] = np.nan
+        # if self.match_value:
+        #     filter = df[self.match_value['column']] == self.match_value['value']
+        #     numbers = [*range(1, sum(filter)+1)]
+        #     df_new.loc[filter, self.number_column_name] = numbers
+        # else:
+        #     df_new[self.number_column_name] = df_new.index + 1
 
         return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/remap_columns_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/remap_columns_op.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
     Required remodeling parameters:   
         - **source_columns** (*list*): The key columns to map (m key columns).   
         - **destination_columns** (*list*): The destination columns to have the mapped values (n destination columns).   
         - **map_list** (*list*): A list of lists with the mapping.    
         - **ignore_missing** (*bool*): If True, entries whose key column values are not in map_list are ignored.   
 
     Optional remodeling parameters:   
-        **integer_sources** (*list*): Sour columns that should be treated as integers rather than strings.   
+        **integer_sources** (*list*): Source columns that should be treated as integers rather than strings.   
 
     Notes:
         Each list element list is of length m + n with the key columns followed by mapped columns. 
-         
+
     TODO: Allow wildcards
 
     """
 
     PARAMS = {
         "operation": "remap_columns",
         "required_parameters": {
@@ -40,28 +40,27 @@
 
     def __init__(self, parameters):
         """ Constructor for the remap columns operation.
 
             Parameters:
                 parameters (dict): Parameter values for required and optional parameters.
 
-            Raises:
-                KeyError   
-                    - If a required parameter is missing.    
-                    - If an unexpected parameter is provided.    
- 
-                TypeError   
-                    - If a parameter has the wrong type.   
-
-                ValueError   
-                    - If an integer column is not a key column.    
-                    - If a column designated as an integer source does not have valid integers.    
-                    - If no source columns are specified.    
-                    - If no destination columns are specified.    
-                    - If a map_list entry has the wrong number of items (source columns + destination columns).    
+            :raises KeyError:
+                - If a required parameter is missing.
+                - If an unexpected parameter is provided.
+
+            :raises TypeError:
+                - If a parameter has the wrong type.
+
+            :raises ValueError:
+                - If an integer column is not a key column.
+                - If a column designated as an integer source does not have valid integers.
+                - If no source columns are specified.
+                - If no destination columns are specified.
+                - If a map_list entry has the wrong number of items (source columns + destination columns).
 
           """
         super().__init__(self.PARAMS, parameters)
         self.source_columns = parameters['source_columns']
         self.integer_sources = []
         self.string_sources = self.source_columns
         if "integer_sources" in parameters:
@@ -97,27 +96,27 @@
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Remap new columns from combinations of others.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like): Only needed for HED operations.
+            sidecar (Sidecar or file-like): Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
-        Raises:
-            ValueError   
-                - If ignore_missing is false and source values from the data are not in the map.   
+        :raises ValueError:
+            - If ignore_missing is false and source values from the data are not in the map.
 
         """
-        df[self.source_columns] = df[self.source_columns].replace(np.NaN, 'n/a')
+        df1 = df.copy()
+        df1[self.source_columns] = df1[self.source_columns].replace(np.NaN, 'n/a')
         for column in self.integer_sources:
-            int_mask = df[column] != 'n/a'
-            df.loc[int_mask, column] = df.loc[int_mask, column].astype(int)
-        df[self.source_columns] = df[self.source_columns].astype(str)
-        df_new, missing = self.key_map.remap(df)
+            int_mask = df1[column] != 'n/a'
+            df1.loc[int_mask, column] = df1.loc[int_mask, column].astype(int)
+        df1[self.source_columns] = df1[self.source_columns].astype(str)
+        df_new, missing = self.key_map.remap(df1)
         if missing and not self.ignore_missing:
             raise ValueError("MapSourceValueMissing",
                              f"{name}: Ignore missing is false, but source values [{missing}] are in data but not map")
         return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/remove_columns_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/remove_columns_op.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,21 +22,20 @@
 
     def __init__(self, parameters):
         """ Constructor for remove columns operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters
 
-        Raises:
-            KeyError
-                - If a required parameter is missing.    
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.column_names = parameters['column_names']
         ignore_missing = parameters['ignore_missing']
         if ignore_missing:
             self.error_handling = 'ignore'
@@ -46,24 +45,24 @@
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Remove indicated columns from a dataframe.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like):  Only needed for HED operations.
+            sidecar (Sidecar or file-like):  Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
-        Raises:
-            KeyError   
-                - If ignore_missing is False and a column not in the data is to be removed.   
+        :raises KeyError:
+            - If ignore_missing is False and a column not in the data is to be removed.
 
         """
-
+        df_new = df.copy()
         try:
-            return df.drop(self.column_names, axis=1, errors=self.error_handling)
+            return df_new.drop(self.column_names, axis=1, errors=self.error_handling)
         except KeyError:
             raise KeyError("MissingColumnCannotBeRemoved",
                            f"{name}: Ignore missing is False but a column in {str(self.column_names)} is "
-                           f"not in the data columns [{str(df.columns)}]")
+                           f"not in the data columns [{str(df_new.columns)}]")
+        return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/remove_rows_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/remove_rows_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,39 +23,38 @@
 
     def __init__(self, parameters):
         """ Constructor for remove rows operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.column_name = parameters["column_name"]
         self.remove_values = parameters["remove_values"]
 
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Remove rows with the values indicated in the column.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str):  Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like): Only needed for HED operations.
+            sidecar (Sidecar or file-like): Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
         """
-
-        if self.column_name not in df.columns:
-            return df
+        df_new = df.copy()
+        if self.column_name not in df_new.columns:
+            return df_new
         for value in self.remove_values:
-            df = df.loc[df[self.column_name] != value, :]
-        return df
+            df_new = df_new.loc[df_new[self.column_name] != value, :]
+        return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/rename_columns_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/rename_columns_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,21 +23,20 @@
 
     def __init__(self, parameters):
         """ Constructor for rename columns operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters
 
-        Raises:
-            KeyError    
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.column_mapping = parameters['column_mapping']
         if parameters['ignore_missing']:
             self.error_handling = 'ignore'
         else:
@@ -46,24 +45,23 @@
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Rename columns as specified in column_mapping dictionary.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like):  Only needed for HED operations.
+            sidecar (Sidecar or file-like):  Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
-        Raises:
-            KeyError   
-                - When ignore_missing is false and column_mapping has columns not in the data.   
+        :raises KeyError:
+            - When ignore_missing is false and column_mapping has columns not in the data.
 
         """
-
+        df_new = df.copy()
         try:
-            return df.rename(columns=self.column_mapping, errors=self.error_handling)
+            return df_new.rename(columns=self.column_mapping, errors=self.error_handling)
         except KeyError:
             raise KeyError("MappedColumnsMissingFromData",
                            f"{name}: ignore_missing is False, mapping columns [{self.column_mapping}]"
                            f" but df columns are [{str(df.columns)}")
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/reorder_columns_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/reorder_columns_op.py`

 * *Files 16% similar despite different names*

```diff
@@ -24,52 +24,50 @@
 
     def __init__(self, parameters):
         """ Constructor for reorder columns operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError  
-                If a parameter has the wrong type.  
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.column_order = parameters['column_order']
         self.ignore_missing = parameters['ignore_missing']
         self.keep_others = parameters['keep_others']
 
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Reorder columns as specified in event dictionary.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame):  The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like):   Only needed for HED operations.
+            sidecar (Sidecar or file-like):  Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
-        Raises:
-            ValueError   
-                - When ignore_missing is false and column_order has columns not in the data.   
+        :raises ValueError:
+            - When ignore_missing is false and column_order has columns not in the data.
 
         """
-
-        current_columns = list(df.columns)
-        missing_columns = set(self.column_order).difference(set(df.columns))
+        df_new = df.copy()
+        current_columns = list(df_new.columns)
+        missing_columns = set(self.column_order).difference(set(df_new.columns))
         ordered = self.column_order
         if missing_columns and not self.ignore_missing:
             raise ValueError("MissingReorderedColumns",
                              f"{str(missing_columns)} are not in dataframe columns "
-                             f" [{str(df.columns)}] and not ignored.")
+                             f" [{str(df_new.columns)}] and not ignored.")
         elif missing_columns:
             ordered = [elem for elem in self.column_order if elem not in list(missing_columns)]
         if self.keep_others:
             ordered += [elem for elem in current_columns if elem not in ordered]
-        df = df.loc[:, ordered]
-        return df
+        df_new = df_new.loc[:, ordered]
+        return df_new
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/split_rows_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/split_rows_op.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 import numpy as np
 import pandas as pd
 from hed.tools.remodeling.operations.base_op import BaseOp
 
 
 class SplitRowsOp(BaseOp):
-    """ Split rows in a tabular file into multiple rows based on a column.
+    """ Split rows in a tabular file into multiple rows based on parameters.
 
     Required remodeling parameters:   
-        - **anchor_column** (*str*): The column in which new items are generated.   
-        - **new_events** (*dict*):  Mapping of new values based on values in the anchor_column.   
-        - **remove_parent_row** (*bool*):  If true, columns not in column_order are placed at end.   
+        - **anchor_column** (*str*): The column in which the names of new items are stored.   
+        - **new_events** (*dict*):  Mapping of new values based on values in the original row.    
+        - **remove_parent_row** (*bool*):  If true, the original row that was split is removed.   
 
     """
 
     PARAMS = {
         "operation": "split_rows",
         "required_parameters": {
             "anchor_column": str,
@@ -27,43 +27,41 @@
 
     def __init__(self, parameters):
         """ Constructor for the split rows operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.anchor_column = parameters['anchor_column']
         self.new_events = parameters['new_events']
         self.remove_parent_row = parameters['remove_parent_row']
 
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Split a row representing a particular event into multiple rows.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str):  Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like):  Only needed for HED operations.
+            sidecar (Sidecar or file-like):  Not needed for this operation.
 
         Returns:
             Dataframe: A new dataframe after processing.
 
-        Raises:
-            TypeError   
-                -If bad onset or duration.   
+        :raises TypeError:
+            -If bad onset or duration.
 
         """
 
         df_new = df.copy()
 
         if self.anchor_column not in df_new.columns:
             df_new[self.anchor_column] = np.nan
@@ -117,16 +115,16 @@
         Parameters:
             df (DataFrame):  The dataframe to process.
             onset_source (list):  List of onsets of process.
 
         Returns:
             list:  list of same length as df with the onsets.
 
-        Raises:
-            HedFileError: raised if one of the onset specifiers is invalid.
+        :raises HedFileError:
+            - If one of the onset specifiers is invalid.
 
         """
 
         onsets = pd.to_numeric(df['onset'], errors='coerce')
         for onset in onset_source:
             if isinstance(onset, float) or isinstance(onset, int):
                 onsets = onsets + onset
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/summarize_column_values_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,150 +1,191 @@
-""" Summarize the values in the columns of a tabular file. """
+""" Create a JSON sidecar from column values in a collection of tabular files. """
 
+import json
 from hed.tools import TabularSummary
 from hed.tools.remodeling.operations.base_op import BaseOp
-from hed.tools.remodeling.operations.base_context import BaseContext
+from hed.tools.remodeling.operations.base_summary import BaseSummary
 
 
-class SummarizeColumnValuesOp(BaseOp):
-    """ Summarize the values in the columns of a tabular file.
+class SummarizeSidecarFromEventsOp(BaseOp):
+    """ Create a JSON sidecar from column values in a collection of tabular files.
 
     Required remodeling parameters:   
         - **summary_name** (*str*): The name of the summary.   
         - **summary_filename** (*str*): Base filename of the summary.   
-        - **skip_columns** (*list*):  Names of columns to skip in the summary.   
+        - **skip_columns** (*list*): Names of columns to skip in the summary.   
         - **value_columns** (*list*): Names of columns to treat as value columns rather than categorical columns.   
 
-    The purpose is to produce a summary of the values in a tabular file.
+    The purpose is to produce a JSON sidecar template for annotating a dataset with HED tags.
 
     """
 
     PARAMS = {
-        "operation": "summarize_column_values",
+        "operation": "summarize_sidecar_from_events",
         "required_parameters": {
             "summary_name": str,
             "summary_filename": str,
             "skip_columns": list,
-            "value_columns": list
+            "value_columns": list,
         },
         "optional_parameters": {
+            "append_timecode": bool
         }
     }
 
-    SUMMARY_TYPE = 'column_values'
+    SUMMARY_TYPE = "events_to_sidecar"
 
     def __init__(self, parameters):
-        """ Constructor for the summarize column values operation.
+        """ Constructor for summarize sidecar from events operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
-
-            TypeError   
-                - If a parameter has the wrong type.    
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
 
         super().__init__(self.PARAMS, parameters)
         self.summary_name = parameters['summary_name']
         self.summary_filename = parameters['summary_filename']
         self.skip_columns = parameters['skip_columns']
         self.value_columns = parameters['value_columns']
+        self.append_timecode = parameters.get('append_timecode', False)
 
     def do_op(self, dispatcher, df, name, sidecar=None):
-        """ Create factor columns corresponding to values in a specified column.
+        """ Extract a sidecar from events file.
 
         Parameters:
-            dispatcher (Dispatcher): Manages the operation I/O.
-            df (DataFrame): The DataFrame to be remodeled.
-            name (str):  Unique identifier for the dataframe -- often the original file path.
-            sidecar (Sidecar or file-like): Only needed for HED operations.
+            dispatcher (Dispatcher): The dispatcher object for managing the operations.
+            df (DataFrame): The tabular file to be remodeled.
+            name (str): Unique identifier for the dataframe -- often the original file path.
+            sidecar (Sidecar or file-like): Not needed for this operation.
 
         Returns:
-            DataFrame: A new DataFrame with the factor columns appended.
+            DataFrame: A copy of df.
 
         Side-effect:
-            Updates the context.
+            Updates the associated summary if applicable.
 
         """
 
-        summary = dispatcher.context_dict.get(self.summary_name, None)
+        df_new = df.copy()
+        summary = dispatcher.summary_dicts.get(self.summary_name, None)
         if not summary:
-            summary = ColumnValueSummaryContext(self)
-            dispatcher.context_dict[self.summary_name] = summary
-        summary.update_context({'df': dispatcher.post_proc_data(df), 'name': name})
-        return df
+            summary = EventsToSidecarSummary(self)
+            dispatcher.summary_dicts[self.summary_name] = summary
+        summary.update_summary({'df': dispatcher.post_proc_data(df_new), 'name': name})
+        return df_new
 
 
-class ColumnValueSummaryContext(BaseContext):
+class EventsToSidecarSummary(BaseSummary):
 
     def __init__(self, sum_op):
-        super().__init__(sum_op.SUMMARY_TYPE, sum_op.summary_name, sum_op.summary_filename)
-        self.value_columns = sum_op.value_columns
-        self.skip_columns = sum_op.skip_columns
-
-    def update_context(self, new_context):
-        name = new_context['name']
-        if name not in self.summary_dict:
-            self.summary_dict[name] = \
-                TabularSummary(value_cols=self.value_columns, skip_cols=self.skip_columns, name=name)
-        self.summary_dict[name].update(new_context['df'])
-
-    def _get_summary_details(self, summary):
-        return summary.get_summary(as_json=False)
-
-    def _merge_all(self):
-        all_sum = TabularSummary(value_cols=self.value_columns, skip_cols=self.skip_columns, name='Dataset')
-        for key, counts in self.summary_dict.items():
-            all_sum.update_summary(counts)
+        super().__init__(sum_op)
+        self.value_cols = sum_op.value_columns
+        self.skip_cols = sum_op.skip_columns
+
+    def update_summary(self, new_info):
+        """ Update the summary for a given tabular input file.
+
+        Parameters:
+            new_info (dict):  A dictionary with the parameters needed to update a summary.
+
+        Notes:
+            - The summary needs a "name" str and a "df".
+
+        """
+
+        tab_sum = TabularSummary(value_cols=self.value_cols, skip_cols=self.skip_cols, name=new_info["name"])
+        tab_sum.update(new_info['df'], new_info['name'])
+        self.summary_dict[new_info["name"]] = tab_sum
+
+    def get_details_dict(self, summary_info):
+        """ Return the summary-specific information.
+
+        Parameters:
+            summary_info (TabularSummary):  Summary to return info from
+
+        Notes:
+            Abstract method be implemented by each individual context summary.
+
+        """
+
+        return {"files": summary_info.files, "total_files": summary_info.total_files,
+                "total_events": summary_info.total_events, "skip_cols": summary_info.skip_cols,
+                "sidecar": summary_info.extract_sidecar_template()}
+
+    def merge_all_info(self):
+        """ Merge summary information from all of the files
+
+        Returns:
+           TabularSummary:  Consolidated summary of information.
+
+        """
+
+        all_sum = TabularSummary(name='Dataset')
+        for key, tab_sum in self.summary_dict.items():
+            all_sum.update_summary(tab_sum)
         return all_sum
 
-    def _get_result_string(self, name, result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return a formatted string with the summary for the indicated name.
+
+        Parameters:
+            name (str):  Identifier (usually the filename) of the individual file.
+            result (dict): The dictionary of the summary results indexed by name.
+            indent (str): A string containing spaces used for indentation (usually 3 spaces).
+
+        Returns:
+            str - The results in a printable format ready to be saved to a text file.
+
+        Notes:
+            This calls _get_dataset_string to get the overall summary string and
+            _get_individual_string to get an individual summary string.
+
+        """
+
         if name == "Dataset":
             return self._get_dataset_string(result, indent=indent)
-        return self._get_individual_string(name, result, indent=indent)
+        return self._get_individual_string(result, indent=indent)
 
     @staticmethod
-    def _get_dataset_string(result, indent=BaseContext.DISPLAY_INDENT):
-        sum_list = [f"Dataset: Total events={result.get('Total events', 0)} "
-                    f"Total files={result.get('Total files', 0)}"]
-        cat_cols = result.get("Categorical columns", {})
-        if cat_cols:
-            sum_list.append(ColumnValueSummaryContext._get_categorical_string(cat_cols, offset="", indent=indent))
-        val_cols = result.get("Value columns", {})
-        if val_cols:
-            sum_list.append(ColumnValueSummaryContext._get_value_string(val_cols, offset="", indent=indent))
-        return "\n".join(sum_list)
+    def _get_dataset_string(result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return  a string with the overall summary for all of the tabular files.
 
-    @staticmethod
-    def _get_individual_string(name, result, indent=BaseContext.DISPLAY_INDENT):
-        sum_list = [f"Total events={result.get('Total events', 0)}"]
-        cat_cols = result.get("Categorical columns", {})
-        if cat_cols:
-            sum_list.append(ColumnValueSummaryContext._get_categorical_string(cat_cols, offset=indent, indent=indent))
-        val_cols = result.get("Value columns", {})
-        if val_cols:
-            sum_list.append(ColumnValueSummaryContext._get_value_string(val_cols, offset=indent, indent=indent))
-        return "\n".join(sum_list)
+        Parameters:
+            result (dict): Dictionary of merged summary information.
+            indent (str):  String of blanks used as the amount to indent for readability.
 
-    @staticmethod
-    def _get_categorical_string(cat_dict, offset="", indent="   "):
-        sum_list = [f"{offset}{indent}Categorical column values[Events, Files]:"]
-        for col_name, col_dict in cat_dict.items():
-            sum_list.append(f"{offset}{indent*2}{col_name}:")
-            col_list = []
-            for col_value, val_counts in col_dict.items():
-                col_list.append(f"{col_value}{str(val_counts)}")
-            sum_list.append(f"{offset}{indent*3}{' '.join(col_list)}")
+        Returns:
+            str: Formatted string suitable for saving in a file or printing.
+
+        """
+        sum_list = [f"Dataset: Total events={result.get('total_events', 0)} "
+                    f"Total files={result.get('total_files', 0)}",
+                    f"Skip columns: {str(result.get('skip_cols', []))}",
+                    f"Value columns: {str(result.get('value_cols', []))}",
+                    f"Sidecar:\n{json.dumps(result['sidecar'], indent=indent)}"]
         return "\n".join(sum_list)
 
     @staticmethod
-    def _get_value_string(val_dict, offset="", indent=""):
-        sum_list = [f"{offset}{indent}Value columns[Events, Files]:"]
-        for col_name, val_counts in val_dict.items():
-            sum_list.append(f"{offset}{indent*2}{col_name}{str(val_counts)}")
+    def _get_individual_string(result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return  a string with the summary for an individual tabular file.
+
+        Parameters:
+            result (dict): Dictionary of summary information for a particular tabular file.
+            indent (str):  String of blanks used as the amount to indent for readability.
+
+        Returns:
+            str: Formatted string suitable for saving in a file or printing.
+
+        """
+        sum_list = [f"Total events={result.get('total_events', 0)}",
+                    f"Skip columns: {str(result.get('skip_cols', []))}",
+                    f"Value columns: {str(result.get('value_cols', []))}",
+                    f"Sidecar:\n{json.dumps(result['sidecar'], indent=indent)}"]
         return "\n".join(sum_list)
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/summarize_hed_tags_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_tags_op.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,169 +1,234 @@
 """ Summarize the HED tags in collection of tabular files.  """
 
 from hed.models.tabular_input import TabularInput
+from hed.models.sidecar import Sidecar
 from hed.tools.analysis.hed_tag_counts import HedTagCounts
 from hed.tools.remodeling.operations.base_op import BaseOp
-from hed.tools.remodeling.operations.base_context import BaseContext
+from hed.tools.remodeling.operations.base_summary import BaseSummary
+from hed.models.df_util import get_assembled
 
 
 class SummarizeHedTagsOp(BaseOp):
     """ Summarize the HED tags in collection of tabular files.
 
 
     Required remodeling parameters:   
         - **summary_name** (*str*): The name of the summary.   
         - **summary_filename** (*str*): Base filename of the summary.   
-        - **type_tags** (*list*): Type tag to get_summary separately (e.g. 'condition-variable' or 'task').   
-        - **include_context** (*bool*): If True, expand Onset and Offset tags.   
+        - **tags** (*dict*): Type tag to get_summary separately (e.g. 'condition-variable' or 'task').   
 
     Optional remodeling parameters:    
-        - **breakout_list** (*list*):  A list of tags to be separated.  
-
+       - **expand_context** (*bool*): If True, include counts from expanded context (not supported).   
 
     The purpose of this op is to produce a summary of the occurrences of specified tag. This summary
     is often used with 'condition-variable' to produce a summary of the experimental design.
 
 
     """
 
     PARAMS = {
         "operation": "summarize_hed_tags",
         "required_parameters": {
             "summary_name": str,
             "summary_filename": str,
-            "tags": dict,
-            "expand_context": bool
+            "tags": dict
         },
         "optional_parameters": {
+            "append_timecode": bool,
+            "expand_context": bool
         }
     }
 
     SUMMARY_TYPE = "hed_tag_summary"
 
     def __init__(self, parameters):
         """ Constructor for the summarize hed tags operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:   
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.summary_name = parameters['summary_name']
         self.summary_filename = parameters['summary_filename']
         self.tags = parameters['tags']
-        self.expand_context = parameters['expand_context']
+        self.append_timecode = parameters.get('append_timecode', False)
+        self.expand_context = parameters.get('expand_context', False)
 
     def do_op(self, dispatcher, df, name, sidecar=None):
-        """ Create factor columns corresponding to values in a specified column.
+        """ Summarize the HED tags present in the dataset.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be remodeled.
             name (str): Unique identifier for the dataframe -- often the original file path.
             sidecar (Sidecar or file-like):  Only needed for HED operations.
 
         Returns:
-            DataFrame: A new DataFrame with the factor columns appended.
+            DataFrame: A copy of df.
 
         Side-effect:
             Updates the context.
 
         """
-        summary = dispatcher.context_dict.get(self.summary_name, None)
+        df_new = df.copy()
+        summary = dispatcher.summary_dicts.get(self.summary_name, None)
         if not summary:
-            summary = HedTagSummaryContext(self)
-            dispatcher.context_dict[self.summary_name] = summary
-        summary.update_context({'df': dispatcher.post_proc_data(df), 'name': name,
+            summary = HedTagSummary(self)
+            dispatcher.summary_dicts[self.summary_name] = summary
+        summary.update_summary({'df': dispatcher.post_proc_data(df_new), 'name': name,
                                 'schema': dispatcher.hed_schema, 'sidecar': sidecar})
-        return df
+        return df_new
 
 
-class HedTagSummaryContext(BaseContext):
+class HedTagSummary(BaseSummary):
 
     def __init__(self, sum_op):
-        super().__init__(sum_op.SUMMARY_TYPE, sum_op.summary_name, sum_op.summary_filename)
+        super().__init__(sum_op)
         self.tags = sum_op.tags
         self.expand_context = sum_op.expand_context
 
-    def update_context(self, new_context):
-        counts = HedTagCounts(new_context['name'], total_events=len(new_context['df']))
-        input_data = TabularInput(new_context['df'], hed_schema=new_context['schema'], sidecar=new_context['sidecar'])
-        definitions = input_data.get_definitions().gathered_defs
-        for objs in input_data.iter_dataframe(hed_ops=[new_context['schema']], return_string_only=False,
-                                              expand_defs=False, remove_definitions=True):
-            counts.update_event_counts(objs['HED'], new_context['name'])
-        self.summary_dict[new_context["name"]] = counts
+    def update_summary(self, new_info):
+        """ Update the summary for a given tabular input file.
+
+        Parameters:
+            new_info (dict):  A dictionary with the parameters needed to update a summary.
+
+        Notes:
+            - The summary needs a "name" str, a "schema", a "df, and a "Sidecar".
+
+        """
+        counts = HedTagCounts(new_info['name'], total_events=len(new_info['df']))
+        sidecar = new_info['sidecar']
+        if sidecar and not isinstance(sidecar, Sidecar):
+            sidecar = Sidecar(sidecar)
+        input_data = TabularInput(new_info['df'], sidecar=sidecar, name=new_info['name'])
+        hed_strings, definitions = get_assembled(input_data, sidecar, new_info['schema'],
+                                                 extra_def_dicts=None, join_columns=True,
+                                                 shrink_defs=False, expand_defs=True)
+        # definitions = input_data.get_definitions().gathered_defs
+        for hed in hed_strings:
+            counts.update_event_counts(hed, new_info['name'])
+        self.summary_dict[new_info["name"]] = counts
+
+    def get_details_dict(self, merge_counts):
+        """ Return the summary-specific information in a dictionary.
+
+        Parameters:
+            merge_counts (HedTagCounts):  Contains the counts of tags in the dataset.
+
+        Returns:
+            dict: dictionary with the summary results.
 
-    def _get_summary_details(self, merge_counts):
+        """
         template, unmatched = merge_counts.organize_tags(self.tags)
         details = {}
         for key, key_list in self.tags.items():
             details[key] = self._get_details(key_list, template, verbose=True)
         leftovers = [value.get_info(verbose=True) for value in unmatched]
         return {"name": merge_counts.name, "total_events": merge_counts.total_events,
                 "files": [name for name in merge_counts.files.keys()],
                 "Main tags": details, "Other tags": leftovers}
 
-    def _get_result_string(self, name, result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return a formatted string with the summary for the indicated name.
+
+        Parameters:
+            name (str):  Identifier (usually the filename) of the individual file.
+            result (dict): The dictionary of the summary results indexed by name.
+            indent (str): A string containing spaces used for indentation (usually 3 spaces).
+
+        Returns:
+            str - The results in a printable format ready to be saved to a text file.
+
+        Notes:
+            This calls _get_dataset_string to get the overall summary string and
+            _get_individual_string to get an individual summary string.
+
+        """
         if name == 'Dataset':
             return self._get_dataset_string(result, indent=indent)
-        return self._get_individual_string(name, result, indent=indent)
+        return self._get_individual_string(result, indent=indent)
+
+    def merge_all_info(self):
+        """ Create a HedTagCounts containing the overall dataset HED tag  summary.
+
+        Returns:
+            HedTagCounts - the overall dataset summary object for HED tag counts.
+
+        """
 
-    def _merge_all(self):
         all_counts = HedTagCounts('Dataset')
         for key, counts in self.summary_dict.items():
             all_counts.merge_tag_dicts(counts.tag_dict)
             for file_name in counts.files.keys():
                 all_counts.files[file_name] = ""
             all_counts.total_events = all_counts.total_events + counts.total_events
         return all_counts
-    
+
     @staticmethod
-    def _get_dataset_string(result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_dataset_string(result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return  a string with the overall summary for all of the tabular files.
+
+        Parameters:
+            result (dict): Dictionary of merged summary information.
+            indent (str):  String of blanks used as the amount to indent for readability.
+
+        Returns:
+            str: Formatted string suitable for saving in a file or printing.
+
+        """
         sum_list = [f"Dataset: Total events={result.get('total_events', 0)} "
                     f"Total files={len(result.get('files', []))}"]
-        sum_list = sum_list + HedTagSummaryContext._get_tag_list(result, indent=indent)
+        sum_list = sum_list + HedTagSummary._get_tag_list(result, indent=indent)
         return "\n".join(sum_list)
-    
+
     @staticmethod
-    def _get_individual_string(name, result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_individual_string(result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return  a string with the summary for an individual tabular file.
+
+        Parameters:
+            result (dict): Dictionary of summary information for a particular tabular file.
+            indent (str):  String of blanks used as the amount to indent for readability.
+
+        Returns:
+            str: Formatted string suitable for saving in a file or printing.
+
+        """
         sum_list = [f"Total events={result.get('total_events', 0)}"]
-        sum_list = sum_list + HedTagSummaryContext._get_tag_list(result, indent=indent)
+        sum_list = sum_list + HedTagSummary._get_tag_list(result, indent=indent)
         return "\n".join(sum_list)
-    
+
     @staticmethod
     def _tag_details(tags):
         tag_list = []
         for tag in tags:
             tag_list.append(f"{tag['tag']}[{tag['events']},{len(tag['files'])}]")
         return tag_list
-    
+
     @staticmethod
-    def _get_tag_list(tag_info, indent=BaseContext.DISPLAY_INDENT):
+    def _get_tag_list(tag_info, indent=BaseSummary.DISPLAY_INDENT):
         sum_list = [f"\n{indent}Main tags[events,files]:"]
         for category, tags in tag_info['Main tags'].items():
             sum_list.append(f"{indent}{indent}{category}:")
             if tags:
-                sum_list.append(f"{indent}{indent}{indent}{' '.join(HedTagSummaryContext._tag_details(tags))}")
+                sum_list.append(f"{indent}{indent}{indent}{' '.join(HedTagSummary._tag_details(tags))}")
         if tag_info['Other tags']:
             sum_list.append(f"{indent}Other tags[events,files]:")
-            sum_list.append(f"{indent}{indent}{' '.join(HedTagSummaryContext._tag_details(tag_info['Other tags']))}")
+            sum_list.append(f"{indent}{indent}{' '.join(HedTagSummary._tag_details(tag_info['Other tags']))}")
         return sum_list
 
     @staticmethod
     def _get_details(key_list, template, verbose=False):
         key_details = []
         for item in key_list:
             for tag_cnt in template[item.lower()]:
                 key_details.append(tag_cnt.get_info(verbose=verbose))
         return key_details
-
-
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/summarize_hed_type_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_type_op.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """ Summarize a HED type tag in a collection of tabular files. """
 
 from hed.models.tabular_input import TabularInput
-from hed.tools.analysis.analysis_util import get_assembled_strings
+from hed.models.sidecar import Sidecar
+from hed.models.df_util import get_assembled
 from hed.tools.analysis.hed_type_values import HedTypeValues
 from hed.tools.analysis.hed_type_counts import HedTypeCounts
 from hed.tools.analysis.hed_context_manager import HedContextManager
 from hed.tools.remodeling.operations.base_op import BaseOp
-from hed.tools.remodeling.operations.base_context import BaseContext
+from hed.tools.remodeling.operations.base_summary import BaseSummary
 
 
 class SummarizeHedTypeOp(BaseOp):
     """ Summarize a HED type tag in a collection of tabular files.
 
     Required remodeling parameters:   
         - **summary_name** (*str*): The name of the summary.   
@@ -26,142 +27,199 @@
         "operation": "summarize_hed_type",
         "required_parameters": {
             "summary_name": str,
             "summary_filename": str,
             "type_tag": str
         },
         "optional_parameters": {
+            "append_timecode": bool
         }
     }
 
     SUMMARY_TYPE = 'hed_type_summary'
 
     def __init__(self, parameters):
         """ Constructor for the summarize hed type operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
 
-            TypeError   
-                - If a parameter has the wrong type.   
+        :raises TypeError:
+            - If a parameter has the wrong type.
 
         """
         super().__init__(self.PARAMS, parameters)
         self.summary_name = parameters['summary_name']
         self.summary_filename = parameters['summary_filename']
         self.type_tag = parameters['type_tag'].lower()
+        self.append_timecode = parameters.get('append_timecode', False)
 
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Summarize a specified HED type variable such as Condition-variable .
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be summarized.
             name (str): Unique identifier for the dataframe -- often the original file path.
             sidecar (Sidecar or file-like): Usually required unless event file has a HED column.
 
         Returns:
-            DataFrame: Input DataFrame, unchanged.
+            DataFrame: A copy of df
 
         Side-effect:
-            Updates the context.
+            Updates the relevant summary.
 
         """
-        summary = dispatcher.context_dict.get(self.summary_name, None)
+        df_new = df.copy()
+        summary = dispatcher.summary_dicts.get(self.summary_name, None)
         if not summary:
-            summary = HedTypeSummaryContext(self)
-            dispatcher.context_dict[self.summary_name] = summary
-        summary.update_context({'df': dispatcher.post_proc_data(df), 'name': name,
+            summary = HedTypeSummary(self)
+            dispatcher.summary_dicts[self.summary_name] = summary
+        summary.update_summary({'df': dispatcher.post_proc_data(df_new), 'name': name,
                                 'schema': dispatcher.hed_schema, 'sidecar': sidecar})
-        return df
+        return df_new
 
 
-class HedTypeSummaryContext(BaseContext):
+class HedTypeSummary(BaseSummary):
 
     def __init__(self, sum_op):
-        super().__init__(sum_op.SUMMARY_TYPE, sum_op.summary_name, sum_op.summary_filename)
+        super().__init__(sum_op)
         self.type_tag = sum_op.type_tag
 
-    def update_context(self, new_context):
-        input_data = TabularInput(new_context['df'], hed_schema=new_context['schema'], sidecar=new_context['sidecar'])
-        hed_strings = get_assembled_strings(input_data, hed_schema=new_context['schema'], expand_defs=False)
-        definitions = input_data.get_definitions().gathered_defs
-        context_manager = HedContextManager(hed_strings, new_context['schema'])
-        type_values = HedTypeValues(context_manager, definitions, new_context['name'], type_tag=self.type_tag)
+    def update_summary(self, new_info):
+        """ Update the summary for a given tabular input file.
 
-        counts = HedTypeCounts(new_context['name'], self.type_tag)
-        counts.update_summary(type_values.get_summary(), type_values.total_events, new_context['name'])
+        Parameters:
+            new_info (dict):  A dictionary with the parameters needed to update a summary.
+
+        Notes:  
+            - The summary needs a "name" str, a "schema", a "df, and a "Sidecar".
+
+        """
+
+        sidecar = new_info['sidecar']
+        if sidecar and not isinstance(sidecar, Sidecar):
+            sidecar = Sidecar(sidecar)
+        input_data = TabularInput(new_info['df'], sidecar=sidecar, name=new_info['name'])
+        hed_strings, definitions = get_assembled(input_data, sidecar, new_info['schema'], 
+                                                 extra_def_dicts=None, join_columns=True, expand_defs=False)
+        context_manager = HedContextManager(hed_strings, new_info['schema'])
+        type_values = HedTypeValues(context_manager, definitions, new_info['name'], type_tag=self.type_tag)
+
+        counts = HedTypeCounts(new_info['name'], self.type_tag)
+        counts.update_summary(type_values.get_summary(), type_values.total_events, new_info['name'])
         counts.add_descriptions(type_values.definitions)
-        self.summary_dict[new_context["name"]] = counts
+        self.summary_dict[new_info["name"]] = counts
 
-    def _get_summary_details(self, counts):
-        return counts.get_summary()
+    def get_details_dict(self, counts):
+        """ Return the summary-specific information in a dictionary.
 
-    def _merge_all(self):
-        """ Return merged information.
+        Parameters:
+            counts (HedTypeCounts):  Contains the counts of the events in which the type occurs.
 
         Returns:
-           object:  Consolidated summary of information.
+            dict: dictionary with the summary results.
 
-        Notes:
-            Abstract method be implemented by each individual context summary.
+        """
+        return counts.get_summary()
+
+    def merge_all_info(self):
+        """ Create a HedTypeCounts containing the overall dataset HED type summary.
+
+        Returns:
+            HedTypeCounts - the overall dataset summary object for HED type summary.
 
         """
         all_counts = HedTypeCounts('Dataset', self.type_tag)
         for key, counts in self.summary_dict.items():
             all_counts.update(counts)
         return all_counts
 
-    def _get_result_string(self, name, result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return a formatted string with the summary for the indicated name.
+
+        Parameters:
+            name (str):  Identifier (usually the filename) of the individual file.
+            result (dict): The dictionary of the summary results indexed by name.
+            indent (str): A string containing spaces used for indentation (usually 3 spaces).
+
+        Returns:
+            str - The results in a printable format ready to be saved to a text file.
+
+        Notes:
+            This calls _get_dataset_string to get the overall summary string and
+            _get_individual_string to get an individual summary string.
+
+        """
         if name == "Dataset":
             return self._get_dataset_string(result, indent=indent)
-        return self._get_individual_string(name, result, indent=indent)
+        return self._get_individual_string(result, indent=indent)
 
     @staticmethod
-    def _get_dataset_string(result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_dataset_string(result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return  a string with the overall summary for all of the tabular files.
+
+        Parameters:
+            result (dict): Dictionary of merged summary information.
+            indent (str):  String of blanks used as the amount to indent for readability.
+
+        Returns:
+            str: Formatted string suitable for saving in a file or printing.
+
+        """
         details = result.get('details', {})
         sum_list = [f"Dataset: Type={result['type_tag']} Type values={len(details)} "
                     f"Total events={result.get('total_events', 0)} Total files={len(result.get('files', []))}"]
 
         for key, item in details.items():
-            str1 = f"{item['events']} event(s) out of {item['total_events']} total events in {len(item['files'])} file(s)"
+            str1 = f"{item['events']} event(s) out of {item['total_events']} total events in " + \
+                   f"{len(item['files'])} file(s)"
             if item['level_counts']:
                 str1 = f"{len(item['level_counts'])} levels in " + str1
             if item['direct_references']:
                 str1 = str1 + f" Direct references:{item['direct_references']}"
             if item['events_with_multiple_refs']:
                 str1 = str1 + f" Multiple references:{item['events_with_multiple_refs']})"
             sum_list.append(f"{indent}{key}: {str1}")
             if item['level_counts']:
-                sum_list = sum_list + HedTypeSummaryContext._level_details(item['level_counts'], indent=indent)
+                sum_list = sum_list + HedTypeSummary._level_details(item['level_counts'], indent=indent)
         return "\n".join(sum_list)
 
     @staticmethod
-    def _get_individual_string(name, result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_individual_string(result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return  a string with the summary for an individual tabular file.
+
+        Parameters:
+            result (dict): Dictionary of summary information for a particular tabular file.
+            indent (str):  String of blanks used as the amount to indent for readability.
+
+        Returns:
+            str: Formatted string suitable for saving in a file or printing.
+
+        """
         details = result.get('details', {})
         sum_list = [f"Type={result['type_tag']} Type values={len(details)} "
                     f"Total events={result.get('total_events', 0)}"]
-        
+
         for key, item in details.items():
             sum_list.append(f"{indent*2}{key}: {item['levels']} levels in {item['events']} events")
             str1 = ""
             if item['direct_references']:
                 str1 = str1 + f" Direct references:{item['direct_references']}"
             if item['events_with_multiple_refs']:
                 str1 = str1 + f" (Multiple references:{item['events_with_multiple_refs']})"
             if str1:
                 sum_list.append(f"{indent*3}{str1}")
             if item['level_counts']:
-                sum_list = sum_list + HedTypeSummaryContext._level_details(item['level_counts'],
-                                                                           offset=indent, indent=indent)
+                sum_list = sum_list + HedTypeSummary._level_details(item['level_counts'],
+                                                                    offset=indent, indent=indent)
         return "\n".join(sum_list)
 
     @staticmethod
     def _level_details(level_counts, offset="", indent=""):
         level_list = []
         for key, details in level_counts.items():
             str1 = f"[{details['events']} events, {details['files']} files]:"
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/summarize_hed_validation_op.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/summarize_hed_validation_op.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """ Validate the HED tags in a dataset and report errors. """
 
 import os
 from hed.errors import ErrorSeverity, ErrorHandler
 from hed.models.sidecar import Sidecar
 from hed.models.tabular_input import TabularInput
 from hed.tools.remodeling.operations.base_op import BaseOp
-from hed.tools.remodeling.operations.base_context import BaseContext
-from hed.validator import HedValidator
+from hed.tools.remodeling.operations.base_summary import BaseSummary
 
 
 class SummarizeHedValidationOp(BaseOp):
     """ Validate the HED tags in a dataset and report errors.
 
     Required remodeling parameters:
         - **summary_name** (*str*): The name of the summary.
@@ -21,75 +20,91 @@
 
     """
 
     PARAMS = {
         "operation": "summarize_hed_validation",
         "required_parameters": {
             "summary_name": str,
-            "summary_filename": str,
-            "check_for_warnings": bool
+            "summary_filename": str
         },
         "optional_parameters": {
+            "append_timecode": bool,
+            "check_for_warnings": bool
         }
     }
 
     SUMMARY_TYPE = 'hed_validation'
 
     def __init__(self, parameters):
         """ Constructor for the summarize hed validation operation.
 
         Parameters:
             parameters (dict): Dictionary with the parameter values for required and optional parameters.
 
-        Raises:  
-            KeyError   
-                - If a required parameter is missing.   
-                - If an unexpected parameter is provided.   
-
-            TypeError   
-                - If a parameter has the wrong type.   
- 
+        :raises KeyError:
+            - If a required parameter is missing.
+            - If an unexpected parameter is provided.
+
+        :raises TypeError:
+            - If a parameter has the wrong type.
+
         """
         super().__init__(self.PARAMS, parameters)
         self.summary_name = parameters['summary_name']
         self.summary_filename = parameters['summary_filename']
-        self.check_for_warnings = parameters['check_for_warnings']
+        self.append_timecode = parameters.get('append_timecode', False)
+        self.check_for_warnings = parameters.get('check_for_warnings', False)
 
     def do_op(self, dispatcher, df, name, sidecar=None):
         """ Validate the dataframe with the accompanying sidecar, if any.
 
         Parameters:
             dispatcher (Dispatcher): Manages the operation I/O.
             df (DataFrame): The DataFrame to be validated.
             name (str): Unique identifier for the dataframe -- often the original file path.
             sidecar (Sidecar or file-like): Usually needed unless only HED tags in HED column of event file.
 
         Returns:
-            DataFrame: Input DataFrame, unchanged.
+            DataFrame: A copy of df
 
         Side-effect:
-            Updates the context.
+            Updates the relevant summary.
 
         """
-        summary = dispatcher.context_dict.get(self.summary_name, None)
+        df_new = df.copy()
+        summary = dispatcher.summary_dicts.get(self.summary_name, None)
         if not summary:
-            summary = HedValidationSummaryContext(self)
-            dispatcher.context_dict[self.summary_name] = summary
-        summary.update_context({'df': dispatcher.post_proc_data(df), 'name': name,
+            summary = HedValidationSummary(self)
+            dispatcher.summary_dicts[self.summary_name] = summary
+        summary.update_summary({'df': dispatcher.post_proc_data(df_new), 'name': name,
                                 'schema': dispatcher.hed_schema, 'sidecar': sidecar})
-        return df
+        return df_new
 
 
-class HedValidationSummaryContext(BaseContext):
+class HedValidationSummary(BaseSummary):
 
     def __init__(self, sum_op):
-        super().__init__(sum_op.SUMMARY_TYPE, sum_op.summary_name, sum_op.summary_filename)
+        super().__init__(sum_op)
         self.check_for_warnings = sum_op.check_for_warnings
 
-    def _get_result_string(self, name, result, indent=BaseContext.DISPLAY_INDENT):
+    def _get_result_string(self, name, result, indent=BaseSummary.DISPLAY_INDENT):
+        """ Return a formatted string with the summary for the indicated name.
+
+        Parameters:
+            name (str):  Identifier (usually the filename) of the individual file.
+            result (dict): The dictionary of the summary results indexed by name.
+            indent (str): A string containing spaces used for indentation (usually 3 spaces).
+
+        Returns:
+            str - The results in a printable format ready to be saved to a text file.
+
+        Notes:
+            This gets the error list from "sidecar_issues" and "event_issues".
+
+        """
 
         if result["is_merged"]:
             sum_list = [f"{name}: [{result['total_sidecar_files']} sidecar files, "
                         f"{result['total_event_files']} event files]"]
             sum_list = sum_list + self.get_error_list(result['sidecar_issues'], count_only=True, indent=indent)
             sum_list = sum_list + self.get_error_list(result['event_issues'], count_only=True, indent=indent)
         else:
@@ -97,53 +112,67 @@
             sum_list = sum_list + self.get_error_list(result['sidecar_issues'], indent=indent*2)
             if result['validation_completed']:
                 sum_list = sum_list + self.get_error_list(result['event_issues'], count_only=False, indent=indent*2)
             else:
                 sum_list = sum_list + [f"{indent*2}Event file validation was incomplete because of sidecar errors"]
         return "\n".join(sum_list)
 
-    def update_context(self, new_context):
-        validator = HedValidator(hed_schema=new_context['schema'])
+    def update_summary(self, new_info):
+        """ Update the summary for a given tabular input file.
+
+        Parameters:
+            new_info (dict):  A dictionary with the parameters needed to update a summary.
+
+        Notes:
+            - The summary needs a "name" str, a schema, a "df", and a "Sidecar".
+        """
+
         results = self.get_empty_results()
         results["total_event_files"] = 1
-        results["event_issues"][new_context["name"]] = []
-        self.summary_dict[new_context["name"]] = results
-        sidecar = new_context.get('sidecar', None)
+        results["event_issues"][new_info["name"]] = []
+        self.summary_dict[new_info["name"]] = results
+        sidecar = new_info.get('sidecar', None)
         filtered_issues = []
         if sidecar:
             if not isinstance(sidecar, Sidecar):
-                sidecar = Sidecar(files=new_context['sidecar'], name=os.path.basename(sidecar))
+                sidecar = Sidecar(files=new_info['sidecar'], name=os.path.basename(sidecar))
             results["sidecar_issues"][sidecar.name] = []
-            sidecar_issues = sidecar.validate_entries(validator, check_for_warnings=self.check_for_warnings)
+            sidecar_issues = sidecar.validate(new_info['schema'])
             filtered_issues = ErrorHandler.filter_issues_by_severity(sidecar_issues, ErrorSeverity.ERROR)
             if not self.check_for_warnings:
                 sidecar_issues = filtered_issues
             results['sidecar_issues'][sidecar.name] = sidecar_issues
             results['total_sidecar_issues'] = len(sidecar_issues)
             results['total_sidecar_files'] = 1
         if not filtered_issues:
             results['validation_completed'] = True
-            input_data = TabularInput(new_context['df'], hed_schema=new_context['schema'],  sidecar=sidecar)
-            issues = input_data.validate_file(validator, check_for_warnings=self.check_for_warnings)
+            input_data = TabularInput(new_info['df'], sidecar=sidecar)
+            issues = input_data.validate(new_info['schema'])
             if not self.check_for_warnings:
                 issues = ErrorHandler.filter_issues_by_severity(issues, ErrorSeverity.ERROR)
-            results['event_issues'][new_context["name"]] = issues
+            results['event_issues'][new_info["name"]] = issues
             results['total_event_issues'] = len(issues)
 
-    def _get_summary_details(self, summary_info):
-        return summary_info
+    def get_details_dict(self, summary_info):
+        """Return the summary details from the summary_info.
 
-    def _merge_all(self):
-        """ Return merged information.
+        Parameters:
+            summary_info (dict): Dictionary of issues
 
         Returns:
-           object:  Consolidated summary of information.
+            dict:  Same summary_info as was passed in.
 
-        Notes:
-            Abstract method be implemented by each individual context summary.
+        """
+        return summary_info
+
+    def merge_all_info(self):
+        """ Create a dictionary containing all of the errors in the dataset.
+
+        Returns:
+            dict - dictionary of issues organized into sidecar_issues and event_issues.
 
         """
 
         results = self.get_empty_results()
         results["is_merged"] = True
         for key, ind_results in self.summary_dict.items():
             results["total_event_files"] += ind_results["total_event_files"]
@@ -163,42 +192,42 @@
     @staticmethod
     def get_empty_results():
         return {"total_event_files": 0, "total_event_issues": 0, "event_issues": {}, "is_merged": False,
                 "total_sidecar_files": 0, "total_sidecar_issues": 0, "sidecar_issues": {},
                 "validation_completed": False}
 
     @staticmethod
-    def get_error_list(error_dict, count_only=False, indent=BaseContext.DISPLAY_INDENT):
+    def get_error_list(error_dict, count_only=False, indent=BaseSummary.DISPLAY_INDENT):
         error_list = []
         for key, item in error_dict.items():
             if count_only and isinstance(item, list):
                 error_list.append(f"{indent}{key}: {len(item)} issues")
             elif count_only:
                 error_list.append(f"{indent}{key}: {item} issues")
             elif not len(item):
                 error_list.append(f"{indent}{key} has no issues")
             else:
                 error_list.append(f"{indent}{key} issues:")
                 for this_item in item:
-                    error_list.append(f"{indent*2}{HedValidationSummaryContext.format_error(this_item)}")
+                    error_list.append(f"{indent*2}{HedValidationSummary.format_error(this_item)}")
         return error_list
 
     @staticmethod
     def format_errors(error_list):
         pass
 
     @staticmethod
     def format_error(error):
         error_str = error['code']
         error_locations = []
-        HedValidationSummaryContext.update_error_location(error_locations, "row", "ec_row", error)
-        HedValidationSummaryContext.update_error_location(error_locations, "column", "ec_column", error)
-        HedValidationSummaryContext.update_error_location(error_locations, "sidecar column",
-                                                          "ec_sidecarColumnName", error)
-        HedValidationSummaryContext.update_error_location(error_locations, "sidecar key", "ec_sidecarKeyName", error)
+        HedValidationSummary.update_error_location(error_locations, "row", "ec_row", error)
+        HedValidationSummary.update_error_location(error_locations, "column", "ec_column", error)
+        HedValidationSummary.update_error_location(error_locations, "sidecar column",
+                                                   "ec_sidecarColumnName", error)
+        HedValidationSummary.update_error_location(error_locations, "sidecar key", "ec_sidecarKeyName", error)
         location_str = ",".join(error_locations)
         if location_str:
             error_str = error_str + f"[{location_str}]"
         error_str = error_str + f": {error['message']}"
         return error_str
 
     @staticmethod
```

### Comparing `hedtools-0.2.0/hed/tools/remodeling/operations/valid_operations.py` & `hedtools-0.3.0/hed/tools/remodeling/operations/valid_operations.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 """ The valid operations for the remodeling tools. """
 
+# from hed.tools.remodeling.operations.convert_columns_op import ConvertColumnsOp
 from hed.tools.remodeling.operations.factor_column_op import FactorColumnOp
 from hed.tools.remodeling.operations.factor_hed_tags_op import FactorHedTagsOp
 from hed.tools.remodeling.operations.factor_hed_type_op import FactorHedTypeOp
 from hed.tools.remodeling.operations.merge_consecutive_op import MergeConsecutiveOp
 from hed.tools.remodeling.operations.number_rows_op import NumberRowsOp
 from hed.tools.remodeling.operations.number_groups_op import NumberGroupsOp
 from hed.tools.remodeling.operations.remove_columns_op import RemoveColumnsOp
 from hed.tools.remodeling.operations.reorder_columns_op import ReorderColumnsOp
 from hed.tools.remodeling.operations.remap_columns_op import RemapColumnsOp
 from hed.tools.remodeling.operations.remove_rows_op import RemoveRowsOp
 from hed.tools.remodeling.operations.rename_columns_op import RenameColumnsOp
 from hed.tools.remodeling.operations.split_rows_op import SplitRowsOp
 from hed.tools.remodeling.operations.summarize_column_names_op import SummarizeColumnNamesOp
 from hed.tools.remodeling.operations.summarize_column_values_op import SummarizeColumnValuesOp
+from hed.tools.remodeling.operations.summarize_definitions_op import SummarizeDefinitionsOp
 from hed.tools.remodeling.operations.summarize_sidecar_from_events_op import SummarizeSidecarFromEventsOp
 from hed.tools.remodeling.operations.summarize_hed_type_op import SummarizeHedTypeOp
 from hed.tools.remodeling.operations.summarize_hed_tags_op import SummarizeHedTagsOp
 from hed.tools.remodeling.operations.summarize_hed_validation_op import SummarizeHedValidationOp
 
 valid_operations = {
+    # 'convert_columns': ConvertColumnsOp,
     'factor_column': FactorColumnOp,
     'factor_hed_tags': FactorHedTagsOp,
     'factor_hed_type': FactorHedTypeOp,
     'merge_consecutive': MergeConsecutiveOp,
     'number_groups_op': NumberGroupsOp,
     'number_rows_op': NumberRowsOp,
     'remap_columns': RemapColumnsOp,
     'remove_columns': RemoveColumnsOp,
     'remove_rows': RemoveRowsOp,
     'rename_columns': RenameColumnsOp,
     'reorder_columns': ReorderColumnsOp,
     'split_rows': SplitRowsOp,
     'summarize_column_names': SummarizeColumnNamesOp,
     'summarize_column_values': SummarizeColumnValuesOp,
+    'summarize_definitions': SummarizeDefinitionsOp,
     'summarize_sidecar_from_events': SummarizeSidecarFromEventsOp,
     'summarize_hed_type': SummarizeHedTypeOp,
     'summarize_hed_tags': SummarizeHedTagsOp,
     'summarize_hed_validation': SummarizeHedValidationOp
 }
```

### Comparing `hedtools-0.2.0/hed/tools/util/data_util.py` & `hedtools-0.3.0/hed/tools/util/data_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,16 +127,16 @@
     Parameters:
         data (DataFrame or str):  DataFrame or filename representing a tsv file.
 
     Returns:
         DataFrame:  A dataframe containing the contents of the tsv file or if data was
              a DataFrame to start with, a new copy of the DataFrame.
 
-    Raises:
-        HedFileError: If a filename is given and it cannot be read into a Dataframe.
+    :raises HedFileError: 
+        - If a filename is given and it cannot be read into a Dataframe.
 
     """
 
     if isinstance(data, str):
         df = pd.read_csv(data, delimiter='\t', header=0, keep_default_na=False, na_values=",null")
     elif isinstance(data, pd.DataFrame):
         df = data.copy()
@@ -151,16 +151,16 @@
     Parameters:
         row (DataSeries)   A Pandas data series corresponding to a row in a spreadsheet.
         key_list (list)    List of column names to create the hash value from.
 
     Returns:
         str: Hash key constructed from the entries of row in the columns specified by key_list.
 
-    Raises:
-        HedFileError: If row doesn't have all of the columns in key_list HedFileError is raised.
+    :raises HedFileError: 
+        - If row doesn't have all of the columns in key_list HedFileError is raised.
 
     """
     columns_present, columns_missing = separate_values(list(row.index.values), key_list)
     if columns_missing:
         raise HedFileError("lookup_row", f"row must have all keys, missing{str(columns_missing)}", "")
     new_row = row[key_list].fillna('n/a').astype(str)
     return get_key_hash(new_row)
@@ -173,16 +173,16 @@
         tsv_path (str):   Path to a tsv file with a header row to be read into a DataFrame.
         key_col (str):    Name of the column which should be the key.
         value_col (str):  Name of the column which should be the value.
 
     Returns:
         dict:  Dictionary with key_col values as the keys and the corresponding value_col values as the values.
 
-    Raises:
-        HedFileError: When tsv_path does not correspond to a file that can be read into a DataFrame.
+    :raises HedFileError: 
+        - When tsv_path does not correspond to a file that can be read into a DataFrame.
 
     """
 
     value_dict = {}
     df = get_new_dataframe(tsv_path)
     for index, row in df.iterrows():
         if row[key_col] in value_dict:
@@ -248,17 +248,18 @@
         data (DataFrame, str):      Dataframe or filename of dataframe whose columns are to be reordered.
         col_order (list):           List of column names in desired order.
         skip_missing (bool):        If true, col_order columns missing from data are skipped, otherwise error.
 
     Returns:
         DataFrame:                  A new reordered dataframe.
 
-    Raises:
-        HedFileError:  If col_order contains columns not in data and skip_missing is False or if
-            data corresponds to a filename from which a dataframe cannot be created.
+    :raises HedFileError:  
+        - If col_order contains columns not in data and skip_missing is False.
+        - If data corresponds to a filename from which a dataframe cannot be created.
+
     """
     df = get_new_dataframe(data)
     present_cols, missing_cols = separate_values(df.columns.values.tolist(), col_order)
     if missing_cols and not skip_missing:
         raise HedFileError("MissingKeys", f"Events file must have columns {str(missing_cols)}", "")
     df = df[present_cols]
     return df
@@ -272,17 +273,17 @@
         target_values (list):   List of desired values.
 
      Returns:
         tuples:
             list:  Target values present in values.
             list:  Target values missing from values.
 
-     Notes:
+     Notes:  
          - The function computes the set difference of target_cols and base_cols and returns a list
-         of columns of target_cols that are in base_cols and a list of those missing.
+           of columns of target_cols that are in base_cols and a list of those missing.
 
      """
 
     if not target_values:
         return [], []
     elif not values:
         return [], target_values
```

### Comparing `hedtools-0.2.0/hed/tools/util/hed_logger.py` & `hedtools-0.3.0/hed/tools/util/hed_logger.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hed/tools/util/io_util.py` & `hedtools-0.3.0/hed/tools/util/io_util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Utilities for generating and handling file names."""
 
 import os
+import re
 from datetime import datetime
-from werkzeug.utils import secure_filename
 from hed.errors.exceptions import HedFileError
 
 TIME_FORMAT = '%Y_%m_%d_T_%H_%M_%S_%f'
 
 
 def check_filename(test_file, name_prefix=None, name_suffix=None, extensions=None):
     """ Return True if correct extension, suffix, and prefix.
@@ -88,47 +88,27 @@
     suffix_path = os.path.normpath(os.path.realpath(path).lower())
     return_path = os.path.normpath(os.path.realpath(path))
     if suffix_path.startswith(real_prefix):
         return_path = return_path[len(real_prefix):]
     return return_path
 
 
-def generate_filename(base_name, name_prefix=None, name_suffix=None, extension=None, append_datetime=False):
-    """ Generate a filename for the attachment.
+def clean_filename(filename):
+    """ Replaces invalid characters with under-bars
 
     Parameters:
-        base_name (str):   Name of the base, usually the name of the file that the issues were generated from.
-        name_prefix (str): Prefix prepended to the front of the base name.
-        name_suffix (str): Suffix appended to the end of the base name.
-        extension (str):   Extension to use.
-        append_datetime (bool): If True, append the current date-time to the base output filename.
+        filename (str):   source filename
 
     Returns:
-        str:  Name of the attachment other containing the issues.
-
-    Notes:
-        - The form prefix_basename_suffix + extension.
-
+        str:  The filename with anything but alphanumeric, period, hyphens, and under-bars removed.
     """
-
-    pieces = []
-    if name_prefix:
-        pieces = pieces + [name_prefix]
-    if base_name:
-        pieces.append(os.path.splitext(base_name)[0])
-    if name_suffix:
-        pieces = pieces + [name_suffix]
-    filename = "".join(pieces)
-    if append_datetime:
-        now = datetime.now()
-        filename = filename + '_' + now.strftime(TIME_FORMAT)[:-3]
-    if filename and extension:
-        filename = filename + extension
-
-    return secure_filename(filename)
+    if not filename:
+        return ""
+    out_name = re.sub(r'[^a-zA-Z0-9._-]+', '_', filename)
+    return out_name
 
 
 def get_dir_dictionary(dir_path, name_prefix=None, name_suffix=None, extensions=None, skip_empty=True,
                        exclude_dirs=None):
 
     """ Create dictionary directory paths keys.
 
@@ -281,19 +261,19 @@
         file_path (str):     Path to be parsed.
 
     Returns:
         str:   BIDS suffix name.
         str:   File extension (including the .).
         dict:  Dictionary with key-value pair being (entity type, entity value).
 
-        Raises:
-            HedFileError when filename does not conform to name-value_suffix format.
+    :raises HedFileError:
+        - If filename does not conform to name-value_suffix format.
 
-        Notes:
-            into BIDS suffix, extension, and a dictionary of entity name-value pairs.
+    Notes:  
+        - splits into BIDS suffix, extension, and a dictionary of entity name-value pairs.
 
     """
 
     filename = os.path.splitext(os.path.basename(file_path))
     ext = filename[1].lower()
     basename = filename[0].strip()
     entity_dict = {}
```

### Comparing `hedtools-0.2.0/hed/validator/hed_validator.py` & `hedtools-0.3.0/hed/validator/hed_validator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,91 @@
 """
 This module contains the HedValidator class which is used to validate the tags in a HED string or a file. The file
 types include .tsv, .txt, and .xlsx. To get the validation issues after creating a HedValidator class call
 the get_validation_issues() function.
 
 """
 
-from hed.errors.error_types import ValidationErrors
-from hed.errors.error_reporter import ErrorHandler
+from hed.errors.error_types import ValidationErrors, DefinitionErrors
+from hed.errors.error_reporter import ErrorHandler, check_for_any_errors
 
 from hed.models.hed_string import HedString
 from hed.models import HedTag
 from hed.validator.tag_validator import TagValidator
-from functools import partial
-from hed.models.hed_ops import HedOps
+from hed.validator.def_validator import DefValidator
+from hed.validator.onset_validator import OnsetValidator
 
 
-class HedValidator(HedOps):
+class HedValidator:
     """ Top level validation of HED strings. """
 
-    def __init__(self, hed_schema=None, run_semantic_validation=True):
+    def __init__(self, hed_schema=None, def_dicts=None, run_full_onset_checks=True, definitions_allowed=False):
         """ Constructor for the HedValidator class.
 
         Parameters:
             hed_schema (HedSchema or HedSchemaGroup): HedSchema object to use for validation.
-            run_semantic_validation (bool): True if the validator should check the HED data against a schema.
+            def_dicts(DefinitionDict or list or dict): the def dicts to use for validation
+            run_full_onset_checks(bool): If True, check for matching onset/offset tags
+            definitions_allowed(bool): If False, flag definitions found as errors
         """
         super().__init__()
         self._tag_validator = None
         self._hed_schema = hed_schema
 
-        self._tag_validator = TagValidator(hed_schema=self._hed_schema,
-                                           run_semantic_validation=run_semantic_validation)
-        self._run_semantic_validation = run_semantic_validation
-
-    def __get_tag_funcs__(self, **kwargs):
-        string_funcs = []
-        allow_placeholders = kwargs.get("allow_placeholders")
-        check_for_warnings = kwargs.get("check_for_warnings")
-        string_funcs.append(self._tag_validator.run_hed_string_validators)
-        string_funcs.append(
-            partial(HedString.convert_to_canonical_forms, hed_schema=self._hed_schema))
-        string_funcs.append(partial(self._validate_individual_tags_in_hed_string,
-                                    allow_placeholders=allow_placeholders,
-                                    check_for_warnings=check_for_warnings))
-        return string_funcs
-
-    def __get_string_funcs__(self, **kwargs):
-        check_for_warnings = kwargs.get("check_for_warnings")
-        string_funcs = [partial(self._validate_tags_in_hed_string, check_for_warnings=check_for_warnings),
-                        self._validate_groups_in_hed_string]
-        return string_funcs
+        self._tag_validator = TagValidator(hed_schema=self._hed_schema)
+        self._def_validator = DefValidator(def_dicts, hed_schema)
+        self._onset_validator = OnsetValidator(def_dict=self._def_validator,
+                                               run_full_onset_checks=run_full_onset_checks)
+        self._definitions_allowed = definitions_allowed
+
+    def validate(self, hed_string, allow_placeholders, error_handler=None):
+        """
+        Validate the string using the schema
+
+        Parameters:
+            hed_string(HedString): the string to validate
+            allow_placeholders(bool): allow placeholders in the string
+            error_handler(ErrorHandler or None): the error handler to use, creates a default one if none passed
+        Returns:
+            issues (list of dict): A list of issues for hed string
+        """
+        if not error_handler:
+            error_handler = ErrorHandler()
+        issues = []
+        issues += self.run_basic_checks(hed_string, allow_placeholders=allow_placeholders)
+        error_handler.add_context_and_filter(issues)
+        if check_for_any_errors(issues):
+            return issues
+        issues += self.run_full_string_checks(hed_string)
+        error_handler.add_context_and_filter(issues)
+        return issues
+
+    def run_basic_checks(self, hed_string, allow_placeholders):
+        issues = []
+        issues += self._tag_validator.run_hed_string_validators(hed_string, allow_placeholders)
+        if check_for_any_errors(issues):
+            return issues
+        if hed_string == "n/a" or not self._hed_schema:
+            return issues
+        issues += hed_string.convert_to_canonical_forms(self._hed_schema)
+        if check_for_any_errors(issues):
+            return issues
+        # This is required so it can validate the tag a tag expands into
+        # e.g. checking units when a definition placeholder has units
+        self._def_validator.construct_def_tags(hed_string)
+        issues += self._validate_individual_tags_in_hed_string(hed_string, allow_placeholders=allow_placeholders)
+        issues += self._def_validator.validate_def_tags(hed_string, self._tag_validator)
+        return issues
+
+    def run_full_string_checks(self, hed_string):
+        issues = []
+        issues += self._validate_tags_in_hed_string(hed_string)
+        issues += self._validate_groups_in_hed_string(hed_string)
+        issues += self._onset_validator.validate_onset_offset(hed_string)
+        return issues
 
     def _validate_groups_in_hed_string(self, hed_string_obj):
         """ Report invalid groups at each level.
 
         Parameters:
             hed_string_obj (HedString): A HedString object.
 
@@ -99,49 +131,54 @@
 
     def _check_for_duplicate_groups(self, original_group):
         sorted_group = original_group.sorted()
         validation_issues = []
         self._check_for_duplicate_groups_recursive(sorted_group, validation_issues)
         return validation_issues
 
-    def _validate_tags_in_hed_string(self, hed_string_obj, check_for_warnings=False):
-        """ Report invalid the multi-tag properties.
+    def _validate_tags_in_hed_string(self, hed_string_obj):
+        """ Report invalid the multi-tag properties in a hed string, e.g. required tags..
 
          Parameters:
             hed_string_obj (HedString): A HedString object.
 
          Returns:
             list: The issues associated with the tags in the HED string. Each issue is a dictionary.
-
-        Notes:
-            - in a hed string, eg required tags.
-
-         """
+        """
         validation_issues = []
         tags = hed_string_obj.get_all_tags()
-        validation_issues += self._tag_validator.run_all_tags_validators(tags, check_for_warnings=check_for_warnings)
+        validation_issues += self._tag_validator.run_all_tags_validators(tags)
         return validation_issues
 
-    def _validate_individual_tags_in_hed_string(self, hed_string_obj, allow_placeholders=False,
-                                                check_for_warnings=False):
+    def _validate_individual_tags_in_hed_string(self, hed_string_obj, allow_placeholders=False):
         """ Validate individual tags in a HED string.
 
          Parameters:
             hed_string_obj (HedString): A HedString  object.
 
          Returns:
             list: The issues associated with the individual tags. Each issue is a dictionary.
 
          """
         from hed.models.definition_dict import DefTagNames
         validation_issues = []
-        def_groups = hed_string_obj.find_top_level_tags(anchor_tags={DefTagNames.DEFINITION_KEY}, include_groups=1)
-        all_def_groups = [group for sub_group in def_groups for group in sub_group.get_all_groups()]
+        definition_groups = hed_string_obj.find_top_level_tags(anchor_tags={DefTagNames.DEFINITION_KEY},
+                                                               include_groups=1)
+        all_definition_groups = [group for sub_group in definition_groups for group in sub_group.get_all_groups()]
         for group in hed_string_obj.get_all_groups():
-            is_definition = group in all_def_groups
+            is_definition = group in all_definition_groups
             for hed_tag in group.tags():
-                validation_issues += \
-                    self._tag_validator.run_individual_tag_validators(hed_tag, allow_placeholders=allow_placeholders,
-                                                                      check_for_warnings=check_for_warnings,
-                                                                      is_definition=is_definition)
+                if not self._definitions_allowed and hed_tag.short_base_tag == DefTagNames.DEFINITION_ORG_KEY:
+                    validation_issues += ErrorHandler.format_error(DefinitionErrors.BAD_DEFINITION_LOCATION, hed_tag)
+                # todo: unclear if this should be restored at some point
+                # if hed_tag.expandable and not hed_tag.expanded:
+                #     for tag in hed_tag.expandable.get_all_tags():
+                #         validation_issues += self._tag_validator. \
+                #             run_individual_tag_validators(tag, allow_placeholders=allow_placeholders,
+                #                                           is_definition=is_definition)
+                # else:
+                validation_issues += self._tag_validator. \
+                    run_individual_tag_validators(hed_tag,
+                                                  allow_placeholders=allow_placeholders,
+                                                  is_definition=is_definition)
 
         return validation_issues
```

### Comparing `hedtools-0.2.0/hed/validator/tag_validator.py` & `hedtools-0.3.0/hed/validator/tag_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,106 +1,104 @@
 """
 This module is used to validate the HED tags as strings.
 
 """
 
 import re
 from hed.errors.error_reporter import ErrorHandler
+from hed.models.model_constants import DefTagNames
 from hed.schema import HedKey
 from hed.errors.error_types import ValidationErrors
 from hed.validator import tag_validator_util
 
 
 class TagValidator:
     """ Validation for individual HED tags. """
 
-    CAMEL_CASE_EXPRESSION = r'([A-Z-]+\s*[a-z-]*)+'
+    CAMEL_CASE_EXPRESSION = r'([A-Z]+\s*[a-z-]*)+'
     INVALID_STRING_CHARS = '[]{}~'
+    INVALID_STRING_CHARS_PLACEHOLDERS = '[]~'
     OPENING_GROUP_CHARACTER = '('
     CLOSING_GROUP_CHARACTER = ')'
     COMMA = ','
 
     # # sign is allowed by default as it is specifically checked for separately.
     DEFAULT_ALLOWED_PLACEHOLDER_CHARS = ".+-^ _#"
     # Placeholder characters are checked elsewhere, but by default allowed
     TAG_ALLOWED_CHARS = "-_/"
 
-    def __init__(self, hed_schema=None, run_semantic_validation=True):
+    def __init__(self, hed_schema=None):
         """Constructor for the Tag_Validator class.
 
         Parameters:
             hed_schema (HedSchema): A HedSchema object.
-            run_semantic_validation (bool): True if the validator should check the HED data against a schema.
 
         Returns:
             TagValidator: A Tag_Validator object.
 
         """
         self._hed_schema = hed_schema
-        self._run_semantic_validation = run_semantic_validation
-        if not self._hed_schema:
-            self._run_semantic_validation = False
 
         # Dict contains all the value portion validators for value class.  e.g. "is this a number?"
         self._value_unit_validators = self._register_default_value_validators()
 
     # ==========================================================================
     # Top level validator functions
     # =========================================================================+
-    def run_hed_string_validators(self, hed_string_obj):
+    def run_hed_string_validators(self, hed_string_obj, allow_placeholders=False):
         """Basic high level checks of the hed string
 
         Parameters:
             hed_string_obj (HedString): A HED string.
+            allow_placeholders: Allow placeholder and curly brace characters
 
         Returns:
             list: The validation issues associated with a HED string. Each issue is a dictionary.
 
         Notes:
             - Used for basic invalid characters or bad delimiters.
 
          """
         validation_issues = []
-        validation_issues += self.check_invalid_character_issues(hed_string_obj.get_original_hed_string())
+        validation_issues += self.check_invalid_character_issues(hed_string_obj.get_original_hed_string(),
+                                                                 allow_placeholders)
         validation_issues += self.check_count_tag_group_parentheses(hed_string_obj.get_original_hed_string())
         validation_issues += self.check_delimiter_issues_in_hed_string(hed_string_obj.get_original_hed_string())
         for tag in hed_string_obj.get_all_tags():
             validation_issues += self.check_tag_formatting(tag)
         return validation_issues
 
-    def run_individual_tag_validators(self, original_tag, check_for_warnings, allow_placeholders=False,
+    def run_individual_tag_validators(self, original_tag, allow_placeholders=False,
                                       is_definition=False):
         """ Runs the hed_ops on the individual tags.
 
         Parameters:
             original_tag (HedTag): A original tag.
-            check_for_warnings (bool): If True, also check for warnings.
             allow_placeholders (bool): Allow value class or extensions to be placeholders rather than a specific value.
             is_definition (bool): This tag is part of a Definition, not a normal line.
 
         Returns:
             list: The validation issues associated with the top-level tags. Each issue is dictionary.
 
          """
         validation_issues = []
         validation_issues += self.check_tag_invalid_chars(original_tag, allow_placeholders)
-        if self._run_semantic_validation:
-            validation_issues += self.check_tag_exists_in_schema(original_tag, check_for_warnings)
+        if self._hed_schema:
+            validation_issues += self.check_tag_exists_in_schema(original_tag)
             if original_tag.is_unit_class_tag():
-                validation_issues += self.check_tag_unit_class_units_are_valid(original_tag, check_for_warnings)
+                validation_issues += self.check_tag_unit_class_units_are_valid(original_tag)
             elif original_tag.is_value_class_tag():
                 validation_issues += self.check_tag_value_class_valid(original_tag)
-            elif original_tag.extension_or_value_portion:
+            elif original_tag.extension:
                 validation_issues += self.check_for_invalid_extension_chars(original_tag)
 
             if not allow_placeholders:
                 validation_issues += self.check_for_placeholder(original_tag, is_definition)
             validation_issues += self.check_tag_requires_child(original_tag)
-        if check_for_warnings:
-            validation_issues += self.check_capitalization(original_tag)
+        validation_issues += self.check_capitalization(original_tag)
         return validation_issues
 
     def run_tag_level_validators(self, original_tag_list, is_top_level, is_group):
         """ Run hed_ops at each level in a HED string.
 
         Parameters:
             original_tag_list (list): A list containing the original HedTags.
@@ -115,53 +113,56 @@
             - This can contain definitions, Onset, etc tags.
 
         """
         validation_issues = []
         validation_issues += self.check_tag_level_issue(original_tag_list, is_top_level, is_group)
         return validation_issues
 
-    def run_all_tags_validators(self, tags, check_for_warnings):
+    def run_all_tags_validators(self, tags):
         """ Validate the multi-tag properties in a hed string.
 
         Parameters:
             tags (list): A list containing the HedTags in a HED string.
-            check_for_warnings (bool): If True, also check for warnings.
 
         Returns:
             list: The validation issues associated with the tags in a HED string. Each issue is a dictionary.
 
         Notes:
             - Multi-tag properties include required tags.
 
         """
         validation_issues = []
-        if self._run_semantic_validation:
-            if check_for_warnings:
-                validation_issues += self.check_for_required_tags(tags)
+        if self._hed_schema:
+            validation_issues += self.check_for_required_tags(tags)
             validation_issues += self.check_multiple_unique_tags_exist(tags)
         return validation_issues
 
     # ==========================================================================
     # Mostly internal functions to check individual types of errors
     # =========================================================================+
-    def check_invalid_character_issues(self, hed_string):
+    def check_invalid_character_issues(self, hed_string, allow_placeholders):
         """ Report invalid characters.
 
         Parameters:
             hed_string (str): A hed string.
+            allow_placeholders: Allow placeholder and curly brace characters
 
         Returns:
             list: Validation issues. Each issue is a dictionary.
 
         Notes:
-            - Invalid tag characters are defined by TagValidator.INVALID_STRING_CHARS.
+            - Invalid tag characters are defined by TagValidator.INVALID_STRING_CHARS or
+                                                    TagValidator.INVALID_STRING_CHARS_PLACEHOLDERS
         """
         validation_issues = []
+        invalid_dict = TagValidator.INVALID_STRING_CHARS
+        if allow_placeholders:
+            invalid_dict = TagValidator.INVALID_STRING_CHARS_PLACEHOLDERS
         for index, character in enumerate(hed_string):
-            if character in TagValidator.INVALID_STRING_CHARS:
+            if character in invalid_dict or ord(character) > 127:
                 validation_issues += self._report_invalid_character_error(hed_string, index)
 
         return validation_issues
 
     def check_count_tag_group_parentheses(self, hed_string):
         """ Report unmatched parentheses.
 
@@ -171,15 +172,15 @@
         Returns:
             list: A list of validation list. Each issue is a dictionary.
         """
         validation_issues = []
         number_open_parentheses = hed_string.count('(')
         number_closed_parentheses = hed_string.count(')')
         if number_open_parentheses != number_closed_parentheses:
-            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_PARENTHESES_MISMATCH,
+            validation_issues += ErrorHandler.format_error(ValidationErrors.PARENTHESES_MISMATCH,
                                                            opening_parentheses_count=number_open_parentheses,
                                                            closing_parentheses_count=number_closed_parentheses)
         return validation_issues
 
     def check_delimiter_issues_in_hed_string(self, hed_string):
         """ Report missing commas or commas in value tags.
 
@@ -196,32 +197,35 @@
 
         for i, current_character in enumerate(hed_string):
             current_tag += current_character
             if not current_character.strip():
                 continue
             if TagValidator._character_is_delimiter(current_character):
                 if current_tag.strip() == current_character:
-                    issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_EMPTY, source_string=hed_string,
+                    issues += ErrorHandler.format_error(ValidationErrors.TAG_EMPTY, source_string=hed_string,
                                                         char_index=i)
                     current_tag = ''
                     continue
                 current_tag = ''
             elif current_character == self.OPENING_GROUP_CHARACTER:
                 if current_tag.strip() == self.OPENING_GROUP_CHARACTER:
                     current_tag = ''
                 else:
-                    issues += ErrorHandler.format_error(ValidationErrors.HED_COMMA_MISSING, tag=current_tag)
+                    issues += ErrorHandler.format_error(ValidationErrors.COMMA_MISSING, tag=current_tag)
+            elif last_non_empty_valid_character == "," and current_character == self.CLOSING_GROUP_CHARACTER:
+                issues += ErrorHandler.format_error(ValidationErrors.TAG_EMPTY, source_string=hed_string,
+                                                    char_index=i)
             elif TagValidator._comma_is_missing_after_closing_parentheses(last_non_empty_valid_character,
                                                                           current_character):
-                issues += ErrorHandler.format_error(ValidationErrors.HED_COMMA_MISSING, tag=current_tag[:-1])
+                issues += ErrorHandler.format_error(ValidationErrors.COMMA_MISSING, tag=current_tag[:-1])
                 break
             last_non_empty_valid_character = current_character
             last_non_empty_valid_index = i
         if TagValidator._character_is_delimiter(last_non_empty_valid_character):
-            issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_EMPTY,
+            issues += ErrorHandler.format_error(ValidationErrors.TAG_EMPTY,
                                                 char_index=last_non_empty_valid_index,
                                                 source_string=hed_string)
         return issues
 
     pattern_doubleslash = re.compile(r"([ \t/]{2,}|^/|/$)")
 
     def check_tag_formatting(self, original_tag):
@@ -231,15 +235,15 @@
             original_tag (HedTag): The original tag that is used to report the error.
 
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         for match in self.pattern_doubleslash.finditer(original_tag.org_tag):
-            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_NODE_NAME_EMPTY,
+            validation_issues += ErrorHandler.format_error(ValidationErrors.NODE_NAME_EMPTY,
                                                            tag=original_tag,
                                                            index_in_tag=match.start(),
                                                            index_in_tag_end=match.end())
 
         return validation_issues
 
     def check_tag_invalid_chars(self, original_tag, allow_placeholders):
@@ -248,102 +252,129 @@
         Parameters:
             original_tag (HedTag): The original tag that is used to report the error.
             allow_placeholders (bool): Allow placeholder characters(#) if True.
 
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
+        validation_issues = self._check_invalid_prefix_issues(original_tag)
         allowed_chars = self.TAG_ALLOWED_CHARS
         if not self._hed_schema or not self._hed_schema.is_hed3_schema:
             allowed_chars += " "
         if allow_placeholders:
             allowed_chars += "#"
-        return self._check_invalid_chars(original_tag.org_base_tag, allowed_chars, original_tag)
+        validation_issues += self._check_invalid_chars(original_tag.org_base_tag, allowed_chars, original_tag)
+        return validation_issues
 
-    def check_tag_exists_in_schema(self, original_tag, check_for_warnings=False):
+    def check_tag_exists_in_schema(self, original_tag):
         """ Report invalid tag or doesn't take a value.
 
         Parameters:
             original_tag (HedTag): The original tag that is used to report the error.
-            check_for_warnings (bool): If True, also check for warnings.
 
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         if original_tag.is_basic_tag() or original_tag.is_takes_value_tag():
             return validation_issues
 
         is_extension_tag = original_tag.is_extension_allowed_tag()
         if not is_extension_tag:
-            validation_issues += ErrorHandler.format_error(ValidationErrors.INVALID_EXTENSION, tag=original_tag)
-        elif check_for_warnings:
-            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_EXTENDED, tag=original_tag,
+            actual_error = None
+            if "#" in original_tag.extension:
+                actual_error = ValidationErrors.PLACEHOLDER_INVALID
+            validation_issues += ErrorHandler.format_error(ValidationErrors.TAG_EXTENSION_INVALID, tag=original_tag,
+                                                           actual_error=actual_error)
+        else:
+            validation_issues += ErrorHandler.format_error(ValidationErrors.TAG_EXTENDED, tag=original_tag,
                                                            index_in_tag=len(original_tag.org_base_tag),
                                                            index_in_tag_end=None)
         return validation_issues
 
-    def check_tag_unit_class_units_are_valid(self, original_tag, check_for_warnings):
+    def check_tag_unit_class_units_are_valid(self, original_tag, report_as=None, error_code=None):
         """ Report incorrect unit class or units.
 
         Parameters:
             original_tag (HedTag): The original tag that is used to report the error.
-            check_for_warnings (bool): Indicates whether to check for warnings.
-
+            report_as (HedTag): Report errors as coming from this tag, rather than original_tag.
+            error_code (str): Override error codes to this
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         if original_tag.is_unit_class_tag():
             stripped_value, unit = original_tag.get_stripped_unit_value()
             if not unit:
-                if self._validate_value_class_portion(original_tag, stripped_value):
-                    if check_for_warnings:
-                        # only suggest a unit is missing if this is a valid number
-                        if tag_validator_util.validate_numeric_value_class(stripped_value):
-                            default_unit = original_tag.get_unit_class_default_unit()
-                            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_UNITS_DEFAULT_USED,
-                                                                           tag=original_tag,
-                                                                           default_unit=default_unit)
-                else:
+                bad_units = " " in original_tag.extension
+                had_error = False
+                # Todo: in theory this should separately validate the number and the units, for units
+                # that are prefixes like $.  Right now those are marked as unit invalid AND value_invalid.
+                if bad_units:
+                    stripped_value = stripped_value.split(" ")[0]
+                if original_tag.is_takes_value_tag() and\
+                        not self._validate_value_class_portion(original_tag, stripped_value):
+                    validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID,
+                                                                   report_as if report_as else original_tag)
+                    if error_code:
+                        had_error = True
+                        validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID,
+                                                                       report_as if report_as else original_tag,
+                                                                       actual_error=error_code)
+
+                if bad_units:
                     tag_unit_class_units = original_tag.get_tag_unit_class_units()
                     if tag_unit_class_units:
-                        validation_issues += ErrorHandler.format_error(ValidationErrors.HED_UNITS_INVALID,
-                                                                       original_tag,
-                                                                       unit_class_units=tag_unit_class_units)
+                        validation_issues += ErrorHandler.format_error(ValidationErrors.UNITS_INVALID,
+                                                                       tag=report_as if report_as else original_tag,
+                                                                       units=tag_unit_class_units)
+                else:
+                    default_unit = original_tag.get_unit_class_default_unit()
+                    validation_issues += ErrorHandler.format_error(ValidationErrors.UNITS_MISSING,
+                                                                   tag=report_as if report_as else original_tag,
+                                                                   default_unit=default_unit)
+
+                # We don't want to give this overall error twice
+                if error_code and not had_error:
+                    new_issue = validation_issues[0].copy()
+                    new_issue['code'] = error_code
+                    validation_issues += [new_issue]
+
         return validation_issues
 
-    def check_tag_value_class_valid(self, original_tag):
+    def check_tag_value_class_valid(self, original_tag, report_as=None, error_code=None):
         """ Report an invalid value portion.
 
         Parameters:
             original_tag (HedTag): The original tag that is used to report the error.
-
+            report_as (HedTag): Report errors as coming from this tag, rather than original_tag.
+            error_code (str): Override error codes to this
         Returns:
             list: Validation issues.
         """
         validation_issues = []
-        if not self._validate_value_class_portion(original_tag, original_tag.extension_or_value_portion):
-            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_VALUE_INVALID,
-                                                           original_tag)
+        if not self._validate_value_class_portion(original_tag, original_tag.extension):
+            validation_issues += ErrorHandler.format_error(ValidationErrors.VALUE_INVALID,
+                                                           report_as if report_as else original_tag,
+                                                           actual_error=error_code)
 
         return validation_issues
 
     def check_tag_requires_child(self, original_tag):
         """ Report if tag is a leaf with 'requiredTag' attribute.
 
         Parameters:
             original_tag (HedTag): The original tag that is used to report the error.
 
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         if original_tag.has_attribute(HedKey.RequireChild):
-            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_REQUIRES_CHILD,
+            validation_issues += ErrorHandler.format_error(ValidationErrors.TAG_REQUIRES_CHILD,
                                                            tag=original_tag)
         return validation_issues
 
     def check_tag_unit_class_units_exist(self, original_tag):
         """ Report warning if tag has a unit class tag with no units.
 
         Parameters:
@@ -351,18 +382,18 @@
 
         Returns:
             list: Validation issues.  Each issue is a dictionary.
 
         """
         validation_issues = []
         if original_tag.is_unit_class_tag():
-            tag_unit_values = original_tag.extension_or_value_portion
+            tag_unit_values = original_tag.extension
             if tag_validator_util.validate_numeric_value_class(tag_unit_values):
                 default_unit = original_tag.get_unit_class_default_unit()
-                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_UNITS_DEFAULT_USED,
+                validation_issues += ErrorHandler.format_error(ValidationErrors.UNITS_MISSING,
                                                                tag=original_tag,
                                                                default_unit=default_unit)
         return validation_issues
 
     def check_for_invalid_extension_chars(self, original_tag):
         """Report invalid characters in extension/value.
 
@@ -371,15 +402,15 @@
 
         Returns:
             list: Validation issues. Each issue is a dictionary.
         """
         allowed_chars = self.TAG_ALLOWED_CHARS
         allowed_chars += self.DEFAULT_ALLOWED_PLACEHOLDER_CHARS
         allowed_chars += " "
-        return self._check_invalid_chars(original_tag.extension_or_value_portion, allowed_chars, original_tag,
+        return self._check_invalid_chars(original_tag.extension, allowed_chars, original_tag,
                                          starting_index=len(original_tag.org_base_tag) + 1)
 
     def check_capitalization(self, original_tag):
         """Report warning if incorrect tag capitalization.
 
         Parameters:
             original_tag (HedTag): The original tag used to report the warning.
@@ -388,15 +419,15 @@
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         tag_names = original_tag.org_base_tag.split("/")
         for tag_name in tag_names:
             correct_tag_name = tag_name.capitalize()
             if tag_name != correct_tag_name and not re.search(self.CAMEL_CASE_EXPRESSION, tag_name):
-                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_STYLE_WARNING,
+                validation_issues += ErrorHandler.format_error(ValidationErrors.STYLE_WARNING,
                                                                tag=original_tag)
                 break
         return validation_issues
 
     def check_tag_level_issue(self, original_tag_list, is_top_level, is_group):
         """ Report tags incorrectly positioned in hierarchy.
 
@@ -408,32 +439,41 @@
         Returns:
             list: Validation issues. Each issue is a dictionary.
 
         Notes:
             - Top-level groups can contain definitions, Onset, etc tags.
         """
         validation_issues = []
-        if self._run_semantic_validation:
-            top_level_tags = [tag for tag in original_tag_list if
-                              tag.base_tag_has_attribute(HedKey.TopLevelTagGroup)]
-            tag_group_tags = [tag for tag in original_tag_list if
-                              tag.base_tag_has_attribute(HedKey.TagGroup)]
-            for tag_group_tag in tag_group_tags:
-                if not is_group:
-                    validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_GROUP_TAG,
-                                                                   tag=tag_group_tag)
-            for top_level_tag in top_level_tags:
-                if not is_top_level:
-                    validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TOP_LEVEL_TAG,
-                                                                   tag=top_level_tag)
+        top_level_tags = [tag for tag in original_tag_list if
+                          tag.base_tag_has_attribute(HedKey.TopLevelTagGroup)]
+        tag_group_tags = [tag for tag in original_tag_list if
+                          tag.base_tag_has_attribute(HedKey.TagGroup)]
+        for tag_group_tag in tag_group_tags:
+            if not is_group:
+                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_GROUP_TAG,
+                                                               tag=tag_group_tag)
+        for top_level_tag in top_level_tags:
+            if not is_top_level:
+                actual_code = None
+                if top_level_tag.short_base_tag == DefTagNames.DEFINITION_ORG_KEY:
+                    actual_code = ValidationErrors.DEFINITION_INVALID
+                elif top_level_tag.short_base_tag in {DefTagNames.ONSET_ORG_KEY, DefTagNames.OFFSET_ORG_KEY}:
+                    actual_code = ValidationErrors.ONSET_OFFSET_INSET_ERROR
 
-            if is_top_level and len(top_level_tags) > 1:
-                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_MULTIPLE_TOP_TAGS,
-                                                               tag=top_level_tags[0],
-                                                               multiple_tags=top_level_tags[1:])
+                if actual_code:
+                    validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TOP_LEVEL_TAG,
+                                                                   tag=top_level_tag,
+                                                                   actual_error=actual_code)
+                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TOP_LEVEL_TAG,
+                                                               tag=top_level_tag)
+
+        if is_top_level and len(top_level_tags) > 1:
+            validation_issues += ErrorHandler.format_error(ValidationErrors.HED_MULTIPLE_TOP_TAGS,
+                                                           tag=top_level_tags[0],
+                                                           multiple_tags=top_level_tags[1:])
 
         return validation_issues
 
     def check_for_required_tags(self, tags):
         """ Report missing required tags.
 
         Parameters:
@@ -443,16 +483,16 @@
             list: Validation issues. Each issue is a dictionary.
 
         """
         validation_issues = []
         required_prefixes = self._hed_schema.get_tags_with_attribute(HedKey.Required)
         for required_prefix in required_prefixes:
             if not any(tag.long_tag.lower().startswith(required_prefix.lower()) for tag in tags):
-                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_REQUIRED_TAG_MISSING,
-                                                               tag_prefix=required_prefix)
+                validation_issues += ErrorHandler.format_error(ValidationErrors.REQUIRED_TAG_MISSING,
+                                                               tag_namespace=required_prefix)
         return validation_issues
 
     def check_multiple_unique_tags_exist(self, tags):
         """ Report if multiple identical unique tags exist
 
             A unique Term can only appear once in a given HedString.
             Unique terms are terms with the 'unique' property in the schema.
@@ -464,21 +504,30 @@
             list: Validation issues. Each issue is a dictionary.
         """
         validation_issues = []
         unique_prefixes = self._hed_schema.get_tags_with_attribute(HedKey.Unique)
         for unique_prefix in unique_prefixes:
             unique_tag_prefix_bool_mask = [x.long_tag.lower().startswith(unique_prefix.lower()) for x in tags]
             if sum(unique_tag_prefix_bool_mask) > 1:
-                validation_issues += ErrorHandler.format_error(ValidationErrors.HED_TAG_NOT_UNIQUE,
-                                                               tag_prefix=unique_prefix)
+                validation_issues += ErrorHandler.format_error(ValidationErrors.TAG_NOT_UNIQUE,
+                                                               tag_namespace=unique_prefix)
         return validation_issues
 
     # ==========================================================================
     # Private utility functions
     # =========================================================================+
+    def _check_invalid_prefix_issues(self, original_tag):
+        """Check for invalid schema namespace."""
+        issues = []
+        schema_namespace = original_tag.schema_namespace
+        if schema_namespace and not schema_namespace[:-1].isalpha():
+            issues += ErrorHandler.format_error(ValidationErrors.TAG_NAMESPACE_PREFIX_INVALID,
+                                                tag=original_tag, tag_namespace=schema_namespace)
+        return issues
+
     def _validate_value_class_portion(self, original_tag, portion_to_validate):
         if portion_to_validate is None:
             return False
 
         value_class_types = original_tag.value_classes
         return self.validate_value_class_type(portion_to_validate, value_class_types)
 
@@ -489,18 +538,18 @@
             hed_string (str): The HED string that caused the error.
             index (int): The index of the invalid character in the HED string.
 
         Returns:
             list: A singleton list with a dictionary representing the error.
 
         """
-        error_type = ValidationErrors.HED_CHARACTER_INVALID
+        error_type = ValidationErrors.CHARACTER_INVALID
         character = hed_string[index]
         if character == "~":
-            error_type = ValidationErrors.HED_TILDES_UNSUPPORTED
+            error_type = ValidationErrors.TILDES_UNSUPPORTED
         return ErrorHandler.format_error(error_type, char_index=index,
                                          source_string=hed_string)
 
     @staticmethod
     def _comma_is_missing_after_closing_parentheses(last_non_empty_character, current_character):
         """ Checks if missing comma after a closing parentheses.
 
@@ -548,21 +597,21 @@
         Notes:
             - Invalid placeholder may appear in the extension/value portion of a tag.
 
         """
         validation_issues = []
         if not is_definition:
             starting_index = len(original_tag.org_base_tag) + 1
-            for i, character in enumerate(original_tag.extension_or_value_portion):
+            for i, character in enumerate(original_tag.extension):
                 if character == "#":
                     validation_issues += ErrorHandler.format_error(ValidationErrors.INVALID_TAG_CHARACTER,
                                                                    tag=original_tag,
                                                                    index_in_tag=starting_index + i,
                                                                    index_in_tag_end=starting_index + i + 1,
-                                                                   actual_error=ValidationErrors.HED_VALUE_INVALID)
+                                                                   actual_error=ValidationErrors.PLACEHOLDER_INVALID)
 
         return validation_issues
 
     def _check_invalid_chars(self, check_string, allowed_chars, source_tag, starting_index=0):
         validation_issues = []
         for i, character in enumerate(check_string):
             if character.isalnum():
```

### Comparing `hedtools-0.2.0/hed/validator/tag_validator_util.py` & `hedtools-0.3.0/hed/validator/tag_validator_util.py`

 * *Files identical despite different names*

### Comparing `hedtools-0.2.0/hedtools.egg-info/PKG-INFO` & `hedtools-0.3.0/hedtools.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 Metadata-Version: 2.1
 Name: hedtools
-Version: 0.2.0
+Version: 0.3.0
 Summary: HED validation, summary, and analysis tools.
 Home-page: https://github.com/hed-standard/hed-python/
 Author: VisLab, Ian Callanan, Jeremy Cockfield, Alexander Jones, Owen Winterberg, Kay Robbins
 Author-email: Kay.Robbins@utsa.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8056010.svg)](https://doi.org/10.5281/zenodo.8056010)
+[![Maintainability](https://api.codeclimate.com/v1/badges/11bf2329590e7b0164ba/maintainability)](https://codeclimate.com/github/hed-standard/hed-python/maintainability)
+[![Test Coverage](https://api.codeclimate.com/v1/badges/11bf2329590e7b0164ba/test_coverage)](https://codeclimate.com/github/hed-standard/hed-python/test_coverage)
+![PyPI - Status](https://img.shields.io/pypi/v/hedtools)
+
+
 # HEDTools - Python
 HED (Hierarchical Event Descriptors) is a framework for systematically describing
 both laboratory and real-world events as well as other experimental metadata.
 HED tags are comma-separated path strings.
 HED, itself, is platform-independent, extendable, and data-neutral. 
 
 This repository contains the underlying python tools that support validation,
 summarization, and analysis of datasets using HED tags.
 
 Most people will simply annotate their events by creating a spreadsheet
 or a BIDS JSON sidecar that associates HED tags with event codes or the events themselves.
 If you have such a spreadsheet or a JSON, 
 you can use the HED Online Validator currently available at 
-[https://hedtools.ucsd.edu/hed](https://hedtools.ucsd.edu/hed) to validate or transform
+[https://hedtools.org](https://hedtools.org) to validate or transform
 your files without downloading any tools. 
 
 A version of the online tools corresponding to the `develop` branch can be found at:
-[https://hedtools.ucsd.edu/hed_dev](https://hedtools.ucsd.edu/hed_dev).
+[https://hedtools.org/hed_dev](https://hedtools.org/hed_dev).
 
 ### Installation
 Use `pip` to install `hedtools` from PyPI:
 
    ```
        pip install hedtools
    ```
@@ -105,12 +111,12 @@
 Cached Schemas by default are stored in "home/.hedtools/" 
 Location of "home" directory varies by OS.
 
 Use `hed.schema.set_cache_directory` to change the location.
 The HED cache can be shared across processes.
 
 Starting with `hedtools 0.2.0` local copies of the most recent schema versions
-are stored within the code modules for easy access.
+are stored within the code modules for easy access.  
 
 ### Other links of interest
 
 Code climate reports: [https://codeclimate.com/github/hed-standard/hed-python](https://codeclimate.com/github/hed-standard/hed-python).
```

### Comparing `hedtools-0.2.0/hedtools.egg-info/SOURCES.txt` & `hedtools-0.3.0/hedtools.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -13,27 +13,25 @@
 ./hed/errors/error_reporter.py
 ./hed/errors/error_types.py
 ./hed/errors/exceptions.py
 ./hed/models/__init__.py
 ./hed/models/base_input.py
 ./hed/models/column_mapper.py
 ./hed/models/column_metadata.py
-./hed/models/def_mapper.py
+./hed/models/def_expand_gather.py
 ./hed/models/definition_dict.py
 ./hed/models/definition_entry.py
+./hed/models/df_util.py
 ./hed/models/expression_parser.py
 ./hed/models/hed_group.py
-./hed/models/hed_ops.py
 ./hed/models/hed_string.py
 ./hed/models/hed_string_group.py
 ./hed/models/hed_tag.py
 ./hed/models/model_constants.py
-./hed/models/onset_mapper.py
 ./hed/models/sidecar.py
-./hed/models/sidecar_base.py
 ./hed/models/spreadsheet_input.py
 ./hed/models/tabular_input.py
 ./hed/models/timeseries_input.py
 ./hed/schema/__init__.py
 ./hed/schema/hed_cache.py
 ./hed/schema/hed_schema.py
 ./hed/schema/hed_schema_constants.py
@@ -41,39 +39,43 @@
 ./hed/schema/hed_schema_group.py
 ./hed/schema/hed_schema_io.py
 ./hed/schema/hed_schema_section.py
 ./hed/schema/schema_compliance.py
 ./hed/schema/schema_validation_util.py
 ./hed/schema/schema_data/HED8.0.0.xml
 ./hed/schema/schema_data/HED8.1.0.xml
+./hed/schema/schema_data/HED8.2.0.xml
 ./hed/schema/schema_data/HED_score_1.0.0.xml
 ./hed/schema/schema_data/HED_testlib_1.0.2.xml
 ./hed/schema/schema_io/__init__.py
+./hed/schema/schema_io/schema2base.py
 ./hed/schema/schema_io/schema2wiki.py
 ./hed/schema/schema_io/schema2xml.py
 ./hed/schema/schema_io/schema_util.py
 ./hed/schema/schema_io/wiki2schema.py
 ./hed/schema/schema_io/wiki_constants.py
 ./hed/schema/schema_io/xml2schema.py
 ./hed/schema/schema_io/xml_constants.py
 ./hed/tools/__init__.py
 ./hed/tools/analysis/__init__.py
 ./hed/tools/analysis/analysis_util.py
 ./hed/tools/analysis/annotation_util.py
-./hed/tools/analysis/column_name_summary.py
+./hed/tools/analysis/event_manager.py
 ./hed/tools/analysis/file_dictionary.py
 ./hed/tools/analysis/hed_context_manager.py
 ./hed/tools/analysis/hed_tag_counts.py
 ./hed/tools/analysis/hed_type_counts.py
 ./hed/tools/analysis/hed_type_definitions.py
 ./hed/tools/analysis/hed_type_factors.py
 ./hed/tools/analysis/hed_type_manager.py
 ./hed/tools/analysis/hed_type_values.py
 ./hed/tools/analysis/key_map.py
+./hed/tools/analysis/tabular_column_name_summary.py
 ./hed/tools/analysis/tabular_summary.py
+./hed/tools/analysis/temporal_event.py
 ./hed/tools/bids/__init__.py
 ./hed/tools/bids/bids_dataset.py
 ./hed/tools/bids/bids_file.py
 ./hed/tools/bids/bids_file_dictionary.py
 ./hed/tools/bids/bids_file_group.py
 ./hed/tools/bids/bids_sidecar_file.py
 ./hed/tools/bids/bids_tabular_dictionary.py
@@ -82,67 +84,72 @@
 ./hed/tools/remodeling/backup_manager.py
 ./hed/tools/remodeling/dispatcher.py
 ./hed/tools/remodeling/cli/__init__.py
 ./hed/tools/remodeling/cli/run_remodel.py
 ./hed/tools/remodeling/cli/run_remodel_backup.py
 ./hed/tools/remodeling/cli/run_remodel_restore.py
 ./hed/tools/remodeling/operations/__init__.py
-./hed/tools/remodeling/operations/base_context.py
 ./hed/tools/remodeling/operations/base_op.py
+./hed/tools/remodeling/operations/base_summary.py
+./hed/tools/remodeling/operations/convert_columns_op.py
 ./hed/tools/remodeling/operations/factor_column_op.py
 ./hed/tools/remodeling/operations/factor_hed_tags_op.py
 ./hed/tools/remodeling/operations/factor_hed_type_op.py
 ./hed/tools/remodeling/operations/merge_consecutive_op.py
 ./hed/tools/remodeling/operations/number_groups_op.py
 ./hed/tools/remodeling/operations/number_rows_op.py
 ./hed/tools/remodeling/operations/remap_columns_op.py
 ./hed/tools/remodeling/operations/remove_columns_op.py
 ./hed/tools/remodeling/operations/remove_rows_op.py
 ./hed/tools/remodeling/operations/rename_columns_op.py
 ./hed/tools/remodeling/operations/reorder_columns_op.py
 ./hed/tools/remodeling/operations/split_rows_op.py
 ./hed/tools/remodeling/operations/summarize_column_names_op.py
 ./hed/tools/remodeling/operations/summarize_column_values_op.py
+./hed/tools/remodeling/operations/summarize_definitions_op.py
 ./hed/tools/remodeling/operations/summarize_hed_tags_op.py
 ./hed/tools/remodeling/operations/summarize_hed_type_op.py
 ./hed/tools/remodeling/operations/summarize_hed_validation_op.py
 ./hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
 ./hed/tools/remodeling/operations/valid_operations.py
 ./hed/tools/util/__init__.py
 ./hed/tools/util/data_util.py
 ./hed/tools/util/hed_logger.py
 ./hed/tools/util/io_util.py
+./hed/tools/util/schema_util.py
 ./hed/validator/__init__.py
+./hed/validator/def_validator.py
 ./hed/validator/hed_validator.py
+./hed/validator/onset_validator.py
+./hed/validator/sidecar_validator.py
+./hed/validator/spreadsheet_validator.py
 ./hed/validator/tag_validator.py
 ./hed/validator/tag_validator_util.py
 hed/__init__.py
 hed/_version.py
 hed/errors/__init__.py
 hed/errors/error_messages.py
 hed/errors/error_reporter.py
 hed/errors/error_types.py
 hed/errors/exceptions.py
 hed/models/__init__.py
 hed/models/base_input.py
 hed/models/column_mapper.py
 hed/models/column_metadata.py
-hed/models/def_mapper.py
+hed/models/def_expand_gather.py
 hed/models/definition_dict.py
 hed/models/definition_entry.py
+hed/models/df_util.py
 hed/models/expression_parser.py
 hed/models/hed_group.py
-hed/models/hed_ops.py
 hed/models/hed_string.py
 hed/models/hed_string_group.py
 hed/models/hed_tag.py
 hed/models/model_constants.py
-hed/models/onset_mapper.py
 hed/models/sidecar.py
-hed/models/sidecar_base.py
 hed/models/spreadsheet_input.py
 hed/models/tabular_input.py
 hed/models/timeseries_input.py
 hed/schema/__init__.py
 hed/schema/hed_cache.py
 hed/schema/hed_schema.py
 hed/schema/hed_schema_constants.py
@@ -150,39 +157,43 @@
 hed/schema/hed_schema_group.py
 hed/schema/hed_schema_io.py
 hed/schema/hed_schema_section.py
 hed/schema/schema_compliance.py
 hed/schema/schema_validation_util.py
 hed/schema/schema_data/HED8.0.0.xml
 hed/schema/schema_data/HED8.1.0.xml
+hed/schema/schema_data/HED8.2.0.xml
 hed/schema/schema_data/HED_score_1.0.0.xml
 hed/schema/schema_data/HED_testlib_1.0.2.xml
 hed/schema/schema_io/__init__.py
+hed/schema/schema_io/schema2base.py
 hed/schema/schema_io/schema2wiki.py
 hed/schema/schema_io/schema2xml.py
 hed/schema/schema_io/schema_util.py
 hed/schema/schema_io/wiki2schema.py
 hed/schema/schema_io/wiki_constants.py
 hed/schema/schema_io/xml2schema.py
 hed/schema/schema_io/xml_constants.py
 hed/tools/__init__.py
 hed/tools/analysis/__init__.py
 hed/tools/analysis/analysis_util.py
 hed/tools/analysis/annotation_util.py
-hed/tools/analysis/column_name_summary.py
+hed/tools/analysis/event_manager.py
 hed/tools/analysis/file_dictionary.py
 hed/tools/analysis/hed_context_manager.py
 hed/tools/analysis/hed_tag_counts.py
 hed/tools/analysis/hed_type_counts.py
 hed/tools/analysis/hed_type_definitions.py
 hed/tools/analysis/hed_type_factors.py
 hed/tools/analysis/hed_type_manager.py
 hed/tools/analysis/hed_type_values.py
 hed/tools/analysis/key_map.py
+hed/tools/analysis/tabular_column_name_summary.py
 hed/tools/analysis/tabular_summary.py
+hed/tools/analysis/temporal_event.py
 hed/tools/bids/__init__.py
 hed/tools/bids/bids_dataset.py
 hed/tools/bids/bids_file.py
 hed/tools/bids/bids_file_dictionary.py
 hed/tools/bids/bids_file_group.py
 hed/tools/bids/bids_sidecar_file.py
 hed/tools/bids/bids_tabular_dictionary.py
@@ -191,41 +202,48 @@
 hed/tools/remodeling/backup_manager.py
 hed/tools/remodeling/dispatcher.py
 hed/tools/remodeling/cli/__init__.py
 hed/tools/remodeling/cli/run_remodel.py
 hed/tools/remodeling/cli/run_remodel_backup.py
 hed/tools/remodeling/cli/run_remodel_restore.py
 hed/tools/remodeling/operations/__init__.py
-hed/tools/remodeling/operations/base_context.py
 hed/tools/remodeling/operations/base_op.py
+hed/tools/remodeling/operations/base_summary.py
+hed/tools/remodeling/operations/convert_columns_op.py
 hed/tools/remodeling/operations/factor_column_op.py
 hed/tools/remodeling/operations/factor_hed_tags_op.py
 hed/tools/remodeling/operations/factor_hed_type_op.py
 hed/tools/remodeling/operations/merge_consecutive_op.py
 hed/tools/remodeling/operations/number_groups_op.py
 hed/tools/remodeling/operations/number_rows_op.py
 hed/tools/remodeling/operations/remap_columns_op.py
 hed/tools/remodeling/operations/remove_columns_op.py
 hed/tools/remodeling/operations/remove_rows_op.py
 hed/tools/remodeling/operations/rename_columns_op.py
 hed/tools/remodeling/operations/reorder_columns_op.py
 hed/tools/remodeling/operations/split_rows_op.py
 hed/tools/remodeling/operations/summarize_column_names_op.py
 hed/tools/remodeling/operations/summarize_column_values_op.py
+hed/tools/remodeling/operations/summarize_definitions_op.py
 hed/tools/remodeling/operations/summarize_hed_tags_op.py
 hed/tools/remodeling/operations/summarize_hed_type_op.py
 hed/tools/remodeling/operations/summarize_hed_validation_op.py
 hed/tools/remodeling/operations/summarize_sidecar_from_events_op.py
 hed/tools/remodeling/operations/valid_operations.py
 hed/tools/util/__init__.py
 hed/tools/util/data_util.py
 hed/tools/util/hed_logger.py
 hed/tools/util/io_util.py
+hed/tools/util/schema_util.py
 hed/validator/__init__.py
+hed/validator/def_validator.py
 hed/validator/hed_validator.py
+hed/validator/onset_validator.py
+hed/validator/sidecar_validator.py
+hed/validator/spreadsheet_validator.py
 hed/validator/tag_validator.py
 hed/validator/tag_validator_util.py
 hedtools.egg-info/PKG-INFO
 hedtools.egg-info/SOURCES.txt
 hedtools.egg-info/dependency_links.txt
 hedtools.egg-info/entry_points.txt
 hedtools.egg-info/requires.txt
```

### Comparing `hedtools-0.2.0/setup.cfg` & `hedtools-0.3.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -43,44 +43,43 @@
 000002a0: 6c0d 0a09 6574 2d78 6d6c 6669 6c65 0d0a  l...et-xmlfile..
 000002b0: 0969 6e66 6c65 6374 0d0a 096a 6463 616c  .inflect...jdcal
 000002c0: 0d0a 096e 756d 7079 0d0a 096f 7065 6e70  ...numpy...openp
 000002d0: 7978 6c0d 0a09 7061 6e64 6173 0d0a 0970  yxl...pandas...p
 000002e0: 6f72 7461 6c6f 636b 6572 0d0a 0970 7974  ortalocker...pyt
 000002f0: 686f 6e2d 6461 7465 7574 696c 0d0a 0970  hon-dateutil...p
 00000300: 7974 7a0d 0a09 7365 6d61 6e74 6963 2d76  ytz...semantic-v
-00000310: 6572 7369 6f6e 0d0a 0973 6978 0d0a 0957  ersion...six...W
-00000320: 6572 6b7a 6575 670d 0a0d 0a5b 6f70 7469  erkzeug....[opti
-00000330: 6f6e 732e 7061 636b 6167 6573 2e66 696e  ons.packages.fin
-00000340: 645d 0d0a 696e 636c 7564 6520 3d20 6865  d]..include = he
-00000350: 642a 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  d*....[options.p
-00000360: 6163 6b61 6765 5f64 6174 615d 0d0a 6865  ackage_data]..he
-00000370: 6420 3d20 7363 6865 6d61 2f73 6368 656d  d = schema/schem
-00000380: 615f 6461 7461 2f2a 2e78 6d6c 0d0a 0d0a  a_data/*.xml....
-00000390: 5b6f 7074 696f 6e73 2e65 6e74 7279 5f70  [options.entry_p
-000003a0: 6f69 6e74 735d 0d0a 636f 6e73 6f6c 655f  oints]..console_
-000003b0: 7363 7269 7074 7320 3d20 0d0a 0972 756e  scripts = ...run
-000003c0: 5f72 656d 6f64 656c 3d68 6564 2e74 6f6f  _remodel=hed.too
-000003d0: 6c73 2e72 656d 6f64 656c 696e 672e 636c  ls.remodeling.cl
-000003e0: 692e 7275 6e5f 7265 6d6f 6465 6c3a 6d61  i.run_remodel:ma
-000003f0: 696e 0d0a 0972 756e 5f72 656d 6f64 656c  in...run_remodel
-00000400: 5f62 6163 6b75 703d 6865 642e 746f 6f6c  _backup=hed.tool
-00000410: 732e 7265 6d6f 6465 6c69 6e67 2e63 6c69  s.remodeling.cli
-00000420: 2e72 756e 5f72 656d 6f64 656c 5f62 6163  .run_remodel_bac
-00000430: 6b75 703a 6d61 696e 0d0a 0972 756e 5f72  kup:main...run_r
-00000440: 656d 6f64 656c 5f72 6573 746f 7265 3d68  emodel_restore=h
-00000450: 6564 2e74 6f6f 6c73 2e72 656d 6f64 656c  ed.tools.remodel
-00000460: 696e 672e 636c 692e 7275 6e5f 7265 6d6f  ing.cli.run_remo
-00000470: 6465 6c5f 7265 7374 6f72 653a 6d61 696e  del_restore:main
-00000480: 0d0a 0d0a 5b76 6572 7369 6f6e 6565 725d  ....[versioneer]
-00000490: 0d0a 5643 5320 3d20 6769 740d 0a73 7479  ..VCS = git..sty
-000004a0: 6c65 203d 2070 6570 3434 300d 0a76 6572  le = pep440..ver
-000004b0: 7369 6f6e 6669 6c65 5f73 6f75 7263 6520  sionfile_source 
-000004c0: 3d20 6865 642f 5f76 6572 7369 6f6e 2e70  = hed/_version.p
-000004d0: 790d 0a76 6572 7369 6f6e 6669 6c65 5f62  y..versionfile_b
-000004e0: 7569 6c64 203d 2068 6564 2f5f 7665 7273  uild = hed/_vers
-000004f0: 696f 6e2e 7079 0d0a 7461 675f 7072 6566  ion.py..tag_pref
-00000500: 6978 203d 200d 0a70 6172 656e 7464 6972  ix = ..parentdir
-00000510: 5f70 7265 6669 7820 3d20 6865 6474 6f6f  _prefix = hedtoo
-00000520: 6c73 2d0d 0a0d 0a5b 6567 675f 696e 666f  ls-....[egg_info
-00000530: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
-00000540: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
-00000550: 0a                                       .
+00000310: 6572 7369 6f6e 0d0a 0973 6978 0d0a 0d0a  ersion...six....
+00000320: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
+00000330: 732e 6669 6e64 5d0d 0a69 6e63 6c75 6465  s.find]..include
+00000340: 203d 2068 6564 2a0d 0a0d 0a5b 6f70 7469   = hed*....[opti
+00000350: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
+00000360: 5d0d 0a68 6564 203d 2073 6368 656d 612f  ]..hed = schema/
+00000370: 7363 6865 6d61 5f64 6174 612f 2a2e 786d  schema_data/*.xm
+00000380: 6c0d 0a0d 0a5b 6f70 7469 6f6e 732e 656e  l....[options.en
+00000390: 7472 795f 706f 696e 7473 5d0d 0a63 6f6e  try_points]..con
+000003a0: 736f 6c65 5f73 6372 6970 7473 203d 200d  sole_scripts = .
+000003b0: 0a09 7275 6e5f 7265 6d6f 6465 6c3d 6865  ..run_remodel=he
+000003c0: 642e 746f 6f6c 732e 7265 6d6f 6465 6c69  d.tools.remodeli
+000003d0: 6e67 2e63 6c69 2e72 756e 5f72 656d 6f64  ng.cli.run_remod
+000003e0: 656c 3a6d 6169 6e0d 0a09 7275 6e5f 7265  el:main...run_re
+000003f0: 6d6f 6465 6c5f 6261 636b 7570 3d68 6564  model_backup=hed
+00000400: 2e74 6f6f 6c73 2e72 656d 6f64 656c 696e  .tools.remodelin
+00000410: 672e 636c 692e 7275 6e5f 7265 6d6f 6465  g.cli.run_remode
+00000420: 6c5f 6261 636b 7570 3a6d 6169 6e0d 0a09  l_backup:main...
+00000430: 7275 6e5f 7265 6d6f 6465 6c5f 7265 7374  run_remodel_rest
+00000440: 6f72 653d 6865 642e 746f 6f6c 732e 7265  ore=hed.tools.re
+00000450: 6d6f 6465 6c69 6e67 2e63 6c69 2e72 756e  modeling.cli.run
+00000460: 5f72 656d 6f64 656c 5f72 6573 746f 7265  _remodel_restore
+00000470: 3a6d 6169 6e0d 0a0d 0a5b 7665 7273 696f  :main....[versio
+00000480: 6e65 6572 5d0d 0a56 4353 203d 2067 6974  neer]..VCS = git
+00000490: 0d0a 7374 796c 6520 3d20 7065 7034 3430  ..style = pep440
+000004a0: 0d0a 7665 7273 696f 6e66 696c 655f 736f  ..versionfile_so
+000004b0: 7572 6365 203d 2068 6564 2f5f 7665 7273  urce = hed/_vers
+000004c0: 696f 6e2e 7079 0d0a 7665 7273 696f 6e66  ion.py..versionf
+000004d0: 696c 655f 6275 696c 6420 3d20 6865 642f  ile_build = hed/
+000004e0: 5f76 6572 7369 6f6e 2e70 790d 0a74 6167  _version.py..tag
+000004f0: 5f70 7265 6669 7820 3d20 0d0a 7061 7265  _prefix = ..pare
+00000500: 6e74 6469 725f 7072 6566 6978 203d 2068  ntdir_prefix = h
+00000510: 6564 746f 6f6c 732d 0d0a 0d0a 5b65 6767  edtools-....[egg
+00000520: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000530: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000540: 2030 0d0a 0d0a                            0....
```

### Comparing `hedtools-0.2.0/versioneer.py` & `hedtools-0.3.0/versioneer.py`

 * *Files identical despite different names*

