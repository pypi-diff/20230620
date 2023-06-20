# Comparing `tmp/timeplus-1.2.1.tar.gz` & `tmp/timeplus-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timeplus-1.2.1.tar", last modified: Wed Jun  7 00:11:38 2023, max compression
+gzip compressed data, was "timeplus-1.2.2.tar", last modified: Tue Jun 20 17:24:07 2023, max compression
```

## Comparing `timeplus-1.2.1.tar` & `timeplus-1.2.2.tar`

### file list

```diff
@@ -1,174 +1,174 @@
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.100458 timeplus-1.2.1/
--rw-r--r--   0 gangtao    (502) staff       (20)     3921 2023-06-07 00:11:38.100624 timeplus-1.2.1/PKG-INFO
--rw-r--r--   0 gangtao    (502) staff       (20)     3479 2022-12-29 18:08:58.000000 timeplus-1.2.1/README.md
--rw-r--r--   0 gangtao    (502) staff       (20)      633 2023-06-07 00:11:38.101254 timeplus-1.2.1/setup.cfg
--rw-r--r--   0 gangtao    (502) staff       (20)     1247 2022-12-29 18:08:58.000000 timeplus-1.2.1/setup.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:37.970289 timeplus-1.2.1/swagger_client/
--rw-r--r--   0 gangtao    (502) staff       (20)     5204 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)    25043 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/api_client.py
--rw-r--r--   0 gangtao    (502) staff       (20)     8229 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/configuration.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.009478 timeplus-1.2.1/swagger_client/models/
--rw-r--r--   0 gangtao    (502) staff       (20)     4099 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3010 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/analyze_sql_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6294 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/api_key.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3907 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/batching_policy.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3495 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/column.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6897 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/column_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4844 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/columns_resp.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5165 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_api_key_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7665 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_api_key_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6083 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/create_query_request_v1_beta2.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/create_sink_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6899 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/create_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6447 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/create_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     8467 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/dashboard_dashboard.py
--rw-r--r--   0 gangtao    (502) staff       (20)     7960 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/dashboard_panel.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3551 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3639 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/error_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2623 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/event.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3056 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/event_infer_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4271 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/event_infer_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5147 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/external_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3038 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/file_upload_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3018 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/format_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3026 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/format_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5084 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/global_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3565 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/graph.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3666 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/ingest_data.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3880 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/metrics_query_throughput.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5334 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/node.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3443 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/owner.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15636 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3739 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3606 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4921 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4199 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_pipeline_node_metric.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3752 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/query_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5782 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/resource_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)    10676 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/sink.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3879 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/sink_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)    12051 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/source.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5811 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/source_preview_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3189 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/source_upload_body.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5737 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/sql_analyze_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11019 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/sql_analyze_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)    13632 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15463 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3102 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/stream_match_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3579 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/stream_setting.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6394 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/stream_stats.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4794 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/time_columns.py
--rw-r--r--   0 gangtao    (502) staff       (20)    15879 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_client/models/udf.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3555 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/udf_argument.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3771 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/udf_auth_context.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/models/update_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     5961 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/update_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6279 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/update_stream_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     6856 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/update_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11854 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/models/view.py
--rw-r--r--   0 gangtao    (502) staff       (20)    12995 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/rest.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.018298 timeplus-1.2.1/swagger_client/timeplus/
--rw-r--r--   0 gangtao    (502) staff       (20)     1040 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4723 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/alerts_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4385 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/alerts_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    11402 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/api_keys_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    19476 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/dashboards_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     9044 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/metrics_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    31463 2023-06-07 00:11:27.000000 timeplus-1.2.1/swagger_client/timeplus/queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4703 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/sinks_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    18309 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/sinks_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    42086 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/sources_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    33693 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/streams_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     3866 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_client/timeplus/topology_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    18450 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/udfs_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)    22977 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_client/timeplus/views_v1beta2_api.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.090202 timeplus-1.2.1/swagger_test/
--rw-r--r--   0 gangtao    (502) staff       (20)       15 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)      920 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_alerts_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      872 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_alerts_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_analyze_sql_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      842 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_api_key.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1215 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_api_keys_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_test/test_batching_policy.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_column_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_columns_resp.py
--rw-r--r--   0 gangtao    (502) staff       (20)      950 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_api_key_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      958 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_api_key_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_query_request_v1_beta2.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_sink_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_create_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_create_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      938 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_dashboard_dashboard.py
--rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_dashboard_panel.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1547 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_dashboards_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_error_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_event.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_event_infer_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_event_infer_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_external_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_file_upload_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_format_query_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_format_query_response.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_global_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_graph.py
--rw-r--r--   0 gangtao    (502) staff       (20)      874 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_ingest_data.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_metrics_query_throughput.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1058 2023-02-14 06:04:34.000000 timeplus-1.2.1/swagger_test/test_metrics_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_owner.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2014 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_queries_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline_edge.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline_node.py
--rw-r--r--   0 gangtao    (502) staff       (20)      982 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_pipeline_node_metric.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_query_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      964 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_resource_metrics_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sink.py
--rw-r--r--   0 gangtao    (502) staff       (20)      858 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sink_stat.py
--rw-r--r--   0 gangtao    (502) staff       (20)      911 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_sinks_internal_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1456 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_sinks_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_source.py
--rw-r--r--   0 gangtao    (502) staff       (20)      956 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_source_preview_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_source_upload_body.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2519 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_sources_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sql_analyze_column.py
--rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_sql_analyze_result.py
--rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_def.py
--rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_match_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_setting.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_stream_stats.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2036 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_streams_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_time_columns.py
--rw-r--r--   0 gangtao    (502) staff       (20)      873 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_topology_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      816 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_udf.py
--rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_udf_argument.py
--rw-r--r--   0 gangtao    (502) staff       (20)      908 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_udf_auth_context.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1438 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_udfs_v1beta2_api.py
--rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_dashboard_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_source_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_stream_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_update_view_request.py
--rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.1/swagger_test/test_view.py
--rw-r--r--   0 gangtao    (502) staff       (20)     1636 2023-06-06 23:40:05.000000 timeplus-1.2.1/swagger_test/test_views_v1beta2_api.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.097105 timeplus-1.2.1/test/
--rw-r--r--   0 gangtao    (502) staff       (20)      624 2022-12-29 02:29:17.000000 timeplus-1.2.1/test/test_stream.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.096633 timeplus-1.2.1/timeplus/
--rw-r--r--   0 gangtao    (502) staff       (20)      240 2022-12-29 02:29:17.000000 timeplus-1.2.1/timeplus/__init__.py
--rw-r--r--   0 gangtao    (502) staff       (20)      931 2023-06-06 23:40:05.000000 timeplus-1.2.1/timeplus/env.py
--rw-r--r--   0 gangtao    (502) staff       (20)      423 2022-12-29 02:29:17.000000 timeplus-1.2.1/timeplus/error.py
--rw-r--r--   0 gangtao    (502) staff       (20)     2912 2023-06-06 23:40:05.000000 timeplus-1.2.1/timeplus/query.py
--rw-r--r--   0 gangtao    (502) staff       (20)     4847 2023-06-06 23:40:05.000000 timeplus-1.2.1/timeplus/stream.py
--rw-r--r--   0 gangtao    (502) staff       (20)      527 2022-12-28 18:52:21.000000 timeplus-1.2.1/timeplus/type.py
--rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-07 00:11:31.000000 timeplus-1.2.1/timeplus/version.py
-drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-07 00:11:38.100043 timeplus-1.2.1/timeplus.egg-info/
--rw-r--r--   0 gangtao    (502) staff       (20)     3921 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/PKG-INFO
--rw-r--r--   0 gangtao    (502) staff       (20)     6532 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/SOURCES.txt
--rw-r--r--   0 gangtao    (502) staff       (20)        1 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/dependency_links.txt
--rw-r--r--   0 gangtao    (502) staff       (20)       82 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/requires.txt
--rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-07 00:11:37.000000 timeplus-1.2.1/timeplus.egg-info/top_level.txt
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.404733 timeplus-1.2.2/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4897 2023-06-20 17:24:07.405014 timeplus-1.2.2/PKG-INFO
+-rw-r--r--   0 gangtao    (502) staff       (20)     4455 2023-06-20 17:23:51.000000 timeplus-1.2.2/README.md
+-rw-r--r--   0 gangtao    (502) staff       (20)      633 2023-06-20 17:24:07.405827 timeplus-1.2.2/setup.cfg
+-rw-r--r--   0 gangtao    (502) staff       (20)     1247 2022-12-29 18:08:58.000000 timeplus-1.2.2/setup.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.247833 timeplus-1.2.2/swagger_client/
+-rw-r--r--   0 gangtao    (502) staff       (20)     5204 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    25043 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/api_client.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     8229 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_client/configuration.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.316967 timeplus-1.2.2/swagger_client/models/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4099 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3010 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/analyze_sql_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6294 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/api_key.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3907 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_client/models/batching_policy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3495 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6897 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/column_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4844 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/columns_resp.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5165 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/create_api_key_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7665 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/create_api_key_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/create_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6083 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_client/models/create_query_request_v1_beta2.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5948 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/create_sink_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6899 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/create_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6447 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/create_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     8467 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/dashboard_dashboard.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     7960 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/dashboard_panel.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3551 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3639 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/error_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2623 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/event.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3056 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/event_infer_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4271 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/event_infer_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5147 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/external_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3038 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/file_upload_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3018 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/format_query_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3026 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/format_query_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5084 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/global_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3565 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/graph.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3666 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/ingest_data.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3880 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/metrics_query_throughput.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5334 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3443 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/owner.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15636 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3739 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/query_pipeline.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3606 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/query_pipeline_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4921 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/query_pipeline_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4199 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/query_pipeline_node_metric.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3752 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/query_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5782 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/resource_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    10676 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/sink.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3879 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/sink_stat.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    12051 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/source.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5811 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/source_preview_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3189 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/source_upload_body.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5737 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/sql_analyze_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11019 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/sql_analyze_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    13632 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15463 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3102 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/stream_match_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3579 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/stream_setting.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6394 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/stream_stats.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4794 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_client/models/time_columns.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    15879 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_client/models/udf.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3555 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/udf_argument.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3771 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/udf_auth_context.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4618 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/models/update_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     5961 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/update_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6279 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/update_stream_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     6856 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/update_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11854 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/models/view.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    12995 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/rest.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.328695 timeplus-1.2.2/swagger_client/timeplus/
+-rw-r--r--   0 gangtao    (502) staff       (20)     1040 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4723 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/alerts_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4385 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/alerts_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    11402 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/api_keys_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    19476 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/dashboards_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     9044 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/metrics_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    31463 2023-06-07 00:11:27.000000 timeplus-1.2.2/swagger_client/timeplus/queries_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4703 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/sinks_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    18309 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/sinks_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    42086 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/sources_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    33693 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/streams_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3866 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_client/timeplus/topology_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    18450 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/udfs_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)    22977 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_client/timeplus/views_v1beta2_api.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.390483 timeplus-1.2.2/swagger_test/
+-rw-r--r--   0 gangtao    (502) staff       (20)       15 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      920 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_alerts_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      872 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_alerts_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_analyze_sql_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      842 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_api_key.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1215 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_api_keys_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_test/test_batching_policy.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_column_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_columns_resp.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      950 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_create_api_key_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      958 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_create_api_key_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_create_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1000 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_create_query_request_v1_beta2.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_create_sink_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_create_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_create_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      938 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_dashboard_dashboard.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      906 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_dashboard_panel.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1547 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_dashboards_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_error_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_event.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_event_infer_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_event_infer_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_external_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_file_upload_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_format_query_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_format_query_response.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_global_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_graph.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      874 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_ingest_data.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_metrics_query_throughput.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1058 2023-02-14 06:04:34.000000 timeplus-1.2.2/swagger_test/test_metrics_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_owner.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2014 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_queries_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      832 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_query_pipeline.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_query_pipeline_edge.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_query_pipeline_node.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      982 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_query_pipeline_node_metric.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_query_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      964 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_resource_metrics_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_sink.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      858 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_sink_stat.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      911 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_sinks_internal_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1456 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_sinks_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_source.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      956 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_source_preview_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_source_upload_body.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2519 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_sources_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_sql_analyze_column.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      924 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_sql_analyze_result.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      840 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      866 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_stream_def.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      940 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_stream_match_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      898 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_stream_setting.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_stream_stats.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     2036 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_streams_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_time_columns.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      873 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_topology_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      816 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_udf.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      882 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_udf_argument.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      908 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_udf_auth_context.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1438 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_udfs_v1beta2_api.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      972 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_update_dashboard_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_update_source_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      948 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_update_stream_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      932 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_update_view_request.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      824 2023-02-14 03:56:15.000000 timeplus-1.2.2/swagger_test/test_view.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     1636 2023-06-06 23:40:05.000000 timeplus-1.2.2/swagger_test/test_views_v1beta2_api.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.399776 timeplus-1.2.2/test/
+-rw-r--r--   0 gangtao    (502) staff       (20)      624 2022-12-29 02:29:17.000000 timeplus-1.2.2/test/test_stream.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.398857 timeplus-1.2.2/timeplus/
+-rw-r--r--   0 gangtao    (502) staff       (20)      240 2022-12-29 02:29:17.000000 timeplus-1.2.2/timeplus/__init__.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      931 2023-06-06 23:40:05.000000 timeplus-1.2.2/timeplus/env.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      423 2022-12-29 02:29:17.000000 timeplus-1.2.2/timeplus/error.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     3233 2023-06-20 17:23:51.000000 timeplus-1.2.2/timeplus/query.py
+-rw-r--r--   0 gangtao    (502) staff       (20)     4847 2023-06-06 23:40:05.000000 timeplus-1.2.2/timeplus/stream.py
+-rw-r--r--   0 gangtao    (502) staff       (20)      527 2022-12-28 18:52:21.000000 timeplus-1.2.2/timeplus/type.py
+-rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-20 17:23:58.000000 timeplus-1.2.2/timeplus/version.py
+drwxr-xr-x   0 gangtao    (502) staff       (20)        0 2023-06-20 17:24:07.404203 timeplus-1.2.2/timeplus.egg-info/
+-rw-r--r--   0 gangtao    (502) staff       (20)     4897 2023-06-20 17:24:07.000000 timeplus-1.2.2/timeplus.egg-info/PKG-INFO
+-rw-r--r--   0 gangtao    (502) staff       (20)     6532 2023-06-20 17:24:07.000000 timeplus-1.2.2/timeplus.egg-info/SOURCES.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)        1 2023-06-20 17:24:07.000000 timeplus-1.2.2/timeplus.egg-info/dependency_links.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)       82 2023-06-20 17:24:07.000000 timeplus-1.2.2/timeplus.egg-info/requires.txt
+-rw-r--r--   0 gangtao    (502) staff       (20)       37 2023-06-20 17:24:07.000000 timeplus-1.2.2/timeplus.egg-info/top_level.txt
```

### Comparing `timeplus-1.2.1/PKG-INFO` & `timeplus-1.2.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: timeplus
-Version: 1.2.1
-Summary: Timeplus python SDK
-Home-page: https://github.com/timeplus-io/gluon/tree/develop/python
-Author: Gang Tao
-Author-email: gang@timeplus.io
-Project-URL: Bug Tracker, https://github.com/timeplus-io/gluon/issues
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-
 # timeplus-client
 
 Welcome to the Timeplus HTTP REST API specification.
 
 # query
 
 ```python
@@ -23,40 +10,61 @@
 import json
 from pprint import pprint
 
 from timeplus import Query, Environment
 
 api_key = os.environ.get("TIMEPLUS_API_KEY")
 api_address = os.environ.get("TIMEPLUS_HOST")
-worksapce = os.environ.get("TIMEPLUS_WORKSAPCE")
+workspace = os.environ.get("TIMEPLUS_WORKSPACE")
 
 # Configure API key and address
-env = Environment().address(api_address).apikey(api_key).workspace(worksapce)
+env = Environment().address(api_address).workspace(workspace).apikey(api_key)
 
 try:
     # list all qeuries
     query_list = Query(env=env).list()
     pprint(f"there are {len(query_list)} queries ")
 
     # create a new query
-    query = Query(env=env).sql(query="SELECT * FROM iot").create()
-    query_id = query.metadata()["id"]
-    pprint(f"created a query with id {query_id}")
-
-    # get a query by id
-    get_query = Query(env=env).get(id=query_id)
-    metadata = query.metadata()
-    pprint(f"get a query with id {metadata['id']}")
+    query = (
+        Query(env=env).sql(query="SELECT * FROM car_live_data")
+        # .batching_policy(1000, 1000)
+        .create()
+    )
+
+    pprint(f"query with metadata {json.dumps(query.metadata())}")
+
+    # query header is the colume definitions of query result table
+    # it is a list of name/value pair
+    # for example : [{'name': 'in_use', 'type': 'bool'}, {'name': 'speed', 'type': 'float32'}]
+    query_header = query.header()
+    pprint(f"query with header {query.header()}")
 
     # iterate query result
     limit = 3
     count = 0
+
+    # query.result() is an iterator which will pull all the query result in small batches
+    # the iterator will continously pulling query result
+    # for streaming query, the iterator will not end until user cancel the query
     for event in query.result():
-        print(event.event)
-        print(json.loads(event.data))
+        # metric event return result time query metrics
+        # a sample metrics event:
+        # {'count': 117, 'eps': 75, 'processing_time': 1560,
+        # 'last_event_time': 1686237113265, 'response_time': 861,
+        # 'scanned_rows': 117, 'scanned_bytes': 7605}
+        if event.event == "metrics":
+            pprint(json.loads(event.data))
+
+        # message event contains query result which is an array of arrays
+        # representing multiple query result rows
+        # a sample message event:
+        # [[True,-73.857],[False, 84.1]]
+        if event.event == "message":
+            pprint(json.loads(event.data))
         count += 1
         if count >= limit:
             break
 
     query.cancel()
     query.delete()
```

