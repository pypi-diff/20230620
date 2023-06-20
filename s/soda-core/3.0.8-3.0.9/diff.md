# Comparing `tmp/soda-core-3.0.8.tar.gz` & `tmp/soda-core-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soda-core-3.0.8.tar", last modified: Wed Sep 21 19:41:31 2022, max compression
+gzip compressed data, was "soda-core-3.0.9.tar", last modified: Tue Sep 27 20:19:41 2022, max compression
```

## Comparing `soda-core-3.0.8.tar` & `soda-core-3.0.9.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.491379 soda-core-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-09-21 19:41:31.491379 soda-core-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 19:41:31.491379 soda-core-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-09-21 19:41:14.000000 soda-core-3.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.471379 soda-core-3.0.8/soda/
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.471379 soda-core-3.0.8/soda/cli/
--rw-r--r--   0 runner    (1001) docker     (121)    16109 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.471379 soda-core-3.0.8/soda/cloud/
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/cloud/dbt_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.471379 soda-core-3.0.8/soda/common/
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/aws_credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/config_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/exception_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/file_system.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/jinja.py
--rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/json_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/lazy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/logs.py
--rw-r--r--   0 runner    (1001) docker     (121)     4408 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/random_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/undefined_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/common/yaml_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.471379 soda-core-3.0.8/soda/configuration/
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/configuration/configuration_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.475379 soda-core-3.0.8/soda/execution/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.475379 soda-core-3.0.8/soda/execution/check/
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/anomaly_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     5588 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/automated_monitoring_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/change_over_time_metric_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    12775 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/check.py
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/discover_tables_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/distribution_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     5807 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/freshness_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/metric_check.py
--rw-r--r--   0 runner    (1001) docker     (121)    20492 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/profile_columns_run.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/reference_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/row_count_comparison_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/sample_tables_run.py
--rw-r--r--   0 runner    (1001) docker     (121)    14744 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/schema_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/user_defined_failed_rows_check.py
--rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check/user_defined_failed_rows_expression_check.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/check_outcome.py
--rw-r--r--   0 runner    (1001) docker     (121)      692 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/column.py
--rw-r--r--   0 runner    (1001) docker     (121)    41471 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/data_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/data_source_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/data_source_scan.py
--rw-r--r--   0 runner    (1001) docker     (121)      662 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/data_type.py
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/derived_formula.py
--rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.479379 soda-core-3.0.8/soda/execution/metric/
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/column_metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/derived_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/metric.py
--rw-r--r--   0 runner    (1001) docker     (121)    11719 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/numeric_query_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)      727 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/query_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/reference_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/schema_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/user_defined_failed_rows_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/metric/user_defined_numeric_metric.py
--rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/partition.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.479379 soda-core-3.0.8/soda/execution/query/
--rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/aggregation_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/duplicates_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/partition_queries.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/reference_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/sample_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/schema_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/user_defined_failed_rows_expression_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/user_defined_failed_rows_query.py
--rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/query/user_defined_numeric_query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/schema_comparator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/table.py
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/execution/telemetry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.479379 soda-core-3.0.8/soda/model/
--rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/model/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.479379 soda-core-3.0.8/soda/profiling/
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/profiling/discover_table_result_table.py
--rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/profiling/discover_tables_result.py
--rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/profiling/discover_tables_result_column.py
--rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/profiling/profile_columns_result.py
--rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/profiling/sample_tables_result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.483379 soda-core-3.0.8/soda/sampler/
--rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/db_sample.py
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/default_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/log_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/sample.py
--rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/sample_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/sample_ref.py
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/sample_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/sampler_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sampler/soda_cloud_sampler.py
--rw-r--r--   0 runner    (1001) docker     (121)    39371 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/scan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.483379 soda-core-3.0.8/soda/soda_cloud/
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/soda_cloud/historic_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (121)    13002 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/soda_cloud/soda_cloud.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.487379 soda-core-3.0.8/soda/sodacl/
--rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/anomaly_metric_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.487379 soda-core-3.0.8/soda/sodacl/antlr/
--rw-r--r--   0 runner    (1001) docker     (121)    16162 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrLexer.py
--rw-r--r--   0 runner    (1001) docker     (121)    13970 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrListener.py
--rw-r--r--   0 runner    (1001) docker     (121)   114986 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrParser.py
--rw-r--r--   0 runner    (1001) docker     (121)     8316 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrVisitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      850 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/change_over_time_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/change_over_time_metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/column_checks_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/column_configurations_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/columnset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/data_source_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      965 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/data_source_scan_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/distribution_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/file_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/for_each_column_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/for_each_dataset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/format_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      981 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/freshness_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/location.py
--rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/metric_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/metric_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/missing_and_valid_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/name_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/partition_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/reference_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      773 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/row_count_comparison_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/schema_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/sodacl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)    74282 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/sodacl_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/table_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/tableset_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/threshold_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/user_defined_failed_rows_check_cfg.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.487379 soda-core-3.0.8/soda/telemetry/
--rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/telemetry/memory_span_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/telemetry/soda_exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/telemetry/soda_telemetry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-09-21 19:41:14.000000 soda-core-3.0.8/soda/telemetry/soda_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 19:41:31.487379 soda-core-3.0.8/soda_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-09-21 19:41:31.000000 soda-core-3.0.8/soda_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-09-21 19:41:31.000000 soda-core-3.0.8/soda_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 19:41:31.000000 soda-core-3.0.8/soda_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-21 19:41:31.000000 soda-core-3.0.8/soda_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-21 19:41:31.000000 soda-core-3.0.8/soda_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-21 19:41:31.000000 soda-core-3.0.8/soda_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.567824 soda-core-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-09-27 20:19:41.567824 soda-core-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-27 20:19:41.567824 soda-core-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1711 2022-09-27 20:19:27.000000 soda-core-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.555824 soda-core-3.0.9/soda/
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.555824 soda-core-3.0.9/soda/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)    16482 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.555824 soda-core-3.0.9/soda/cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)      339 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/cloud/dbt_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.555824 soda-core-3.0.9/soda/common/
+-rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/aws_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3847 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/config_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/exception_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1155 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2014 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/jinja.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3031 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/json_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3933 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/log.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/logs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4408 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/random_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/undefined_instance.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/common/yaml_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.555824 soda-core-3.0.9/soda/configuration/
+-rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4611 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/configuration/configuration_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.559824 soda-core-3.0.9/soda/execution/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.559824 soda-core-3.0.9/soda/execution/check/
+-rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/anomaly_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5588 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/automated_monitoring_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3129 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/change_over_time_metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13072 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/discover_tables_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6145 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/distribution_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5807 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/freshness_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6419 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/metric_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20492 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/profile_columns_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/reference_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3472 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/row_count_comparison_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1943 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/sample_tables_run.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14744 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/schema_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2171 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/user_defined_failed_rows_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3403 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check/user_defined_failed_rows_expression_check.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/check_outcome.py
+-rw-r--r--   0 runner    (1001) docker     (121)      692 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/column.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41645 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3575 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/data_source_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3626 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/data_source_scan.py
+-rw-r--r--   0 runner    (1001) docker     (121)      662 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/derived_formula.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4136 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.559824 soda-core-3.0.9/soda/execution/metric/
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/column_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5426 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/derived_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3684 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11747 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/numeric_query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/query_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1154 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/reference_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/schema_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1271 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/user_defined_failed_rows_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1124 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/metric/user_defined_numeric_metric.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4116 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/partition.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.559824 soda-core-3.0.9/soda/execution/query/
+-rw-r--r--   0 runner    (1001) docker     (121)     1658 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/aggregation_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1633 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/duplicates_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/partition_queries.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/reference_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/sample_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1398 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/schema_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/user_defined_failed_rows_expression_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)      863 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/user_defined_failed_rows_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)      705 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/query/user_defined_numeric_query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1923 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/schema_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/table.py
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/execution/telemetry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.559824 soda-core-3.0.9/soda/model/
+-rw-r--r--   0 runner    (1001) docker     (121)      153 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/model/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.563824 soda-core-3.0.9/soda/profiling/
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/profiling/discover_table_result_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/profiling/discover_tables_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)      561 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/profiling/discover_tables_result_column.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4189 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/profiling/profile_columns_result.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1245 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/profiling/sample_tables_result.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.563824 soda-core-3.0.9/soda/sampler/
+-rw-r--r--   0 runner    (1001) docker     (121)      709 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/db_sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)      730 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/default_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2522 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/log_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      284 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/sample.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1090 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/sample_context.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1959 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/sample_ref.py
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/sample_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/sampler_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1473 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sampler/soda_cloud_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39916 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/scan.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.563824 soda-core-3.0.9/soda/soda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/soda_cloud/historic_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13002 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/soda_cloud/soda_cloud.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.567824 soda-core-3.0.9/soda/sodacl/
+-rw-r--r--   0 runner    (1001) docker     (121)     1489 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/anomaly_metric_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.567824 soda-core-3.0.9/soda/sodacl/antlr/
+-rw-r--r--   0 runner    (1001) docker     (121)    16162 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrLexer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13970 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrListener.py
+-rw-r--r--   0 runner    (1001) docker     (121)   114986 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrParser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8316 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      850 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/change_over_time_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/change_over_time_metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/column_checks_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      310 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/column_configurations_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/columnset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1321 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/data_source_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      965 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/data_source_scan_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/distribution_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/file_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/for_each_column_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/for_each_dataset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/format_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      981 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/freshness_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      859 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)      232 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/metric_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2263 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/metric_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6431 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/missing_and_valid_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/name_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/partition_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/reference_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      773 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/row_count_comparison_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/schema_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/sodacl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74282 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/sodacl_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2136 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/table_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/tableset_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3416 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/threshold_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/user_defined_failed_rows_check_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (121)      665 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.567824 soda-core-3.0.9/soda/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (121)     1230 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/telemetry/memory_span_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1693 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/telemetry/soda_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5248 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/telemetry/soda_telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3139 2022-09-27 20:19:27.000000 soda-core-3.0.9/soda/telemetry/soda_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-27 20:19:41.567824 soda-core-3.0.9/soda_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-09-27 20:19:41.000000 soda-core-3.0.9/soda_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4550 2022-09-27 20:19:41.000000 soda-core-3.0.9/soda_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-27 20:19:41.000000 soda-core-3.0.9/soda_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       43 2022-09-27 20:19:41.000000 soda-core-3.0.9/soda_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2022-09-27 20:19:41.000000 soda-core-3.0.9/soda_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-09-27 20:19:41.000000 soda-core-3.0.9/soda_core.egg-info/top_level.txt
```

### Comparing `soda-core-3.0.8/PKG-INFO` & `soda-core-3.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-core
-Version: 3.0.8
+Version: 3.0.9
 Summary: Soda Core library & CLI
 Author: Soda Data N.V.
 Author-email: info@soda.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `soda-core-3.0.8/setup.py` & `soda-core-3.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 if sys.version_info < (3, 7):
     print("Error: Soda SQL requires at least Python 3.7")
     print("Error: Please upgrade your Python version to 3.7 or later")
     sys.exit(1)
 
 package_name = "soda-core"
 # Managed by tbump - do not change manually
-package_version = "3.0.8"
+package_version = "3.0.9"
 description = "Soda Core"
 
 # long_description = (pathlib.Path(__file__).parent.parent / "README.md").read_text()
 
 requires = [
     "markupsafe==2.0.1",
     "Jinja2~=2.11",  # Downgraded from 3.x until dbt-core 1.3 is released
```