### Comparing `timeplus-1.2.1/setup.cfg` & `timeplus-1.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/setup.py` & `timeplus-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/__init__.py` & `timeplus-1.2.2/swagger_client/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/api_client.py` & `timeplus-1.2.2/swagger_client/api_client.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/configuration.py` & `timeplus-1.2.2/swagger_client/configuration.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/__init__.py` & `timeplus-1.2.2/swagger_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/analyze_sql_request.py` & `timeplus-1.2.2/swagger_client/models/analyze_sql_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/api_key.py` & `timeplus-1.2.2/swagger_client/models/api_key.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/batching_policy.py` & `timeplus-1.2.2/swagger_client/models/batching_policy.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/column.py` & `timeplus-1.2.2/swagger_client/models/column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/column_def.py` & `timeplus-1.2.2/swagger_client/models/column_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/columns_resp.py` & `timeplus-1.2.2/swagger_client/models/columns_resp.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_api_key_request.py` & `timeplus-1.2.2/swagger_client/models/create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_api_key_response.py` & `timeplus-1.2.2/swagger_client/models/create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_dashboard_request.py` & `timeplus-1.2.2/swagger_client/models/create_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_query_request_v1_beta2.py` & `timeplus-1.2.2/swagger_client/models/create_query_request_v1_beta2.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_sink_request.py` & `timeplus-1.2.2/swagger_client/models/create_sink_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_source_request.py` & `timeplus-1.2.2/swagger_client/models/create_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/create_view_request.py` & `timeplus-1.2.2/swagger_client/models/create_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/dashboard_dashboard.py` & `timeplus-1.2.2/swagger_client/models/dashboard_dashboard.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/dashboard_panel.py` & `timeplus-1.2.2/swagger_client/models/dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/edge.py` & `timeplus-1.2.2/swagger_client/models/edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/error_response.py` & `timeplus-1.2.2/swagger_client/models/error_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/event.py` & `timeplus-1.2.2/swagger_client/models/event.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/event_infer_request.py` & `timeplus-1.2.2/swagger_client/models/event_infer_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/event_infer_response.py` & `timeplus-1.2.2/swagger_client/models/event_infer_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/external_stream_def.py` & `timeplus-1.2.2/swagger_client/models/external_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/file_upload_response.py` & `timeplus-1.2.2/swagger_client/models/file_upload_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/format_query_request.py` & `timeplus-1.2.2/swagger_client/models/format_query_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/format_query_response.py` & `timeplus-1.2.2/swagger_client/models/format_query_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/global_metrics_result.py` & `timeplus-1.2.2/swagger_client/models/global_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/graph.py` & `timeplus-1.2.2/swagger_client/models/graph.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/ingest_data.py` & `timeplus-1.2.2/swagger_client/models/ingest_data.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/metrics_query_throughput.py` & `timeplus-1.2.2/swagger_client/models/metrics_query_throughput.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/node.py` & `timeplus-1.2.2/swagger_client/models/node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/owner.py` & `timeplus-1.2.2/swagger_client/models/owner.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/query.py` & `timeplus-1.2.2/swagger_client/models/query.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/query_pipeline.py` & `timeplus-1.2.2/swagger_client/models/query_pipeline.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/query_pipeline_edge.py` & `timeplus-1.2.2/swagger_client/models/query_pipeline_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/query_pipeline_node.py` & `timeplus-1.2.2/swagger_client/models/query_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/query_pipeline_node_metric.py` & `timeplus-1.2.2/swagger_client/models/query_pipeline_node_metric.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/query_result.py` & `timeplus-1.2.2/swagger_client/models/query_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/resource_metrics_result.py` & `timeplus-1.2.2/swagger_client/models/resource_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/sink.py` & `timeplus-1.2.2/swagger_client/models/sink.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/sink_stat.py` & `timeplus-1.2.2/swagger_client/models/sink_stat.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/source.py` & `timeplus-1.2.2/swagger_client/models/source.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/source_preview_request.py` & `timeplus-1.2.2/swagger_client/models/source_preview_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/source_upload_body.py` & `timeplus-1.2.2/swagger_client/models/source_upload_body.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/sql_analyze_column.py` & `timeplus-1.2.2/swagger_client/models/sql_analyze_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/sql_analyze_result.py` & `timeplus-1.2.2/swagger_client/models/sql_analyze_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/stream.py` & `timeplus-1.2.2/swagger_client/models/stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/stream_def.py` & `timeplus-1.2.2/swagger_client/models/stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/stream_match_request.py` & `timeplus-1.2.2/swagger_client/models/stream_match_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/stream_setting.py` & `timeplus-1.2.2/swagger_client/models/stream_setting.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/stream_stats.py` & `timeplus-1.2.2/swagger_client/models/stream_stats.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/time_columns.py` & `timeplus-1.2.2/swagger_client/models/time_columns.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/udf.py` & `timeplus-1.2.2/swagger_client/models/udf.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/udf_argument.py` & `timeplus-1.2.2/swagger_client/models/udf_argument.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/udf_auth_context.py` & `timeplus-1.2.2/swagger_client/models/udf_auth_context.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/update_dashboard_request.py` & `timeplus-1.2.2/swagger_client/models/update_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/update_source_request.py` & `timeplus-1.2.2/swagger_client/models/update_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/update_stream_request.py` & `timeplus-1.2.2/swagger_client/models/update_stream_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/update_view_request.py` & `timeplus-1.2.2/swagger_client/models/update_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/models/view.py` & `timeplus-1.2.2/swagger_client/models/view.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/rest.py` & `timeplus-1.2.2/swagger_client/rest.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/__init__.py` & `timeplus-1.2.2/swagger_client/timeplus/__init__.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/alerts_internal_api.py` & `timeplus-1.2.2/swagger_client/timeplus/alerts_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/alerts_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/alerts_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/api_keys_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/api_keys_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/dashboards_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/dashboards_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/metrics_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/metrics_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/queries_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/queries_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/sinks_internal_api.py` & `timeplus-1.2.2/swagger_client/timeplus/sinks_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/sinks_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/sinks_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/sources_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/sources_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/streams_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/streams_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/topology_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/topology_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/udfs_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/udfs_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_client/timeplus/views_v1beta2_api.py` & `timeplus-1.2.2/swagger_client/timeplus/views_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_alerts_internal_api.py` & `timeplus-1.2.2/swagger_test/test_alerts_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_alerts_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_alerts_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_analyze_sql_request.py` & `timeplus-1.2.2/swagger_test/test_analyze_sql_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_api_key.py` & `timeplus-1.2.2/swagger_test/test_api_key.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_api_keys_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_api_keys_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_batching_policy.py` & `timeplus-1.2.2/swagger_test/test_batching_policy.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_column.py` & `timeplus-1.2.2/swagger_test/test_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_column_def.py` & `timeplus-1.2.2/swagger_test/test_column_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_columns_resp.py` & `timeplus-1.2.2/swagger_test/test_columns_resp.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_api_key_request.py` & `timeplus-1.2.2/swagger_test/test_create_api_key_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_api_key_response.py` & `timeplus-1.2.2/swagger_test/test_create_api_key_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_dashboard_request.py` & `timeplus-1.2.2/swagger_test/test_create_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_query_request_v1_beta2.py` & `timeplus-1.2.2/swagger_test/test_create_query_request_v1_beta2.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_sink_request.py` & `timeplus-1.2.2/swagger_test/test_create_sink_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_source_request.py` & `timeplus-1.2.2/swagger_test/test_create_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_create_view_request.py` & `timeplus-1.2.2/swagger_test/test_create_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_dashboard_dashboard.py` & `timeplus-1.2.2/swagger_test/test_dashboard_dashboard.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_dashboard_panel.py` & `timeplus-1.2.2/swagger_test/test_dashboard_panel.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_dashboards_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_dashboards_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_edge.py` & `timeplus-1.2.2/swagger_test/test_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_error_response.py` & `timeplus-1.2.2/swagger_test/test_error_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_event.py` & `timeplus-1.2.2/swagger_test/test_event.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_event_infer_request.py` & `timeplus-1.2.2/swagger_test/test_event_infer_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_event_infer_response.py` & `timeplus-1.2.2/swagger_test/test_event_infer_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_external_stream_def.py` & `timeplus-1.2.2/swagger_test/test_external_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_file_upload_response.py` & `timeplus-1.2.2/swagger_test/test_file_upload_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_format_query_request.py` & `timeplus-1.2.2/swagger_test/test_format_query_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_format_query_response.py` & `timeplus-1.2.2/swagger_test/test_format_query_response.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_global_metrics_result.py` & `timeplus-1.2.2/swagger_test/test_global_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_graph.py` & `timeplus-1.2.2/swagger_test/test_graph.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_ingest_data.py` & `timeplus-1.2.2/swagger_test/test_ingest_data.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_metrics_query_throughput.py` & `timeplus-1.2.2/swagger_test/test_metrics_query_throughput.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_metrics_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_metrics_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_node.py` & `timeplus-1.2.2/swagger_test/test_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_owner.py` & `timeplus-1.2.2/swagger_test/test_owner.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_queries_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_queries_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_query.py` & `timeplus-1.2.2/swagger_test/test_query.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_query_pipeline.py` & `timeplus-1.2.2/swagger_test/test_query_pipeline.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_query_pipeline_edge.py` & `timeplus-1.2.2/swagger_test/test_query_pipeline_edge.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_query_pipeline_node.py` & `timeplus-1.2.2/swagger_test/test_query_pipeline_node.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_query_pipeline_node_metric.py` & `timeplus-1.2.2/swagger_test/test_query_pipeline_node_metric.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_query_result.py` & `timeplus-1.2.2/swagger_test/test_query_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_resource_metrics_result.py` & `timeplus-1.2.2/swagger_test/test_resource_metrics_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sink.py` & `timeplus-1.2.2/swagger_test/test_sink.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sink_stat.py` & `timeplus-1.2.2/swagger_test/test_sink_stat.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sinks_internal_api.py` & `timeplus-1.2.2/swagger_test/test_sinks_internal_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sinks_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_sinks_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_source.py` & `timeplus-1.2.2/swagger_test/test_source.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_source_preview_request.py` & `timeplus-1.2.2/swagger_test/test_source_preview_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_source_upload_body.py` & `timeplus-1.2.2/swagger_test/test_source_upload_body.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sources_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_sources_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sql_analyze_column.py` & `timeplus-1.2.2/swagger_test/test_sql_analyze_column.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_sql_analyze_result.py` & `timeplus-1.2.2/swagger_test/test_sql_analyze_result.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_stream.py` & `timeplus-1.2.2/swagger_test/test_stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_stream_def.py` & `timeplus-1.2.2/swagger_test/test_stream_def.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_stream_match_request.py` & `timeplus-1.2.2/swagger_test/test_stream_match_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_stream_setting.py` & `timeplus-1.2.2/swagger_test/test_stream_setting.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_stream_stats.py` & `timeplus-1.2.2/swagger_test/test_stream_stats.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_streams_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_streams_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_time_columns.py` & `timeplus-1.2.2/swagger_test/test_time_columns.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_topology_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_topology_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_udf.py` & `timeplus-1.2.2/swagger_test/test_udf.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_udf_argument.py` & `timeplus-1.2.2/swagger_test/test_udf_argument.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_udf_auth_context.py` & `timeplus-1.2.2/swagger_test/test_udf_auth_context.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_udfs_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_udfs_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_update_dashboard_request.py` & `timeplus-1.2.2/swagger_test/test_update_dashboard_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_update_source_request.py` & `timeplus-1.2.2/swagger_test/test_update_source_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_update_stream_request.py` & `timeplus-1.2.2/swagger_test/test_update_stream_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_update_view_request.py` & `timeplus-1.2.2/swagger_test/test_update_view_request.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_view.py` & `timeplus-1.2.2/swagger_test/test_view.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/swagger_test/test_views_v1beta2_api.py` & `timeplus-1.2.2/swagger_test/test_views_v1beta2_api.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/test/test_stream.py` & `timeplus-1.2.2/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/timeplus/env.py` & `timeplus-1.2.2/timeplus/env.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/timeplus/query.py` & `timeplus-1.2.2/timeplus/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,32 @@
         self._env = env
         self._configuration = self._env._conf()
         self._api_instance = swagger_client.QueriesV1beta2Api(
             swagger_client.ApiClient(self._configuration)
         )
         self._create_response = None
         self._id = None