### Comparing `soda-core-3.0.8/soda/cli/cli.py` & `soda-core-3.0.9/soda/cli/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,24 +73,32 @@
     "--data-timestamp",
     required=False,
     default=datetime.now(tz=timezone.utc).isoformat(timespec="seconds"),
     help="The scan time in ISO8601 format. Example: 2021-04-28T09:00:00+02:00",
     type=click.STRING,
 )
 @click.option("-V", "--verbose", is_flag=True)
+@click.option(
+    "-srf",
+    "--scan-results-file",
+    required=False,
+    default=None,
+    help="Specify the file path where the scan results as json will be stored",
+)
 @click.argument("sodacl_paths", nargs=-1, type=click.STRING)
 @soda_trace
 def scan(
     sodacl_paths: list[str],
     data_source: str,
     scan_definition: str | None,
     configuration: list[str],
     data_timestamp: str,
     variable: list[str],
     verbose: bool | None,
+    scan_results_file: Optional[str] = None,
 ):
     """
     The soda scan command:
 
       * parses the checks files and reports any errors
 
       * build and executes SQL queries for the checks
@@ -139,14 +147,15 @@
             "command_option": {
                 "sodacl_paths": len(sodacl_paths),
                 "variables": len(variable),
                 "configuration_paths": len(configuration),
                 "offline": False,  # TODO: change after offline mode is supported.
                 "non_interactive": False,  # TODO: change after non interactive mode is supported.
                 "verbose": verbose,
+                "scan_results_file": scan_results_file,
             },
         }
     )
 
     scan = Scan()
     scan._data_timestamp = datetime.fromisoformat(data_timestamp)
 
@@ -178,14 +187,17 @@
     else:
         scan._logs.warning("No checks file specified")
 
     if variable:
         variables_dict = dict([tuple(v.split("=")) for v in variable])
         scan.add_variables(variables_dict)
 
+    if isinstance(scan_results_file, str):
+        scan.set_scan_results_file(scan_results_file)
+
     sys.exit(scan.execute())
 
 
 @main.command(
     short_help="Updates contents of a distribution reference file",
 )
 @click.option(
```

### Comparing `soda-core-3.0.8/soda/common/aws_credentials.py` & `soda-core-3.0.9/soda/common/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/config_helper.py` & `soda-core-3.0.9/soda/common/config_helper.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/exceptions.py` & `soda-core-3.0.9/soda/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/file_system.py` & `soda-core-3.0.9/soda/common/file_system.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/jinja.py` & `soda-core-3.0.9/soda/common/jinja.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/json_helper.py` & `soda-core-3.0.9/soda/common/json_helper.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/log.py` & `soda-core-3.0.9/soda/common/log.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/logs.py` & `soda-core-3.0.9/soda/common/logs.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/parser.py` & `soda-core-3.0.9/soda/common/parser.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/common/yaml_helper.py` & `soda-core-3.0.9/soda/common/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/configuration/configuration.py` & `soda-core-3.0.9/soda/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/configuration/configuration_parser.py` & `soda-core-3.0.9/soda/configuration/configuration_parser.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/anomaly_metric_check.py` & `soda-core-3.0.9/soda/execution/check/anomaly_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/automated_monitoring_run.py` & `soda-core-3.0.9/soda/execution/check/automated_monitoring_run.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/change_over_time_metric_check.py` & `soda-core-3.0.9/soda/execution/check/change_over_time_metric_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/check.py` & `soda-core-3.0.9/soda/execution/check/check.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 import collections
+import os
 from abc import ABC, abstractmethod
 
 from soda.execution.check_outcome import CheckOutcome
 from soda.execution.column import Column
 from soda.execution.identity import ConsistentHashBuilder
 from soda.execution.metric.metric import Metric
 from soda.sampler.sample_ref import SampleRef
@@ -152,15 +153,15 @@
         from soda.common.yaml_helper import to_yaml_str
 
         if isinstance(check_cfg.source_configurations, dict):
             return to_yaml_str({check_cfg.source_header: [{check_cfg.source_line: check_cfg.source_configurations}]})
         else:
             return f"{check_cfg.source_header}:\n  {check_cfg.source_line}"
 
-    def create_identity(self, with_datasource: bool = False) -> str:
+    def create_identity(self, with_datasource: bool = False, with_filename: bool = False) -> str:
         check_cfg: CheckCfg = self.check_cfg
         from soda.common.yaml_helper import to_yaml_str
 
         if isinstance(check_cfg.source_configurations, dict):
             identity = check_cfg.source_configurations.get("identity")
             if isinstance(identity, str):
                 return identity
@@ -186,14 +187,17 @@
                 identity_source_configurations_yaml = to_yaml_str(identity_source_configurations)
                 hash_builder.add(identity_source_configurations_yaml)
         # Temp solution to introduce new variant of identity to help cloud identifying datasets with same name
         # See https://sodadata.atlassian.net/browse/CLOUD-1143
         if with_datasource:
             hash_builder.add(self.data_source_scan.data_source.data_source_name)
 
+        if with_filename:
+            hash_builder.add(os.path.basename(self.check_cfg.location.file_path))
+
         return hash_builder.get_hash()
 
     def add_outcome_reason(self, outcome_type: str, message: str, severity: str):
         self.force_send_results_to_cloud = True
         self.outcome_reasons.append({"code": outcome_type, "message": message, "severity": severity})  # error/warn/info
 
     @staticmethod
@@ -206,19 +210,20 @@
 
     def get_cloud_dict(self):
         from soda.execution.column import Column
         from soda.execution.partition import Partition
 
         cloud_dict = {
             # See https://sodadata.atlassian.net/browse/CLOUD-1143
-            "identity": self.create_identity(with_datasource=False),
+            "identity": self.create_identity(with_datasource=False, with_filename=False),
             "identities": {
                 # v1 is original without the datasource name and v2 is with datasource name in the hash
-                "v1": self.create_identity(with_datasource=False),
-                "v2": self.create_identity(with_datasource=True),
+                "v1": self.create_identity(with_datasource=False, with_filename=False),
+                "v2": self.create_identity(with_datasource=True, with_filename=False),
+                "v3": self.create_identity(with_datasource=True, with_filename=True),
             },
             "name": self.name,
             "type": self.cloud_check_type,
             "definition": self.create_definition(),
             "location": self.check_cfg.location.get_cloud_dict(),
             "dataSource": self.data_source_scan.data_source.data_source_name,
             "table": Partition.get_table_name(self.partition),
```

### Comparing `soda-core-3.0.8/soda/execution/check/discover_tables_run.py` & `soda-core-3.0.9/soda/execution/check/discover_tables_run.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/distribution_check.py` & `soda-core-3.0.9/soda/execution/check/distribution_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/freshness_check.py` & `soda-core-3.0.9/soda/execution/check/freshness_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/metric_check.py` & `soda-core-3.0.9/soda/execution/check/metric_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/profile_columns_run.py` & `soda-core-3.0.9/soda/execution/check/profile_columns_run.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/reference_check.py` & `soda-core-3.0.9/soda/execution/check/reference_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/row_count_comparison_check.py` & `soda-core-3.0.9/soda/execution/check/row_count_comparison_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/sample_tables_run.py` & `soda-core-3.0.9/soda/execution/check/sample_tables_run.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/schema_check.py` & `soda-core-3.0.9/soda/execution/check/schema_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/user_defined_failed_rows_check.py` & `soda-core-3.0.9/soda/execution/check/user_defined_failed_rows_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/check/user_defined_failed_rows_expression_check.py` & `soda-core-3.0.9/soda/execution/check/user_defined_failed_rows_expression_check.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/column.py` & `soda-core-3.0.9/soda/execution/column.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/data_source.py` & `soda-core-3.0.9/soda/execution/data_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -285,31 +285,37 @@
         """Column to be used as a 'database' equivalent."""
         return "table_catalog"
 
     ######################
     # Store Table Sample
     ######################
 
-    def store_table_sample(self, table_name: str, limit: int | None = None) -> SampleRef:
-        sql = self.sql_select_all(table_name=table_name, limit=limit)
+    def store_table_sample(self, table_name: str, limit: int | None = None, filter: str | None = None) -> SampleRef:
+        sql = self.sql_select_all(table_name=table_name, limit=limit, filter=filter)
         query = Query(
             data_source_scan=self.data_source_scan,
             unqualified_query_name=f"store-sample-for-{table_name}",
             sql=sql,
             sample_name="table_sample",
         )
         query.store()
         return query.sample_ref
 
-    def sql_select_all(self, table_name: str, limit: int | None = None) -> str:
+    def sql_select_all(self, table_name: str, limit: int | None = None, filter: str | None = None) -> str:
         qualified_table_name = self.qualified_table_name(table_name)
+
+        filter_sql = ""
+        if filter:
+            filter_sql = f" \n WHERE {filter}"
+
         limit_sql = ""
         if limit is not None:
             limit_sql = f" \n LIMIT {limit}"
-        sql = f"SELECT * FROM {qualified_table_name}{limit_sql}"
+
+        sql = f"SELECT * FROM {qualified_table_name}{filter_sql}{limit_sql}"
         return sql
 
     ############################################
     # For a table, get the columns metadata
     ############################################
 
     def get_table_columns(
```

### Comparing `soda-core-3.0.8/soda/execution/data_source_manager.py` & `soda-core-3.0.9/soda/execution/data_source_manager.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/data_source_scan.py` & `soda-core-3.0.9/soda/execution/data_source_scan.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/data_type.py` & `soda-core-3.0.9/soda/execution/data_type.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/derived_formula.py` & `soda-core-3.0.9/soda/execution/derived_formula.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/identity.py` & `soda-core-3.0.9/soda/execution/identity.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/column_metrics.py` & `soda-core-3.0.9/soda/execution/metric/column_metrics.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/derived_metric.py` & `soda-core-3.0.9/soda/execution/metric/derived_metric.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/metric.py` & `soda-core-3.0.9/soda/execution/metric/metric.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/numeric_query_metric.py` & `soda-core-3.0.9/soda/execution/metric/numeric_query_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
         return None
 
     def is_missing_or_validity_configured(self) -> bool:
         return self.missing_and_valid_cfg is not None
 
     metric_names_with_failed_rows = ["missing_count", "invalid_count"]
 
-    def create_failed_rows_sample_query(self) -> SampleQuery | None:
+    def create_failed_rows_sample_query(self, limit: int = 1000) -> SampleQuery | None:
         sampler = self.data_source_scan.scan._configuration.sampler
         if (
             sampler
             and self.name in self.metric_names_with_failed_rows
             and isinstance(self.value, Number)
             and self.value > 0
         ):
@@ -252,10 +252,10 @@
                 where_clauses.append(f"NOT {self.build_valid_condition()}")
 
             if self.filter:
                 where_clauses.append(self.filter)
 
             where_sql = " AND ".join(where_clauses)
 
-            sql = f"SELECT * \n" f"FROM {self.partition.table.qualified_table_name} \n" f"WHERE {where_sql}"
+            sql = self.data_source_scan.data_source.sql_select_all(self.partition.table.table_name, limit, where_sql)
 
             return SampleQuery(self.data_source_scan, self, "failed_rows", sql)
```

### Comparing `soda-core-3.0.8/soda/execution/metric/query_metric.py` & `soda-core-3.0.9/soda/execution/metric/query_metric.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,9 +22,9 @@
             partition=partition,
             column=column,
             name=name,
             check=check,
             identity_parts=identity_parts,
         )
 
-    def create_failed_rows_sample_query(self):
+    def create_failed_rows_sample_query(self, limit: int = 1000):
         return None
```

### Comparing `soda-core-3.0.8/soda/execution/metric/reference_metric.py` & `soda-core-3.0.9/soda/execution/metric/reference_metric.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/schema_metric.py` & `soda-core-3.0.9/soda/execution/metric/schema_metric.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/user_defined_failed_rows_metric.py` & `soda-core-3.0.9/soda/execution/metric/user_defined_failed_rows_metric.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/metric/user_defined_numeric_metric.py` & `soda-core-3.0.9/soda/execution/metric/user_defined_numeric_metric.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/partition.py` & `soda-core-3.0.9/soda/execution/partition.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/aggregation_query.py` & `soda-core-3.0.9/soda/execution/query/aggregation_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/duplicates_query.py` & `soda-core-3.0.9/soda/execution/query/duplicates_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/partition_queries.py` & `soda-core-3.0.9/soda/execution/query/partition_queries.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/query.py` & `soda-core-3.0.9/soda/execution/query/query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/reference_query.py` & `soda-core-3.0.9/soda/execution/query/reference_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/sample_query.py` & `soda-core-3.0.9/soda/execution/query/sample_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/schema_query.py` & `soda-core-3.0.9/soda/execution/query/schema_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/user_defined_failed_rows_expression_query.py` & `soda-core-3.0.9/soda/execution/query/user_defined_failed_rows_expression_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/user_defined_failed_rows_query.py` & `soda-core-3.0.9/soda/execution/query/user_defined_failed_rows_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/query/user_defined_numeric_query.py` & `soda-core-3.0.9/soda/execution/query/user_defined_numeric_query.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/schema_comparator.py` & `soda-core-3.0.9/soda/execution/schema_comparator.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/execution/table.py` & `soda-core-3.0.9/soda/execution/table.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/profiling/discover_table_result_table.py` & `soda-core-3.0.9/soda/profiling/discover_table_result_table.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/profiling/discover_tables_result.py` & `soda-core-3.0.9/soda/profiling/discover_tables_result.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/profiling/discover_tables_result_column.py` & `soda-core-3.0.9/soda/profiling/discover_tables_result_column.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/profiling/profile_columns_result.py` & `soda-core-3.0.9/soda/profiling/profile_columns_result.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/profiling/sample_tables_result.py` & `soda-core-3.0.9/soda/profiling/sample_tables_result.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/db_sample.py` & `soda-core-3.0.9/soda/sampler/db_sample.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/default_sampler.py` & `soda-core-3.0.9/soda/sampler/default_sampler.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/log_sampler.py` & `soda-core-3.0.9/soda/sampler/log_sampler.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/sample_context.py` & `soda-core-3.0.9/soda/sampler/sample_context.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/sample_ref.py` & `soda-core-3.0.9/soda/sampler/sample_ref.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/sample_schema.py` & `soda-core-3.0.9/soda/sampler/sample_schema.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sampler/soda_cloud_sampler.py` & `soda-core-3.0.9/soda/sampler/soda_cloud_sampler.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/scan.py` & `soda-core-3.0.9/soda/scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from soda.execution.metric.metric import Metric
 from soda.profiling.discover_table_result_table import DiscoverTablesResultTable
 from soda.profiling.profile_columns_result import ProfileColumnsResultTable
 from soda.profiling.sample_tables_result import SampleTablesResultTable
 from soda.sampler.default_sampler import DefaultSampler
 from soda.sampler.sampler import Sampler
 from soda.soda_cloud.historic_descriptor import HistoricDescriptor
+from soda.soda_cloud.soda_cloud import SodaCloud
 from soda.sodacl.location import Location
 from soda.sodacl.sodacl_cfg import SodaCLCfg
 from soda.telemetry.soda_telemetry import SodaTelemetry
 
 logger = logging.getLogger(__name__)
 verbose = False
 
@@ -40,14 +41,15 @@
         from soda.execution.query.query import Query
 
         # Using this instead of utcnow() as that creates tz naive object, this has explicitly utc set. More info https://docs.python.org/3/library/datetime.html#datetime.datetime.utcnow
         now = datetime.now(tz=timezone.utc)
         self.sampler: Sampler | None = None
         self._logs = Logs(logger)
         self._scan_definition_name: str | None = None
+        self._scan_results_file: str | None = None
         self._data_source_name: str | None = None
         self._variables: dict[str, object] = {"NOW": now.isoformat()}
         self._configuration: Configuration = Configuration(scan=self)
         self._sodacl_cfg: SodaCLCfg = SodaCLCfg(scan=self)
         self._file_paths: set[str] = set()
         self._data_timestamp: datetime = now
         self._scan_start_timestamp: datetime = now
@@ -114,14 +116,17 @@
         self._scan_definition_name = scan_definition_name
 
     def set_verbose(self, verbose_var: bool = True):
         self._logs.verbose = verbose_var
         global verbose
         verbose = verbose_var
 
+    def set_scan_results_file(self, set_scan_results_file: str):
+        self._scan_results_file = set_scan_results_file
+
     def add_configuration_yaml_file(self, file_path: str):
         """
         Adds configurations from a YAML file on the given path.
         :param str file_path: is a string file_path pointing to a configuration file.
                               ~ will be expanded to the user home dir.
         """
         try:
@@ -525,14 +530,19 @@
             except Exception as e:
                 exit_value = 3
                 self._logs.error(f"Error occurred while sending scan results to soda cloud.", exception=e)
 
             self._close()
             self.scan_results = self.build_scan_results()
 
+        if self._scan_results_file is not None:
+            logger.info(f"Saving scan results to {self._scan_results_file}")
+            with open(self._scan_results_file, "w") as f:
+                json.dump(SodaCloud.build_scan_results(self), f)
+
         # Telemetry data
         soda_telemetry.set_attributes(
             {
                 "scan_exit_code": exit_value,
                 "checks_count": len(self._checks),
                 "queries_count": len(self._queries),
                 "metrics_count": len(self._metrics),
@@ -736,14 +746,17 @@
         # Note: ordering here must be the same as in Jinja.OsContext.resolve_or_missing: First env vars, then scan vars
         if variable_name in os.environ:
             return os.environ[variable_name]
         elif variable_name in self._variables:
             return self._variables[variable_name]
         return default_value
 
+    def get_scan_results(self) -> dict:
+        return self.scan_results
+
     def get_logs_text(self) -> str | None:
         return self.__logs_to_text(self._logs.logs)
 
     def has_error_logs(self) -> bool:
         return any(log.level == LogLevel.ERROR for log in self._logs.logs)
 
     def get_error_logs(self) -> list[Log]:
```

### Comparing `soda-core-3.0.8/soda/soda_cloud/historic_descriptor.py` & `soda-core-3.0.9/soda/soda_cloud/historic_descriptor.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/soda_cloud/soda_cloud.py` & `soda-core-3.0.9/soda/soda_cloud/soda_cloud.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/anomaly_metric_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/anomaly_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrLexer.py` & `soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrLexer.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrListener.py` & `soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrListener.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrParser.py` & `soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrParser.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/antlr/SodaCLAntlrVisitor.py` & `soda-core-3.0.9/soda/sodacl/antlr/SodaCLAntlrVisitor.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/change_over_time_cfg.py` & `soda-core-3.0.9/soda/sodacl/change_over_time_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/change_over_time_metric_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/change_over_time_metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/check_cfg.py` & `soda-core-3.0.9/soda/sodacl/check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/data_source_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/data_source_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/data_source_scan_cfg.py` & `soda-core-3.0.9/soda/sodacl/data_source_scan_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/distribution_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/distribution_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/format_cfg.py` & `soda-core-3.0.9/soda/sodacl/format_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/freshness_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/freshness_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/location.py` & `soda-core-3.0.9/soda/sodacl/location.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/metric_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/metric_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/missing_and_valid_cfg.py` & `soda-core-3.0.9/soda/sodacl/missing_and_valid_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/partition_cfg.py` & `soda-core-3.0.9/soda/sodacl/partition_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/reference_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/reference_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/row_count_comparison_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/row_count_comparison_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/schema_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/schema_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/sodacl_cfg.py` & `soda-core-3.0.9/soda/sodacl/sodacl_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/sodacl_parser.py` & `soda-core-3.0.9/soda/sodacl/sodacl_parser.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/table_cfg.py` & `soda-core-3.0.9/soda/sodacl/table_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/threshold_cfg.py` & `soda-core-3.0.9/soda/sodacl/threshold_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/user_defined_failed_rows_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/user_defined_failed_rows_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py` & `soda-core-3.0.9/soda/sodacl/user_defined_failed_rows_expression_check_cfg.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/telemetry/memory_span_exporter.py` & `soda-core-3.0.9/soda/telemetry/memory_span_exporter.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/telemetry/soda_exporter.py` & `soda-core-3.0.9/soda/telemetry/soda_exporter.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/telemetry/soda_telemetry.py` & `soda-core-3.0.9/soda/telemetry/soda_telemetry.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda/telemetry/soda_tracer.py` & `soda-core-3.0.9/soda/telemetry/soda_tracer.py`

 * *Files identical despite different names*

### Comparing `soda-core-3.0.8/soda_core.egg-info/PKG-INFO` & `soda-core-3.0.9/soda_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soda-core
-Version: 3.0.8
+Version: 3.0.9
 Summary: Soda Core library & CLI
 Author: Soda Data N.V.
 Author-email: info@soda.io
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `soda-core-3.0.8/soda_core.egg-info/SOURCES.txt` & `soda-core-3.0.9/soda_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