-        self._batching_pilicy = None
+        self._batching_policy = None
 
     def sql(self, query):
         self._sql = query
         return self
 
-    def batching_pilicy(self, count, time_ms):
-        self._batching_pilicy = swagger_client.models.BatchingPolicy(
+    # refer to https://docs.timeplus.com/rest.html#tag/Queries-v1beta2/paths/~1v1beta2~1queries/post
+    # count : The max result count per batch
+    # time_ms : The max interval per batch in milliseconds
+    def batching_policy(self, count, time_ms):
+        self._batching_policy = swagger_client.models.BatchingPolicy(
             count=count, time_ms=time_ms
         )
         return self
 
     def create(self):
         body = swagger_client.CreateQueryRequestV1Beta2(
-            sql=self._sql, batching_policy=self._batching_pilicy
+            sql=self._sql, batching_policy=self._batching_policy
         )
         try:
             # as to support sse, the reponse is urllib3.response.HTTPResponse
             # instead of swagger_client.models.query.Query
             self._create_response = self._api_instance.v1beta2_queries_post(body)
             _sse_client = sseclient.SSEClient(self._create_response)
             self._events = _sse_client.events()
@@ -48,14 +51,20 @@
                 % e
             )
             raise e
 
     def metadata(self):
         return self._metadata
 
+    def id(self):
+        return self._id
+
+    def header(self):
+        return self._metadata["result"]["header"]
+
     def result(self):
         return self._events
 
     def delete(self):
         self._api_instance.v1beta2_queries_id_delete(self._id)
 
     def cancel(self):
```

### Comparing `timeplus-1.2.1/timeplus/stream.py` & `timeplus-1.2.2/timeplus/stream.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/timeplus/type.py` & `timeplus-1.2.2/timeplus/type.py`

 * *Files identical despite different names*

### Comparing `timeplus-1.2.1/timeplus.egg-info/SOURCES.txt` & `timeplus-1.2.2/timeplus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

