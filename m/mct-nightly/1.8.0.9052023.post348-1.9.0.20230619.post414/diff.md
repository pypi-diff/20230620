# Comparing `tmp/mct-nightly-1.8.0.9052023.post348.tar.gz` & `tmp/mct-nightly-1.9.0.20230619.post414.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-nightly-1.8.0.9052023.post348.tar", last modified: Tue May  9 00:03:48 2023, max compression
+gzip compressed data, was "mct-nightly-1.9.0.20230619.post414.tar", last modified: Mon Jun 19 00:04:15 2023, max compression
```

## Comparing `mct-nightly-1.8.0.9052023.post348.tar` & `mct-nightly-1.9.0.20230619.post414.tar`

### file list

```diff
@@ -1,587 +1,529 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10466 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.916520 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12314 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39250 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.916520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/base_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/base_substitutions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/base_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/histogram_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/mean_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/defaultdict.py
--rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/layer_fusing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.920520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/functional_node.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_matchers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_searches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/cut.py
--rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
--rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/
--rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_graph_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/edge_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/node_matcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/walk_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/memory_computation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
--rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_builder_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.924520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/edit_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/node_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/core_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/debug_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5142 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/similarity_analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.928521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/user_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/nn_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3837 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15550 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.932520 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
--rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_model_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_node_prior_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/connectivity_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/node_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/tf_tensor_numpy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.936521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/visualization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5157 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12690 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/default_framework_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
--rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/kpi_data_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
--rw-r--r--   0 runner    (1001) docker     (123)    25698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.940521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/graph_builders.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/node_holders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3069 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8646 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.944521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9507 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_training.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    15915 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    14583 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8544 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_training.py
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/graph_info.py
--rw-r--r--   0 runner    (1001) docker     (123)    12319 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4221 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.948521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/keras_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    17223 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/pytorch_quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8375 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/quantization_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/qat_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13618 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11892 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantization_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.952521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7478 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3479 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8669 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11248 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.956521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/immutable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9107 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.960521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.964521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-09 00:03:09.000000 mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-09 00:03:48.968521 mct-nightly-1.8.0.9052023.post348/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-09 00:03:48.000000 mct-nightly-1.8.0.9052023.post348/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10054 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11727 2023-06-19 00:04:15.000000 mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    32808 2023-06-19 00:04:15.000000 mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 00:04:15.000000 mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-19 00:04:15.000000 mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-19 00:04:15.000000 mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/back2framework/base_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/base_substitutions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/base_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/histogram_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/mean_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7929 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/statistics_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2281 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/defaultdict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22391 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/fusion/layer_fusing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.331306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28860 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/base_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20579 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/base_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/functional_node.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4732 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/graph_matchers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5128 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/graph_searches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2612 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/cut.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17045 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3091 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/base_graph_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2210 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/base_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3706 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/edge_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1773 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2745 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/node_matcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1111 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/walk_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/memory_computation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6704 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19323 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8041 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6822 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34622 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/search_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15453 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25266 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6326 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/model_builder_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5005 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/model_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/model_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17994 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/edit_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/node_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.335306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/core_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/debug_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7247 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.339306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8484 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4315 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41685 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantize_node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.339306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7450 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/similarity_analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.339306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10228 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.339306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/apply_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9093 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2250 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10978 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/user_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.339306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/final_config_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/nn_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20099 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/tensorboard_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.339306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16452 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7150 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15316 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3940 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26778 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3872 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10781 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27197 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/keras_model_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/keras_node_prior_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/base_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10902 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.343306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/connectivity_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7906 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/node_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8109 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2022 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/tf_tensor_numpy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/visualization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4976 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18214 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16443 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/default_framework_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.351306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4804 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38353 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9838 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8482 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/kpi_data_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12113 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/graph_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/node_holders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/statistics_correction/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23009 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/fw_agonstic/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4020 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3543 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.355306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/validate_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9508 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_framework_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15167 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_training.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17319 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4564 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4751 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4136 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/gptq_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14668 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/gptq_training.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/graph_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12768 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3893 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9103 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.359306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18116 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/keras_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17664 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/pytorch_quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/pytorch/quantization_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/common/qat_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16051 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13436 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10708 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantization_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5004 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9629 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/immutable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.363306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6040 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6846 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4631 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4209 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8332 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8145 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4714 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8140 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5379 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.367306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6131 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7564 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4212 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-19 00:03:35.000000 mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-19 00:04:15.371306 mct-nightly-1.9.0.20230619.post414/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-19 00:04:14.000000 mct-nightly-1.9.0.20230619.post414/setup.py
```

### Comparing `mct-nightly-1.8.0.9052023.post348/LICENSE.md` & `mct-nightly-1.9.0.20230619.post414/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/PKG-INFO` & `mct-nightly-1.9.0.20230619.post414/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.8.0.9052023.post348
+Version: 1.9.0.20230619.post414
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -16,129 +16,107 @@
         
         MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
         
         
         
         ## Table of Contents
         
-        - [Supported features](#supported-features)
         - [Getting Started](#getting-started)
+        - [Supported features](#supported-features)
         - [Results](#results)
         - [Contributions](#contributions)
         - [License](#license)
         
-        ## Supported Features
-        
-        MCT supports different quantization methods:
-        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
-        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
-        * Quantization aware training (QAT)[*](#experimental-features)
-        
-        
-        | Quantization Method | Complexity                                    | Computational Cost          |
-        |---------------------|-----------------------------------------------|-----------------------------|
-        | PTQ                 | Low                                           | Low (order of minutes)      |
-        | GPTQ                | Mild (parameters fine-tuning using gradients) | Mild (order of 2-3 hours)   |
-        | QAT                 | High                                          | High (order of 12-36 hours) |
-        
-        
-        In addition, MCT supports different quantization schemes for quantizing weights and activations:
-        * Power-Of-Two (hardware-friendly quantization [1])
-        * Symmetric
-        * Uniform
-        
-        Main features:
-        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
-        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
-        
-        
-        #### Experimental features 
-        
-        Some features are experimental and subject to future changes. 
-         
-        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-        
         
         ## Getting Started
         
-        This section provides a quick starting guide. We begin with installation via source code or pip server. Then, we provide a short usage example.
+        This section provides an installation and a quick starting guide.
         
         ### Installation
-        See the MCT install guide for the pip package, and build from the source.
-        
         
-        #### From Source
-        ```
-        git clone https://github.com/sony/model_optimization.git
-        python setup.py install
-        ```
-        #### From PyPi - latest stable release
+        To install the latest stable release of MCT, run the following command:
         ```
         pip install model-compression-toolkit
         ```
         
-        A nightly package is also available (unstable):
-        ```
-        pip install mct-nightly
-        ```
-        
-        ### Requirements
+        For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
         
-        To run MCT, one of the supported frameworks, Tensorflow/Pytorch, needs to be installed.
         
-        For use with Tensorflow please install the packages: 
-        [tensorflow](https://www.tensorflow.org/install), 
-        [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+        ### Quick start & tutorials 
         
-        For use with PyTorch please install the packages: 
-        [torch](https://pytorch.org/)
+        For an example of how to use MCT with TensorFlow or PyTorch on various models and tasks,
+        check out the [quick-start page](tutorials/quick_start/README.md) and
+        the [results CSV](tutorials/quick_start/results/model_quantization_results.csv).
         
-        Also, a [requirements](requirements.txt) file can be used to set up your environment.
+        In addition, a set of [notebooks](tutorials/notebooks) are provided for an easy start. For example:
+        * [MobileNet with Tensorflow](tutorials/notebooks/example_keras_mobilenet.py).
+        * [MobileNetV2 with PyTorch](tutorials/notebooks/example_pytorch_mobilenet_v2.py).
         
         
         ### Supported Python Versions
         
         Currently, MCT is being tested on various Python versions:
         
-        
-        
         | Python Version                                                                                                                                                                                                                                                            |
         |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
         | [![Run Tests - Python 3.10](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python310.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python310.yml) |
         | [![Run Tests - Python 3.9](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python39.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python39.yml)   |
         | [![Run Tests - Python 3.8](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python38.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python38.yml)   |
         | [![Run Tests - Python 3.7](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python37.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python37.yml)   |
         
         
         ### Supported NN-Frameworks Versions
         
-        Currently, MCT supports compressing models of TensorFlow and PyTorch, and
-        is tested on various versions:
+        MCT supports compressing models built with the TensorFlow or PyTorch frameworks, and is tested on various python versions:
         
         | TensorFlow Version                                                                                   | PyTorch Version                                                                                          |
         |------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
         | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf211.yml/badge.svg) | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_13.yml/badge.svg) |
         | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf210.yml/badge.svg) | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_12.yml/badge.svg) |
         | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf29.yml/badge.svg)  | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_11.yml/badge.svg) |
         
         
-        ### Usage Example 
-        For an example of how to use the post-training quantization, using Keras,
-        please use this [link](tutorials/example_keras_mobilenet.py).
+        ## Supported Features
+        
+        MCT supports different quantization methods:
+        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
+        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
+        * Quantization-aware training (QAT)[*](#experimental-features)
+        
+        
+        | Quantization Method                           | Complexity | Computational Cost          |
+        |-----------------------------------------------|------------|-----------------------------|
+        | PTQ                                           | Low        | Low (order of minutes)      |
+        | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+        | QAT                                           | High       | High (order of 12-36 hours) |
+        
+        
+        In addition, MCT supports different quantization schemes for quantizing weights and activations:
+        
+        * Power-Of-Two (hardware-friendly quantization [1])
+        * Symmetric
+        * Uniform
+        
+        Main features:
+        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
+        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
+        
         
-        For an example using PyTorch, please use this [link](tutorials/example_pytorch_mobilenet_v2.py).
+        #### Experimental features 
         
-        For more examples please see the [tutorials' directory](https://github.com/sony/model_optimization/tree/main/tutorials).
+        Some features are experimental and subject to future changes. 
+         
+        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
         
         
         ## Results
         ### Keras
         Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
         single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
         
@@ -152,15 +130,15 @@
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | 
         | --------------------------| ---------------:| ---------------:| 
         | MobileNet V2 [3]          | 71.886          | 71.444           |                                      
         | ResNet-18 [3]             | 69.86           | 69.63           |                                      
         | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |                                      
         
-        
+        For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
         
         ## Contributions
         MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
         
         *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
```

### Comparing `mct-nightly-1.8.0.9052023.post348/README.md` & `mct-nightly-1.9.0.20230619.post414/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,129 +10,107 @@
 
 MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
 
 
 
 ## Table of Contents
 
-- [Supported features](#supported-features)
 - [Getting Started](#getting-started)
+- [Supported features](#supported-features)
 - [Results](#results)
 - [Contributions](#contributions)
 - [License](#license)
 
-## Supported Features
-
-MCT supports different quantization methods:
-* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
-* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
-* Quantization aware training (QAT)[*](#experimental-features)
-
-
-| Quantization Method | Complexity                                    | Computational Cost          |
-|---------------------|-----------------------------------------------|-----------------------------|
-| PTQ                 | Low                                           | Low (order of minutes)      |
-| GPTQ                | Mild (parameters fine-tuning using gradients) | Mild (order of 2-3 hours)   |
-| QAT                 | High                                          | High (order of 12-36 hours) |
-
-
-In addition, MCT supports different quantization schemes for quantizing weights and activations:
-* Power-Of-Two (hardware-friendly quantization [1])
-* Symmetric
-* Uniform
-
-Main features:
-* <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-* <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-  * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-  * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-* <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
-* <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-* <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
-
-
-#### Experimental features 
-
-Some features are experimental and subject to future changes. 
- 
-For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-
 
 ## Getting Started
 
-This section provides a quick starting guide. We begin with installation via source code or pip server. Then, we provide a short usage example.
+This section provides an installation and a quick starting guide.
 
 ### Installation
-See the MCT install guide for the pip package, and build from the source.
-
 
-#### From Source
-```
-git clone https://github.com/sony/model_optimization.git
-python setup.py install
-```
-#### From PyPi - latest stable release
+To install the latest stable release of MCT, run the following command:
 ```
 pip install model-compression-toolkit
 ```
 
-A nightly package is also available (unstable):
-```
-pip install mct-nightly
-```
-
-### Requirements
+For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
 
-To run MCT, one of the supported frameworks, Tensorflow/Pytorch, needs to be installed.
 
-For use with Tensorflow please install the packages: 
-[tensorflow](https://www.tensorflow.org/install), 
-[tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+### Quick start & tutorials 
 
-For use with PyTorch please install the packages: 
-[torch](https://pytorch.org/)
+For an example of how to use MCT with TensorFlow or PyTorch on various models and tasks,
+check out the [quick-start page](tutorials/quick_start/README.md) and
+the [results CSV](tutorials/quick_start/results/model_quantization_results.csv).
 
-Also, a [requirements](requirements.txt) file can be used to set up your environment.
+In addition, a set of [notebooks](tutorials/notebooks) are provided for an easy start. For example:
+* [MobileNet with Tensorflow](tutorials/notebooks/example_keras_mobilenet.py).
+* [MobileNetV2 with PyTorch](tutorials/notebooks/example_pytorch_mobilenet_v2.py).
 
 
 ### Supported Python Versions
 
 Currently, MCT is being tested on various Python versions:
 
-
-
 | Python Version                                                                                                                                                                                                                                                            |
 |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | [![Run Tests - Python 3.10](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python310.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python310.yml) |
 | [![Run Tests - Python 3.9](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python39.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python39.yml)   |
 | [![Run Tests - Python 3.8](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python38.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python38.yml)   |
 | [![Run Tests - Python 3.7](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python37.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python37.yml)   |
 
 
 ### Supported NN-Frameworks Versions
 
-Currently, MCT supports compressing models of TensorFlow and PyTorch, and
-is tested on various versions:
+MCT supports compressing models built with the TensorFlow or PyTorch frameworks, and is tested on various python versions:
 
 | TensorFlow Version                                                                                   | PyTorch Version                                                                                          |
 |------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
 | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf211.yml/badge.svg) | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_13.yml/badge.svg) |
 | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf210.yml/badge.svg) | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_12.yml/badge.svg) |
 | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf29.yml/badge.svg)  | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_11.yml/badge.svg) |
 
 
-### Usage Example 
-For an example of how to use the post-training quantization, using Keras,
-please use this [link](tutorials/example_keras_mobilenet.py).
+## Supported Features
+
+MCT supports different quantization methods:
+* Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
+* Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
+* Quantization-aware training (QAT)[*](#experimental-features)
+
+
+| Quantization Method                           | Complexity | Computational Cost          |
+|-----------------------------------------------|------------|-----------------------------|
+| PTQ                                           | Low        | Low (order of minutes)      |
+| GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+| QAT                                           | High       | High (order of 12-36 hours) |
+
+
+In addition, MCT supports different quantization schemes for quantizing weights and activations:
+
+* Power-Of-Two (hardware-friendly quantization [1])
+* Symmetric
+* Uniform
+
+Main features:
+* <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+* <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+* <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+  * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+  * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+* <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
+* <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+* <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+* <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
+
 
-For an example using PyTorch, please use this [link](tutorials/example_pytorch_mobilenet_v2.py).
+#### Experimental features 
 
-For more examples please see the [tutorials' directory](https://github.com/sony/model_optimization/tree/main/tutorials).
+Some features are experimental and subject to future changes. 
+ 
+For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
 
 
 ## Results
 ### Keras
 Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
 single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
 
@@ -146,15 +124,15 @@
 
 | Network Name              | Float Accuracy  | 8Bit Accuracy   | 
 | --------------------------| ---------------:| ---------------:| 
 | MobileNet V2 [3]          | 71.886          | 71.444           |                                      
 | ResNet-18 [3]             | 69.86           | 69.63           |                                      
 | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |                                      
 
-
+For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
 
 ## Contributions
 MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
 
 *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
```

### Comparing `mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/PKG-INFO` & `mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-nightly
-Version: 1.8.0.9052023.post348
+Version: 1.9.0.20230619.post414
 Summary: A Model Compression Toolkit for neural networks
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT)
         
         Model Compression Toolkit (MCT) is an open-source project for neural network model optimization under efficient, constrained hardware.
         
@@ -16,129 +16,107 @@
         
         MCT is developed by researchers and engineers working at Sony Semiconductor Israel.
         
         
         
         ## Table of Contents
         
-        - [Supported features](#supported-features)
         - [Getting Started](#getting-started)
+        - [Supported features](#supported-features)
         - [Results](#results)
         - [Contributions](#contributions)
         - [License](#license)
         
-        ## Supported Features
-        
-        MCT supports different quantization methods:
-        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
-        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
-        * Quantization aware training (QAT)[*](#experimental-features)
-        
-        
-        | Quantization Method | Complexity                                    | Computational Cost          |
-        |---------------------|-----------------------------------------------|-----------------------------|
-        | PTQ                 | Low                                           | Low (order of minutes)      |
-        | GPTQ                | Mild (parameters fine-tuning using gradients) | Mild (order of 2-3 hours)   |
-        | QAT                 | High                                          | High (order of 12-36 hours) |
-        
-        
-        In addition, MCT supports different quantization schemes for quantizing weights and activations:
-        * Power-Of-Two (hardware-friendly quantization [1])
-        * Symmetric
-        * Uniform
-        
-        Main features:
-        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
-        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
-        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
-          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
-          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
-        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
-        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
-        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
-        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
-        
-        
-        #### Experimental features 
-        
-        Some features are experimental and subject to future changes. 
-         
-        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
-        
         
         ## Getting Started
         
-        This section provides a quick starting guide. We begin with installation via source code or pip server. Then, we provide a short usage example.
+        This section provides an installation and a quick starting guide.
         
         ### Installation
-        See the MCT install guide for the pip package, and build from the source.
-        
         
-        #### From Source
-        ```
-        git clone https://github.com/sony/model_optimization.git
-        python setup.py install
-        ```
-        #### From PyPi - latest stable release
+        To install the latest stable release of MCT, run the following command:
         ```
         pip install model-compression-toolkit
         ```
         
-        A nightly package is also available (unstable):
-        ```
-        pip install mct-nightly
-        ```
-        
-        ### Requirements
+        For installing the nightly version or installing from source, refer to the [installation guide](INSTALLATION.md).
         
-        To run MCT, one of the supported frameworks, Tensorflow/Pytorch, needs to be installed.
         
-        For use with Tensorflow please install the packages: 
-        [tensorflow](https://www.tensorflow.org/install), 
-        [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+        ### Quick start & tutorials 
         
-        For use with PyTorch please install the packages: 
-        [torch](https://pytorch.org/)
+        For an example of how to use MCT with TensorFlow or PyTorch on various models and tasks,
+        check out the [quick-start page](tutorials/quick_start/README.md) and
+        the [results CSV](tutorials/quick_start/results/model_quantization_results.csv).
         
-        Also, a [requirements](requirements.txt) file can be used to set up your environment.
+        In addition, a set of [notebooks](tutorials/notebooks) are provided for an easy start. For example:
+        * [MobileNet with Tensorflow](tutorials/notebooks/example_keras_mobilenet.py).
+        * [MobileNetV2 with PyTorch](tutorials/notebooks/example_pytorch_mobilenet_v2.py).
         
         
         ### Supported Python Versions
         
         Currently, MCT is being tested on various Python versions:
         
-        
-        
         | Python Version                                                                                                                                                                                                                                                            |
         |---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
         | [![Run Tests - Python 3.10](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python310.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python310.yml) |
         | [![Run Tests - Python 3.9](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python39.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python39.yml)   |
         | [![Run Tests - Python 3.8](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python38.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python38.yml)   |
         | [![Run Tests - Python 3.7](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python37.yml/badge.svg)](https://github.com/sony/model_optimization/actions/workflows/run_tests_suite_python37.yml)   |
         
         
         ### Supported NN-Frameworks Versions
         
-        Currently, MCT supports compressing models of TensorFlow and PyTorch, and
-        is tested on various versions:
+        MCT supports compressing models built with the TensorFlow or PyTorch frameworks, and is tested on various python versions:
         
         | TensorFlow Version                                                                                   | PyTorch Version                                                                                          |
         |------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------|
         | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf211.yml/badge.svg) | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_13.yml/badge.svg) |
         | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf210.yml/badge.svg) | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_12.yml/badge.svg) |
         | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_tf29.yml/badge.svg)  | ![tests](https://github.com/sony/model_optimization/actions/workflows/run_tests_torch1_11.yml/badge.svg) |
         
         
-        ### Usage Example 
-        For an example of how to use the post-training quantization, using Keras,
-        please use this [link](tutorials/example_keras_mobilenet.py).
+        ## Supported Features
+        
+        MCT supports different quantization methods:
+        * Post-training quantization (PTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_post_training_quantization_experimental.html#ug-keras-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_post_training_quantization_experimental.html#ug-pytorch-post-training-quantization-experimental)
+        * Gradient-based post-training quantization (GPTQ): [Keras API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/keras_gradient_post_training_quantization_experimental.html#ug-keras-gradient-post-training-quantization-experimental), [PyTorch API](https://sony.github.io/model_optimization/docs/api/experimental_api_docs/methods/pytorch_gradient_post_training_quantization_experimental.html#ug-pytorch-gradient-post-training-quantization-experimental)
+        * Quantization-aware training (QAT)[*](#experimental-features)
+        
+        
+        | Quantization Method                           | Complexity | Computational Cost          |
+        |-----------------------------------------------|------------|-----------------------------|
+        | PTQ                                           | Low        | Low (order of minutes)      |
+        | GPTQ (parameters fine-tuning using gradients) | Mild       | Mild (order of 2-3 hours)   |
+        | QAT                                           | High       | High (order of 12-36 hours) |
+        
+        
+        In addition, MCT supports different quantization schemes for quantizing weights and activations:
+        
+        * Power-Of-Two (hardware-friendly quantization [1])
+        * Symmetric
+        * Uniform
+        
+        Main features:
+        * <ins>Graph optimizations:</ins> Transforming the model to an equivalent (yet, more efficient) model (for example, batch-normalization layer folding to its preceding linear layer).
+        * <ins>Quantization parameter search:</ins> Different methods can be used to minimize the expected added quantization-noise during thresholds search (by default, we use Mean-Square-Error, but other metrics can be used such as No-Clipping, Mean-Average-Error, and more).
+        * <ins>Advanced quantization algorithms:</ins> To prevent a performance degradation some algorithms are applied such as: 
+          * <ins>Shift negative correction:</ins> Symmetric activation quantization can hurt the model's performance when some layers output both negative and positive activations, but their range is asymmetric. For more details please visit [1].
+          * <ins>Outliers filtering:</ins> Computing z-score for activation statistics to detect and remove outliers.
+        * <ins>Clustering:</ins> Using non-uniform quantization grid to quantize the weights and activations to match their distributions.[*](#experimental-features)
+        * <ins>Mixed-precision search:</ins> Assigning quantization bit-width per layer (for weights/activations), based on the layer's sensitivity to different bit-widths.
+        * <ins>Visualization:</ins> You can use TensorBoard to observe useful information for troubleshooting the quantized model's performance (for example, the model in different phases of the quantization, collected statistics, similarity between layers of the float and quantized model and bit-width configuration for mixed-precision quantization). For more details, please read the [visualization documentation](https://sony.github.io/model_optimization/docs/guidelines/visualization.html).   
+        * <ins>Target Platform Capabilities:</ins> The Target Platform Capabilities (TPC) describes the target platform (an edge device with dedicated hardware). For more details, please read the [TPC README](model_compression_toolkit/target_platform_capabilities/README.md).   
+        
         
-        For an example using PyTorch, please use this [link](tutorials/example_pytorch_mobilenet_v2.py).
+        #### Experimental features 
         
-        For more examples please see the [tutorials' directory](https://github.com/sony/model_optimization/tree/main/tutorials).
+        Some features are experimental and subject to future changes. 
+         
+        For more details, we highly recommend visiting our project website where experimental features are mentioned as experimental.
         
         
         ## Results
         ### Keras
         Graph of [MobileNetV2](https://keras.io/api/applications/mobilenet/) accuracy on ImageNet vs average bit-width of weights, using 
         single-precision quantization, mixed-precision quantization, and mixed-precision quantization with GPTQ.
         
@@ -152,15 +130,15 @@
         
         | Network Name              | Float Accuracy  | 8Bit Accuracy   | 
         | --------------------------| ---------------:| ---------------:| 
         | MobileNet V2 [3]          | 71.886          | 71.444           |                                      
         | ResNet-18 [3]             | 69.86           | 69.63           |                                      
         | SqueezeNet 1.1 [3]        | 58.128          | 57.678          |                                      
         
-        
+        For more results, please refer to [quick start](https://github.com/sony/model_optimization/tree/main/tutorials/quick_start).
         
         ## Contributions
         MCT aims at keeping a more up-to-date fork and welcomes contributions from anyone.
         
         *You will find more information about contributions in the [Contribution guide](CONTRIBUTING.md).
```

### Comparing `mct-nightly-1.8.0.9052023.post348/mct_nightly.egg-info/SOURCES.txt` & `mct-nightly-1.9.0.20230619.post414/mct_nightly.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -240,25 +240,25 @@
 model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py
 model_compression_toolkit/exporter/__init__.py
 model_compression_toolkit/exporter/model_exporter/__init__.py
 model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py
 model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py
 model_compression_toolkit/exporter/model_exporter/keras/__init__.py
 model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py
+model_compression_toolkit/exporter/model_exporter/keras/export_serialization_format.py
 model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_keras_exporter.py
+model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py
+model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py
 model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py
 model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py
 model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py
+model_compression_toolkit/exporter/model_exporter/pytorch/export_serialization_format.py
 model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py
 model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py
 model_compression_toolkit/exporter/model_exporter/pytorch/pytorch_export_facade.py
-model_compression_toolkit/exporter/model_exporter/tflite/__init__.py
-model_compression_toolkit/exporter/model_exporter/tflite/fakely_quant_tflite_exporter.py
-model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py
-model_compression_toolkit/exporter/model_exporter/tflite/tflite_export_facade.py
 model_compression_toolkit/exporter/model_wrapper/__init__.py
 model_compression_toolkit/exporter/model_wrapper/keras/__init__.py
 model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py
 model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py
 model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py
 model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py
 model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py
@@ -336,75 +336,14 @@
 model_compression_toolkit/qat/pytorch/quantizer/__init__.py
 model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py
 model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py
 model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py
 model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py
-model_compression_toolkit/quantizers_infrastructure/__init__.py
-model_compression_toolkit/quantizers_infrastructure/constants.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/base_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/constants.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_all_subclasses.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/get_quantizers.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/quant_utils.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantize_wrapper.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizer_utils.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/validation_functions.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantize_wrapper.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizer_utils.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_pytorch_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/base_uniform_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/constants.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py
-model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
 model_compression_toolkit/target_platform_capabilities/__init__.py
 model_compression_toolkit/target_platform_capabilities/constants.py
 model_compression_toolkit/target_platform_capabilities/immutable.py
 model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py
 model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py
 model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py
 model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py
@@ -468,8 +407,23 @@
 model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py
 model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py
-model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py
+model_compression_toolkit/trainable_infrastructure/__init__.py
+model_compression_toolkit/trainable_infrastructure/common/__init__.py
+model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py
+model_compression_toolkit/trainable_infrastructure/common/constants.py
+model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py
+model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py
+model_compression_toolkit/trainable_infrastructure/common/quant_utils.py
+model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py
+model_compression_toolkit/trainable_infrastructure/keras/__init__.py
+model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py
+model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py
+model_compression_toolkit/trainable_infrastructure/keras/load_model.py
+model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py
+model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py
+model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/analyzer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/back2framework/base_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/back2framework/base_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/base_substitutions.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/base_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/base_collector.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/base_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/histogram_collector.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/histogram_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/mean_collector.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/mean_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/min_max_per_channel_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/statistics_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/collectors/statistics_collector_generator.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/data_loader.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/data_loader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/defaultdict.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/defaultdict.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_implementation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/framework_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/framework_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from enum import Enum
 from typing import Dict, Any, List
 
 
 
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.core.common.graph.base_node import BaseNode
-from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import QuantizationMethod
+from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
 
 
 class ChannelAxis(Enum):
     """
 
     Index of output channels axis:
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/fusion/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/fusion/layer_fusing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/fusion/layer_fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/base_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/base_node.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/base_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/edge.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/edge.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/functional_node.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/functional_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_matchers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/graph_matchers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/graph_searches.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/graph_searches.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/bipartite_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/compute_graph_max_cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/cut.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/cut.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/max_cut_astar.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/memory_element.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/memory_graph/memory_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/graph/virtual_activation_weights_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_graph_filter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/base_graph_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/base_matcher.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/base_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/edge_matcher.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/edge_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/function.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/function.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/node_matcher.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/node_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/matchers/walk_matcher.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/matchers/walk_matcher.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/memory_computation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/memory_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/bit_width_setter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/distance_weighting.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_aggregation_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_data.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_functions_mapping.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/kpi_tools/kpi_methods.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/mixed_precision_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/mixed_precision_search_manager.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/search_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/search_methods/linear_programming.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/sensitivity_evaluation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/mixed_precision/solution_refinement_procedure.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_builder_mode.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/model_builder_mode.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_collector.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/model_collector.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/model_validation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/actions.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/actions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/edit_network.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/edit_network.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/network_editors/node_filters.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/network_editors/node_filters.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/node_prior_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/candidate_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/core_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/core_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/debug_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/debug_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/filter_nodes_candidates.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/node_quantization_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_analyzer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_fn_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/error_functions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/lut_kmeans_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/outlier_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/power_of_two_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_activations_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_search.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/qparams_weights_computation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/symmetric_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantization_params_generation/uniform_selection.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantize_graph_weights.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantize_node.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantize_node.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/lut_kmeans_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/quantizers_helpers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/quantizers/uniform_quantizers.py`

 * *Files 12% similar despite different names*

```diff
@@ -51,14 +51,17 @@
         Quantized data.
     """
     threshold = quantization_params.get(THRESHOLD)
     if threshold is None:
         Logger.error(f"{THRESHOLD} parameter must be defined in 'quantization_params'")  # pragma: no cover
     if not threshold_is_power_of_two(threshold, per_channel):
         Logger.error(f"Expects {THRESHOLD} parameter to be a power of two, but got {threshold}")  # pragma: no cover
+    if (per_channel and (threshold <= 0).any()) or ((not per_channel) and threshold <= 0):
+        Logger.error(f"{THRESHOLD} parameter must positive")  # pragma: no cover
+
 
     return quantize_tensor(tensor_data,
                            threshold,
                            n_bits,
                            signed)
 
 
@@ -83,14 +86,17 @@
     Returns:
         Quantized data.
     """
     threshold = quantization_params.get(THRESHOLD)
     if threshold is None:
         Logger.error(f"{THRESHOLD} parameter must be defined in 'quantization_params'")  # pragma: no cover
 
+    if (per_channel and np.any(threshold <= 0)) or (not per_channel and threshold <= 0):
+        Logger.error(f"{THRESHOLD} parameter must positive")  # pragma: no cover
+
     return quantize_tensor(tensor_data,
                            threshold,
                            n_bits,
                            signed)
 
 
 def uniform_quantizer(tensor_data: np.ndarray,
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/quantization/set_node_quantization_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/similarity_analyzer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/similarity_analyzer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/apply_bias_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/apply_second_moment_correction_to_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/compute_bias_correction_of_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/statistics_correction/statistics_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/apply_substitutions.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/apply_substitutions.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/linear_collapsing_substitution.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/user_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/user_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/final_config_visualizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/final_config_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/nn_visualizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/nn_visualizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/common/visualization/tensorboard_writer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/common/visualization/tensorboard_writer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/exporter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/instance_builder.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,22 +27,30 @@
 
 
 class OperationHandler:
     """
     Class to handle conversions from graph nodes to Keras operators and retrieving them.
     """
 
-    def __init__(self, graph: Graph):
+    def __init__(self, graph: Graph, wrapper: Callable = None):
+        """
+
+        Args:
+            graph: Graph to build its layers based on its nodes.
+            wrapper: Wrapper to use for wrapping the layers.
+        """
+
         # hold nodes after sorting them
         self.node_sort = list(topological_sort(graph))
 
         self.layer_to_node_dict = {}
 
         # hold dictionary from node to its equivalent Keras layer
-        self.node_to_fw_op_dict = instance_builder(self.node_sort)
+        self.node_to_fw_op_dict = instance_builder(self.node_sort,
+                                                   wrapper)
 
     def get_node_op_function(self, n: BaseNode) -> Layer:
         """
         Get the Keras layer that was built from the passed node.
 
         Args:
             n: Node to get its equivalent Keras layer.
@@ -70,42 +78,41 @@
     Args:
         n: Node to build its Keras layer
 
     Returns:
         Keras layer that was built from the node.
     """
     framework_attr = copy.copy(n.framework_attr)
-    if n.layer_class is InputLayer:
-        # replace input node with identity, so can wrap it with QuantizationWrapper
-        _layer_class = Layer  # Identity
-        framework_attr = {}
-    else:
-        _layer_class = n.layer_class
+    _layer_class = n.layer_class
     framework_attr[LAYER_NAME] = n.name  # Overwrite framework name to identical graph node name
     node_instance = _layer_class.from_config(framework_attr)  # Build layer from node's configuration.
     with tf.name_scope(n.name):
         # Add layer name to default weight name to avoid name duplications
         node_instance.build(n.input_shape)
     node_instance.set_weights(n.get_weights_list())
     node_instance.trainable = False  # Set all node as not trainable
     return node_instance
 
 
-def instance_builder(toposort: List[BaseNode]) -> Dict[BaseNode, Layer]:
+def instance_builder(toposort: List[BaseNode],
+                     wrapper: Callable = None) -> Dict[BaseNode, Layer]:
     """
     Build a dictionary of nodes to their corresponding Keras
     layers, given a list of nodes.
 
     Args:
         toposort: List of nodes sorted topological to build their layers.
+        wrapper: Wrapper to use for wrapping the layers.
 
     Returns:
         A dictionary of nodes to their corresponding Keras layers.
     """
 
     nodes_dict = dict()
     for n in toposort:
         if not n.reuse:  # Hold a single node in dictionary for all reused nodes from the same layer.
             keras_node = node_builder(n)
+            if wrapper is not None:
+                keras_node = wrapper(n, keras_node)
             nodes_dict.update({n: keras_node})
 
     return nodes_dict
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/keras_model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 # ==============================================================================
 
 import tensorflow as tf
 from keras.engine.input_layer import InputLayer
 from keras.models import Model, clone_model
 from packaging import version
 
+from model_compression_toolkit.constants import INPUT_BASE_NAME
 from model_compression_toolkit.core.common.back2framework.base_model_builder import BaseModelBuilder
 from model_compression_toolkit.core.common.user_info import UserInformation
-from model_compression_toolkit.constants import INPUT_BASE_NAME
+from mct_quantizers import KerasActivationQuantizationHolder
 
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.keras.layers import Input
     from tensorflow.python.keras.layers.core import TFOpLambda
     from tensorflow.python.keras.engine.base_layer import TensorFlowOpLayer
     from tensorflow.python.keras.layers import Layer
@@ -88,33 +89,50 @@
     """
 
     def __init__(self,
                  graph: common.Graph,
                  append2output=None,
                  fw_info: FrameworkInfo = DEFAULT_KERAS_INFO,
                  return_float_outputs: bool = False,
-                 wrapper: Callable = None):
+                 wrapper: Callable = None,
+                 get_activation_quantizer_holder_fn: Callable=None):
         """
 
         Args:
             graph: Graph to build the model from.
             append2output: Nodes to append to model's output.
             fw_info: Information about the specific framework of the model that is built.
             return_float_outputs: Whether the model returns float tensors or not.
             wrapper: A function wrapper keras Layers.
+            get_activation_quantizer_holder_fn: Function to retrieve a quantization holder for a node.
+
         """
 
         super().__init__(graph,
                          append2output,
                          fw_info,
                          return_float_outputs)
 
         # Build an OperationHandler to handle conversions from graph nodes to Keras operators.
-        self.oh = OperationHandler(self.graph)
+        self.oh = OperationHandler(self.graph,
+                                   wrapper=wrapper)
         self.wrapper = wrapper
+        self.get_activation_quantizer_holder = get_activation_quantizer_holder_fn
+
+    @property
+    def use_activation_holder_during_model_building(self) -> bool:
+        """
+
+        Returns: Whether the model builder uses KerasActivationQuantizationHolder during
+        model building (by adding it as a layer when converting the graph to the Keras model)
+        or not. If so - the model builder expects the activation quantizers to not be wrapped
+        in KerasQuantizeWrapper that was received in its init.
+
+        """
+        return self.get_activation_quantizer_holder is not None
 
     def _quantize_node_activations(self,
                                    node: BaseNode,
                                    input_tensors: List[TFReference]) -> List[TFReference]:
         """
         Quantize node's activation given input tensors.
 
@@ -151,46 +169,41 @@
         # building the model. Initially input nodes with input tensors are added to the dictionary,
         # as they're not added later.
         input_nodes_to_input_tensors = {inode: Input(inode.framework_attr[BATCH_INPUT_SHAPE][1:],
                                                      name=f'{inode.name}_{INPUT_BASE_NAME}')
                                         for
                                         inode in self.graph.get_inputs()}
 
-        # Support adding Layer after input layers require us to store it in layer_to_node_dict
-        # dict offline (unlike other layers which stored during running).
-        for node, layer in self.oh.node_to_fw_op_dict.items():
-            if node.type == InputLayer:
-                self.oh.layer_to_node_dict[layer] = node
 
         # Build a list of the model's input tensors. Switching from a dictionary to a list
         # to keep the tensors input order, since inputs in Graph are ordered by their indices.
         inputs_list = []
         for input_node in self.graph.get_inputs():
             inputs_list.append(input_nodes_to_input_tensors.get(input_node))
 
         # Build a dictionary from node to its output tensors, by applying the layers sequentially.
         for n in self.oh.node_sort:
-            op_func = self.oh.get_node_op_function(n)  # Get node operation function
+            op_func = self.oh.get_node_op_function(n) # Get node operation function
+
             input_tensors = self._build_input_tensors_list(n,
                                                            node_to_output_tensors_dict)  # Fetch Node inputs
             out_tensors_of_n, out_tensors_of_n_float = self._run_operation(n,  # Run node operation and fetch outputs
                                                                            input_tensors,
                                                                            op_func,
                                                                            input_nodes_to_input_tensors)
 
             if isinstance(out_tensors_of_n, (list, tuple)):
                 node_to_output_tensors_dict.update({n: out_tensors_of_n})
                 node_to_output_tensors_dict_float.update({n: out_tensors_of_n_float})
             else:
                 node_to_output_tensors_dict.update({n: [out_tensors_of_n]})
                 node_to_output_tensors_dict_float.update({n: [out_tensors_of_n_float]})
 
-        # convert node_to_output_tensors_dict keys to nodes' names since oh.node_sort contains different objects
-        # than
-        # original graph nodes.
+        # convert node_to_output_tensors_dict keys to nodes' names since oh.node_sort
+        # contains different objects than original graph nodes.
         node_name_to_outtensors = self._convert_node2name(node_to_output_tensors_dict)
         node_name_to_outtensors_float = self._convert_node2name(node_to_output_tensors_dict_float)
 
         for ot in output_list:
             if len(node_name_to_outtensors[ot.node.name]) == 1 or self.append2output is None:
                 if self.return_float_outputs:
                     model_output_tensors.append(node_name_to_outtensors_float[ot.node.name][ot.node_out_index])
@@ -203,27 +216,14 @@
                     model_output_tensors.append(node_name_to_outtensors_float[ot.node.name])
                 else:
                     model_output_tensors.append(node_name_to_outtensors[ot.node.name])
 
         # Build the model.
         model = tf.keras.Model(inputs=inputs_list, outputs=model_output_tensors)
 
-        if self.wrapper is not None:
-            def _wrap(layer):
-                _node = self.oh.layer_to_node_dict.get(layer)
-                if _node is not None:
-                    return self.wrapper(_node, layer)
-                elif is_layer_fake_quant(layer):
-                    return layer
-                raise Exception(  # pragma: no cover
-                    f'Mismatch between keras model and graph cant find node named: '
-                    f'{get_node_name_from_layer(layer)}')
-
-            model = clone_model(model, clone_function=_wrap)
-
         return model, self.graph.user_info
 
     def _convert_node2name(self, in_node_to_output_tensors_dict):
         node_name_to_outtensors = dict()
         for node, tensors in in_node_to_output_tensors_dict.items():
             node_name_to_outtensors[node.name] = tensors
         return node_name_to_outtensors
@@ -271,47 +271,69 @@
 
         Returns:
             A list of references to Keras tensors. The layer's output tensors after applying the
             layer to the input tensors.
         """
         if len(input_tensors) == 0:  # Placeholder handling
             out_tensors_of_n_float = input_nodes_to_input_tensors[n]
-            if self.wrapper is not None:
-                # if a wrapper is defined, add an identity layer for cloning. The Identity will be warpped
-                out_tensors_of_n = op_func(out_tensors_of_n_float)
-            elif n.is_activation_quantization_enabled():
-                out_tensors_of_n = self._quantize_node_activations(n, out_tensors_of_n_float)
-            else:
-                out_tensors_of_n = out_tensors_of_n_float
+            out_tensors_of_n = self._run_operation_activation_quantization(n,
+                                                                           out_tensors_of_n_float)
         else:
             input_tensors = [tensor for tensor_list in input_tensors for tensor in tensor_list]  # flat list of lists
             # Build a functional node using its args
             if isinstance(n, FunctionalNode):
                 if n.inputs_as_list:  # If the first argument should be a list of tensors:
                     out_tensors_of_n_float = op_func(input_tensors, *n.op_call_args, **n.op_call_kwargs)
                 else:  # If the input tensors should not be a list but iterated:
                     out_tensors_of_n_float = op_func(*input_tensors, *n.op_call_args, **n.op_call_kwargs)
             else:
                 # If operator expects a single input tensor, it cannot be a list as it should
                 # have a dtype field.
                 if len(input_tensors) == 1:
                     input_tensors = input_tensors[0]
                 out_tensors_of_n_float = op_func(input_tensors)
-            out_tensors_of_n = out_tensors_of_n_float
 
-            # Add a fake quant node if the node has an activation threshold and a wrapper isn't defined
-            if n.is_activation_quantization_enabled() and self.wrapper is None:
-                out_tensors_of_n = self._quantize_node_activations(n, out_tensors_of_n_float)
+            out_tensors_of_n = self._run_operation_activation_quantization(n,
+                                                                           out_tensors_of_n_float)
 
         # Save a mapping from the layer that created the tensor to the node (as this layer is not the
         # same instance as op_func. We do this to solve an issue that names are different between these
         # layers, thus we can not rely on the op_func name during model cloning (such as GPTQ, MP, etc.)
         if not n.reuse:
             if isinstance(out_tensors_of_n_float, (list, tuple)):
                 # If layer has multiple outputs (e.g., split) we take the layer of the first output (as all outputs are
                 # from the same layer).
                 layer_from_tensor = out_tensors_of_n_float[0].node.layer
             else:
                 layer_from_tensor = out_tensors_of_n_float.node.layer
             self.oh.layer_to_node_dict[layer_from_tensor] = n
 
         return out_tensors_of_n, out_tensors_of_n_float
+
+    def _run_operation_activation_quantization(self,
+                                               node: BaseNode,
+                                               node_outputs: List[TFReference]):
+        """
+        Quantize node's activations
+
+        Args:
+            node: Node to quantize its activations
+            node_outputs: Output tensors of the float node.
+
+        Returns:
+            Quantized node's outputs.
+        """
+        if self.wrapper is not None:
+
+            # In case the activation quantizer is attached out of the wrapper we use get_activation_quantizer_holder
+            # for the activation quantization holder (if the node's activations are quantized)
+            if node.is_activation_quantization_enabled() and self.use_activation_holder_during_model_building:
+                activation_quantizer_holder = self.get_activation_quantizer_holder(node)
+                quantized_node_outputs = activation_quantizer_holder(node_outputs)
+                return quantized_node_outputs
+
+        elif node.is_activation_quantization_enabled():  # Used only when old exporter is used
+            quantized_node_outputs = self._quantize_node_activations(node,
+                                                                     node_outputs)
+            return quantized_node_outputs
+
+        return node_outputs
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/mixed_precision_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/back2framework/quantized_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/default_framework_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/activation_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/input_scaling.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/remove_relu_upper_bound.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/separableconv_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_implementation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_model_validation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/keras_model_validation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/keras_node_prior_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/keras_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/kpi_data_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/base_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/base_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/input_layer_quantize_transform.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/quantization_config_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_activation_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/quantizer/mixed_precision/selective_weights_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/common.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/common.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/connectivity_handler.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/connectivity_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/edges_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/nested_model_handler.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/nodes_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/nested_model/outputs_merger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/node_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/node_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/reader/reader.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/tf_tensor_numpy.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/tf_tensor_numpy.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/keras/visualization/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/keras/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/factory_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/float_model_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/instance_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,18 +34,22 @@
     framework_attr = copy.copy(n.framework_attr)
     node_instance = n.type(**framework_attr)
     node_instance.load_state_dict({k: torch.Tensor(v) for k, v in n.weights.items()}, strict=False)
     set_model(node_instance)
     return node_instance
 
 
-def identity_wrapper(node: BaseNode, module: Module):
+# todo: remove. It is not used anymore
+def identity_wrapper(node: BaseNode,
+                     module: Module,
+                     include_activation_quantizers: bool):
     """
     A function which takes a computational graph node and a pytorch module and return an identity wrapping which return the layer itself
     Args:
         node: A node of mct graph.
         layer: A pytorch module
+        include_activation_quantizers: bool flag.
     Returns: pytorch module
     """
     return module
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/mixed_precision_model_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,34 +30,32 @@
 from model_compression_toolkit.core.pytorch.mixed_precision.mixed_precision_wrapper import PytorchMixedPrecisionWrapper
 
 
 class MixedPrecisionPyTorchModel(PytorchModel):
 
     def __init__(self,
                  graph: common.Graph,
-                 append2output=None,
-                 fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO):
+                 append2output=None):
         """
 
         Args:
             graph: Graph to build its corresponding Pytorch model.
             append2output: List of nodes or OutTensor objects.
-            fw_info: Framework information (e.g., mapping from layers to their attributes to quantize).
         """
 
         super().__init__(graph,
-                         append2output,
-                         fw_info)
+                         append2output)
 
 
     def _add_modules(self):
         configurable_nodes = self.graph.get_configurable_sorted_nodes()
         for n in self.node_sort:
             if n in configurable_nodes:
-                self.add_module(n.name, PytorchMixedPrecisionWrapper(n, self.fw_info))
+                self.add_module(n.name, PytorchMixedPrecisionWrapper(n,
+                                                                     DEFAULT_PYTORCH_INFO))
             else:
                 if not isinstance(n, FunctionalNode):
                     self.add_module(n.name, node_builder(n))
 
     def _quantize_node_activations(self,
                                    node: BaseNode,
                                    input_tensors: List[torch.Tensor]) -> List[torch.Tensor]:
@@ -125,9 +123,8 @@
     def build_model(self) -> Tuple[PytorchModel, UserInformation]:
         """
         Build a PyTorch float model and return it.
         Returns: Float PyTorch model and user information.
 
         """
         return MixedPrecisionPyTorchModel(self.graph,
-                                          self.append2output,
-                                          self.fw_info), self.graph.user_info
+                                          self.append2output), self.graph.user_info
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/model_gradients.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/pytorch_model_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from abc import abstractmethod
+from functools import partial
 from typing import Tuple, Any, Dict, List, Union, Callable
 
 import torch
 from networkx import topological_sort
 
 from model_compression_toolkit.core import FrameworkInfo
 from model_compression_toolkit.core import common
@@ -26,14 +27,15 @@
 from model_compression_toolkit.core.common.graph.functional_node import FunctionalNode
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.pytorch.back2framework.instance_builder import node_builder, identity_wrapper
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.core.pytorch.reader.node_holders import DummyPlaceHolder, BufferHolder
 from model_compression_toolkit.core.pytorch.utils import get_working_device
 from model_compression_toolkit.core.pytorch.constants import BUFFER
+from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER
 
 
 def _build_input_tensors_list(node: BaseNode,
                               graph: Graph,
                               inputs: Tuple[Any],
                               node_to_output_tensors_dict: Dict[BaseNode, List]) -> List[List]:
     """
@@ -62,44 +64,44 @@
     return input_tensors
 
 
 def _run_operation(n: BaseNode,
                    input_tensors: List,
                    op_func: Any,
                    quantize_node_activation_fn,
-                   is_wrapped: bool) -> Tuple[Union[List,torch.Tensor], Union[List,torch.Tensor]]:
+                   use_activation_quantization: bool) -> Tuple[Union[List, torch.Tensor], Union[List, torch.Tensor]]:
     """
     Applying the layer (op_func) to the input tensors (input_tensors).
     If quantized is set to True, and the layer's corresponding node (n) has quantization
     attributes, an additional fake-quantization node is built and appended to the layer.
 
     Args:
         n: The corresponding node of the layer it runs.
         input_tensors: List of Pytorch tensors that are the layer's inputs.
         op_func: Module/functional to apply to the input tensors.
         quantize_node_activation_fn: quantization function
-        is_wrapped : Flag to indicate if layer is already quantization wrapped so no activation is needed
+        use_activation_quantization: Flag to indicate if we have an activation function.
     Returns:
         A tuple of Pytorch tensors. The Module/functional output tensors after applying the
         Module/functional to the input tensors.
     """
 
     op_call_args = n.op_call_args if isinstance(n, FunctionalNode) else []
     functional_kwargs = n.op_call_kwargs if isinstance(n, FunctionalNode) else {}
     if isinstance(n, FunctionalNode) and n.inputs_as_list:
         out_tensors_of_n_float = op_func(input_tensors, *op_call_args, **functional_kwargs)
     else:
         out_tensors_of_n_float = op_func(*input_tensors + op_call_args, **functional_kwargs)
 
     # Add a fake quant node if the node has an activation threshold.
     out_tensors_of_n = out_tensors_of_n_float
-    if n.is_activation_quantization_enabled() and not is_wrapped:
+    if use_activation_quantization:
         if isinstance(out_tensors_of_n_float, list):
             out_tensors_of_n_float = torch.cat(out_tensors_of_n_float, dim=0)
-        out_tensors_of_n = quantize_node_activation_fn(n, out_tensors_of_n_float)
+        out_tensors_of_n = quantize_node_activation_fn(out_tensors_of_n_float)
 
     return out_tensors_of_n, out_tensors_of_n_float
 
 
 def _find_by_node_name(node_to_output_tensors_dict: dict, node_name: str):
     """
     Args:
@@ -139,37 +141,49 @@
     """
     Class for reconstructing a Pytorch model from a graph
     """
 
     def __init__(self,
                  graph: Graph,
                  append2output: List[Any] = None,
-                 fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO,
                  return_float_outputs: bool = False,
-                 wrapper: Callable = identity_wrapper):
+                 wrapper: Callable = None,
+                 get_activation_quantizer_holder_fn: Callable = None):
         """
         Construct a Pytorch model.
 
         Args:
             graph: Graph to build its corresponding Pytorch model.
             append2output: List of nodes or OutTensor objects.
-            fw_info: Framework information (e.g., mapping from layers to their attributes to quantize).
             return_float_outputs: Whether the model returns float tensors or not.
             wrapper: A function wrapper Pytorch Layers.
+            get_activation_quantizer_holder_fn: Function to retrieve a quantization holder for a node.
+
         """
         super(PytorchModel, self).__init__()
         self.graph = graph
         self.node_sort = list(topological_sort(graph))
-        self.nodes_dict = {}
+        self.node_to_activation_quantization_holder = {}
         self.append2output = append2output
         self.return_float_outputs = return_float_outputs
-        self.fw_info = fw_info
         self.wrapper = wrapper
+        self.get_activation_quantizer_holder = get_activation_quantizer_holder_fn
         self._add_modules()
 
+    # todo: Move to parent class BaseModelBuilder
+    @property
+    def use_activation_holder_during_model_building(self) -> bool:
+        """
+        Returns: Whether or not the model builder uses a PytorchActivationQuantizationHolder during
+        model building (by adding it as a module when converting the graph to a Pytorch model).
+        If so - the model builder expects the activation quantizers not to be wrapped
+        in a PytorchQuantizeWrapper.
+        """
+        return self.get_activation_quantizer_holder is not None
+
     @abstractmethod
     def _quantize_node_activations(self,
                                    node: BaseNode,
                                    input_tensors: List[torch.Tensor]) -> List[torch.Tensor]:
         """
         Quantize node's activation given input tensors.
 
@@ -180,60 +194,92 @@
         Returns:
             Output of the node.
 
         """
         raise NotImplemented(f'{self.__class__.__name__} '
                              f'have to implement a method for quantization activation nodes.')  # pragma: no cover
 
+    def wrap(self, node):
+        """
+        Wraps a node operation with a wrapper, if one is available.
+
+        Args:
+            node: node to wrap its operation.
+
+        Returns: the node's operation. If a wrapper is available, the operation is wrapped.
+        """
+        if isinstance(node, FunctionalNode):
+            if self.wrapper is None:
+                node_op = node.type
+            else:
+                node_op = self.wrapper(node, node.type)
+        else:
+            if self.wrapper is None or node.type == BufferHolder:
+                node_op = node_builder(node)
+            else:
+                node_op = self.wrapper(node, node_builder(node))
+        return node_op
+
     def _add_modules(self):
-        for n in self.node_sort:
-            if isinstance(n, FunctionalNode):
+        """
+        Build and add the modules and functional nodes from node_sort list as attributes to PytorchModel
+        """
+        for node in self.node_sort:
+            node_op = self.wrap(node)
+            if isinstance(node, FunctionalNode):
                 # for functional layers
-                setattr(self, n.name, self.wrapper(n, n.type))
+                setattr(self, node.name, node_op)
             else:
-                if n.type == BufferHolder:
-                    self.add_module(n.name, node_builder(n))
-                    self.get_submodule(n.name). \
-                        register_buffer(n.name, torch.Tensor(n.get_weights_by_keys(BUFFER)).to(get_working_device()))
-                else:
-                    self.add_module(n.name, self.wrapper(n, node_builder(n)))
+                self.add_module(node.name, node_op)
+                if node.type == BufferHolder:
+                    self.get_submodule(node.name). \
+                        register_buffer(node.name,
+                                        torch.Tensor(node.get_weights_by_keys(BUFFER)).to(get_working_device()))
+
+            # Add activation quantization modules if an activation holder is configured for this node
+            if node.is_activation_quantization_enabled() and self.get_activation_quantizer_holder is not None:
+                activation_quantizer_holder = self.get_activation_quantizer_holder(node)
+                if activation_quantizer_holder is not None:
+                    self.add_module(node.name + '_' + ACTIVATION_HOLDER_QUANTIZER, activation_quantizer_holder)
+                    self.node_to_activation_quantization_holder.update(
+                        {node.name: node.name + '_' + ACTIVATION_HOLDER_QUANTIZER})
 
     def forward(self,
                 *args: Any) -> Any:
         """
         Args:
             args: argument input tensors to model.
         Returns:
             torch Tensor/s which is/are the output of the model logic.
         """
         node_to_output_tensors_dict = dict()
         node_to_output_tensors_dict_float = dict()
         configurable_nodes = self.graph.get_configurable_sorted_nodes_names()
-        for n in self.node_sort:
-            input_tensors = _build_input_tensors_list(n,
+        for node in self.node_sort:
+            input_tensors = _build_input_tensors_list(node,
                                                       self.graph,
                                                       args,
                                                       node_to_output_tensors_dict)
 
-            op_func = self._get_op_func(n, configurable_nodes)
+            op_func = self._get_op_func(node, configurable_nodes)
+            use_activation_quantization, activation_quantization_fn = self._get_activation_quantization_fn(node)
 
             # Run node operation and fetch outputs
-            out_tensors_of_n, out_tensors_of_n_float = _run_operation(n,
+            out_tensors_of_n, out_tensors_of_n_float = _run_operation(node,
                                                                       input_tensors,
                                                                       op_func=op_func,
-                                                                      quantize_node_activation_fn=self._quantize_node_activations,
-                                                                      is_wrapped=self.wrapper is not identity_wrapper)
+                                                                      quantize_node_activation_fn=activation_quantization_fn,
+                                                                      use_activation_quantization=use_activation_quantization)
 
             if isinstance(out_tensors_of_n, list):
-                node_to_output_tensors_dict.update({n: out_tensors_of_n})
-                node_to_output_tensors_dict_float.update({n: out_tensors_of_n_float})
+                node_to_output_tensors_dict.update({node: out_tensors_of_n})
+                node_to_output_tensors_dict_float.update({node: out_tensors_of_n_float})
             else:
-                node_to_output_tensors_dict.update({n: [out_tensors_of_n]})
-                node_to_output_tensors_dict_float.update({n: [out_tensors_of_n_float]})
-
+                node_to_output_tensors_dict.update({node: [out_tensors_of_n]})
+                node_to_output_tensors_dict_float.update({node: [out_tensors_of_n_float]})
 
         if self.append2output:
             outputs = _generate_outputs(self.append2output,
                                         node_to_output_tensors_dict_float if self.return_float_outputs else node_to_output_tensors_dict)
         else:
             outputs = _generate_outputs([ot.node for ot in self.graph.get_outputs()],
                                         node_to_output_tensors_dict_float if self.return_float_outputs else node_to_output_tensors_dict)
@@ -252,46 +298,72 @@
             configurable_nodes_names: A list of names of configurable nodes in the quantized model.
 
         Returns: Module/functional to apply to the input tensors.
 
         """
         return getattr(self, node.name)
 
+    def _get_activation_quantization_fn(self, node) -> Tuple[bool, bool, Callable]:
+        """
+        Get activation quantization parameters for this node.
+
+        Args:
+            node: Node from which to extract the activation quantization parameters.
+
+        Returns: Flag to indicate if we quantize activations, flag to indicate if we quantize activations
+        using a quantization holder and a quantization function to use for the node's activations.
+        """
+        activation_quantization_holder = self.node_to_activation_quantization_holder.get(node.name)
+        use_activation_quantization = node.is_activation_quantization_enabled()
+        if use_activation_quantization:
+            if activation_quantization_holder is None:
+                activation_quantization_fn = partial(self._quantize_node_activations, node)
+                use_activation_quantization = self.wrapper is None
+            else:
+                activation_quantization_fn = getattr(self, activation_quantization_holder)
+        else:
+            activation_quantization_fn = None
+        return use_activation_quantization, activation_quantization_fn
+
 
 class PyTorchModelBuilder(BaseModelBuilder):
     """
     Builder of PyTorch models.
     """
 
     def __init__(self,
                  graph: common.Graph,
                  append2output=None,
                  fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO,
                  return_float_outputs: bool = False,
-                 wrapper: Callable = identity_wrapper):
+                 wrapper: Callable = None,
+                 get_activation_quantizer_holder_fn: Callable = None):
         """
 
         Args:
             graph: Graph to build the model from.
             append2output: Nodes to append to model's output.
             fw_info: Information about the specific framework of the model that is built.
             return_float_outputs: Whether the model returns float tensors or not.
             wrapper: A function wrapper Pytorch Layers.
+            get_activation_quantizer_holder_fn: Function to retrieve a quantization holder for a node.
         """
 
         super().__init__(graph,
                          append2output,
                          fw_info,
                          return_float_outputs)
 
         self.wrapper = wrapper
+        self.get_activation_quantizer_holder_fn = get_activation_quantizer_holder_fn
 
     def build_model(self) -> Tuple[PytorchModel, UserInformation]:
         """
         Build a PyTorch model and return it.
         Returns: Pytorch model and user information.
 
         """
         return PytorchModel(self.graph,
                             self.append2output,
                             return_float_outputs=self.return_float_outputs,
-                            wrapper=self.wrapper), self.graph.user_info
+                            wrapper=self.wrapper,
+                            get_activation_quantizer_holder_fn=self.get_activation_quantizer_holder_fn), self.graph.user_info
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/quantized_layer_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantization_wrapper/wrapper_quantize_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/back2framework/quantized_model_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,27 +29,24 @@
 class QuantizedPyTorchModel(PytorchModel):
     """
     Quantized PyTorch model.
     """
 
     def __init__(self,
                  graph: common.Graph,
-                 append2output=None,
-                 fw_info: FrameworkInfo = DEFAULT_PYTORCH_INFO):
+                 append2output=None):
         """
 
         Args:
             graph: Graph to build its corresponding Pytorch model.
             append2output: List of nodes or OutTensor objects.
-            fw_info: Framework information (e.g., mapping from layers to their attributes to quantize).
         """
 
         super().__init__(graph,
-                         append2output,
-                         fw_info)
+                         append2output)
 
     def _quantize_node_activations(self,
                                    node: BaseNode,
                                    input_tensors: List[torch.Tensor]) -> List[torch.Tensor]:
         """
         Quantize node's activation given input tensors.
 
@@ -92,9 +89,8 @@
     def build_model(self) -> Tuple[PytorchModel, UserInformation]:
         """
         Build a PyTorch quantized model and return it.
         Returns: Quantized PyTorch model and user information.
 
         """
         return QuantizedPyTorchModel(self.graph,
-                                     self.append2output,
-                                     self.fw_info), self.graph.user_info
+                                     self.append2output), self.graph.user_info
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/default_framework_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/default_framework_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_folding.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_reconstruction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/batchnorm_refusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/const_holder_conv.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/linear_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/multi_head_attention_decomposition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/permute_call_method.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/relu_bound_to_power_of_2.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/reshape_with_static_shapes.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/residual_collapsing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/scale_equalization.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/shift_negative_activation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/softmax_shift.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/virtual_activation_weights_composition.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/graph_substitutions/substitutions/weights_activation_split.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/kpi_data_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/kpi_data_facade.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/mixed_precision_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/mixed_precision/set_layer_to_bitwidth.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_implementation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/pytorch_node_prior_info.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/fake_quant_builder.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/quantizer/lut_fake_quant.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/graph_builders.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/graph_builders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/node_holders.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/node_holders.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/reader/reader.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/reader/reader.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/statistics_correction/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/statistics_correction/apply_second_moment_correction.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/pytorch/utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/core/runner.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/core/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/fw_agonstic/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/fw_agonstic/exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/base_keras_exporter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/keras/keras_export_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/fakely_quant_tflite_exporter.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,63 +8,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from enum import Enum
-from typing import Callable, Dict
+import os
+import tempfile
+from typing import Callable
 
-from model_compression_toolkit.logger import Logger
-from model_compression_toolkit.constants import FOUND_TF
-
-
-class KerasExportMode(Enum):
-    FAKELY_QUANT = 0
+import keras.models
+import tensorflow as tf
 
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
+from model_compression_toolkit.trainable_infrastructure.keras.load_model import keras_load_quantized_model
 
-if FOUND_TF:
-    import keras
-    from model_compression_toolkit.exporter.model_wrapper.keras.validate_layer import is_keras_layer_exportable
-    from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
 
-    def keras_export_model(model: keras.models.Model,
-                           save_model_path: str,
-                           is_layer_exportable_fn: Callable = is_keras_layer_exportable,
-                           mode: KerasExportMode = KerasExportMode.FAKELY_QUANT) -> Dict[str, type]:
+class FakelyQuantTFLiteExporter(FakelyQuantKerasExporter):
+    """
+    Exporter for fakely-quant TFLite models.
+    The exporter expects to receive an exportable model (where each layer's full quantization parameters
+    can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
+    format) and fake-quant layers for the activations.
+    """
+
+    def __init__(self,
+                 model: keras.models.Model,
+                 is_layer_exportable_fn: Callable,
+                 save_model_path: str):
         """
-        Export a Keras quantized model to h5 model.
-        The model will be saved to the path in save_model_path.
-        Mode can be used for different exported files. Currently, keras_export_model
-        supports KerasExportMode.FAKELY_QUANT (where weights and activations are
-        float fakely-quantized values).
 
         Args:
             model: Model to export.
             is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
-            mode: Mode to export the model according to.
-            save_model_path: Path to save the model.
+            save_model_path: Path to save the exported model.
+        """
+        super().__init__(model,
+                         is_layer_exportable_fn,
+                         save_model_path)
 
-        Returns:
-            Custom objects dictionary needed to load the model.
+        self.exported_model = None
 
+    def export(self):
         """
+        Convert an exportable (fully-quantized) Keras model to a fakely-quant TFLite model
+        (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
 
-        if mode == KerasExportMode.FAKELY_QUANT:
-            exporter = FakelyQuantKerasExporter(model,
-                                                is_layer_exportable_fn,
-                                                save_model_path)
-
-        else:
-            Logger.critical(
-                f'Unsupported mode was used {mode.name} to '
-                f'export Keras model. Please see API for supported modes.')  # pragma: no cover
-
-        exporter.export()
-
-        return exporter.get_custom_objects()
-else:
-    def keras_export_model(*args, **kwargs):
-        Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
-                     'when using keras_export_model. '
-                     'Could not find some or all of TensorFlow packages.')  # pragma: no cover
+        """
+        # Use Keras exporter to quantize model's weights before converting it to TFLite.
+        # Since exporter saves the model, we use a tmp path for saving, and then we delete it.
+        _, tmp_h5_file = tempfile.mkstemp('.h5')
+        custom_objects = FakelyQuantKerasExporter(self.model,
+                                                  self.is_layer_exportable_fn,
+                                                  tmp_h5_file).export()
+
+        model = keras_load_quantized_model(tmp_h5_file)
+        os.remove(tmp_h5_file)
+
+        self.exported_model = tf.lite.TFLiteConverter.from_keras_model(model).convert()
+        Logger.info(f'Exporting FQ tflite model to: {self.save_model_path}')
+        with open(self.save_model_path, 'wb') as f:
+            f.write(self.exported_model)
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/base_pytorch_exporter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_torchscript_pytorch_exporter.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,36 +8,68 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
 from typing import Callable
 
 import torch.nn
 
-from model_compression_toolkit.exporter.model_exporter.fw_agonstic.exporter import Exporter
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
+from model_compression_toolkit.exporter.model_exporter.pytorch.base_pytorch_exporter import BasePyTorchExporter
 
 
-class BasePyTorchExporter(Exporter):
+class FakelyQuantTorchScriptPyTorchExporter(BasePyTorchExporter):
     """
-    Base PyTorch exporter class.
+    Exporter for fakely-quant PyTorch models.
+    The exporter expects to receive an exportable model (where each layer's full quantization parameters
+    can be retrieved), and convert it into a fakely-quant model (namely, weights that are in fake-quant
+    format) and fake-quant layers for the activations.
     """
 
     def __init__(self,
                  model: torch.nn.Module,
                  is_layer_exportable_fn: Callable,
                  save_model_path: str,
                  repr_dataset: Callable):
         """
+
         Args:
             model: Model to export.
             is_layer_exportable_fn: Callable to check whether a layer can be exported or not.
             save_model_path: Path to save the exported model.
             repr_dataset: Representative dataset (needed for creating torch script).
-
         """
+
         super().__init__(model,
                          is_layer_exportable_fn,
-                         save_model_path)
-        self.repr_dataset = repr_dataset
+                         save_model_path,
+                         repr_dataset)
+
+    def export(self) -> None:
+        """
+        Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
+        (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
+
+        Returns:
+            Fake-quant PyTorch model.
+        """
+        for layer in self.model.children():
+            self.is_layer_exportable_fn(layer)
+
+        self._substitute_fully_quantized_model()
+
+        torch_traced = torch.jit.trace(self.model,
+                                       to_torch_tensor(next(self.repr_dataset())),
+                                       check_trace=True)
+
+        self.exported_model = torch.jit.script(torch_traced)
+
+        Logger.info(f"Exporting PyTorch torch script Model: {self.save_model_path}")
+
+        torch.jit.save(self.exported_model, self.save_model_path)
+
+
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/pytorch/fakely_quant_onnx_pytorch_exporter.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,17 +17,14 @@
 import torch.nn
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.exporter.model_exporter.pytorch.base_pytorch_exporter import BasePyTorchExporter
 from packaging import version
 
-from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import LAYER
-
 # ONNX opset version 16 is supported from PyTorch 1.12
 if version.parse(torch.__version__) < version.parse("1.12"):
     OPSET_VERSION = 15
 else:
     OPSET_VERSION = 16
 
 
@@ -64,29 +61,21 @@
         Convert an exportable (fully-quantized) PyTorch model to a fakely-quant model
         (namely, weights that are in fake-quant format) and fake-quant layers for the activations.
 
         Returns:
             Fake-quant PyTorch model.
         """
         for layer in self.model.children():
-            assert self.is_layer_exportable_fn(layer), f'Layer {layer.name} is not exportable.'
+            self.is_layer_exportable_fn(layer)
 
-        model_input = to_torch_tensor(next(self.repr_dataset())[0])
+        self._substitute_fully_quantized_model()
 
         Logger.info(f"Exporting PyTorch fake quant onnx model: {self.save_model_path}")
 
-        # Replace float weight with wrapped quantized weights
-        for layer in self.model.modules():
-            if isinstance(layer, PytorchQuantizationWrapper):
-                for name in layer.weights_quantizers.keys():
-                    quantized_weight = torch.nn.Parameter(layer.get_quantized_weights()[name]).detach()
-                    linear_layer = getattr(layer, LAYER)
-                    delattr(linear_layer, name)
-                    setattr(linear_layer, name, torch.nn.Parameter(quantized_weight))
-                layer.weights_quantizers = {}
+        model_input = to_torch_tensor(next(self.repr_dataset())[0])
 
         torch.onnx.export(self.model,
                           model_input,
                           self.save_model_path,
                           opset_version=OPSET_VERSION,
                           verbose=False,
                           input_names=['input'],
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_exporter/tflite/int8_tflite_exporter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_exporter/keras/int8_tflite_exporter.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,19 +18,17 @@
 import keras.models
 import numpy as np
 import tensorflow as tf
 from keras import Sequential
 from keras.layers import Dense, Conv2D, Reshape
 from keras.models import clone_model
 
-from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.exporter.model_exporter.keras.fakely_quant_keras_exporter import FakelyQuantKerasExporter
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
-    constants as keras_inferable_constants
+from mct_quantizers import constants as keras_inferable_constants, KerasQuantizationWrapper
 
 BIAS_INITIALIZER = 'bias_initializer'
 BIAS_REGULARIZER = 'bias_regularizer'
 BIAS_CONSTRAINT = 'bias_constraint'
 ACTIVITY_REGULARIZER = 'activity_regularizer'
 KERNEL_INITIALIZER = 'kernel_initializer'
 KERNEL_REGULARIZER = 'kernel_regularizer'
@@ -46,14 +44,15 @@
 UNITS = 'units'
 PAD_VALID = 'valid'
 KERNEL = 'kernel'
 
 CONV_KERNEL_CHANNEL_AXIS = 3
 CONV_INPUT_CHANNELS_DIM = 4
 
+
 class INT8TFLiteExporter(FakelyQuantKerasExporter):
     """
     Exporter for INT8 TFLite models.
     The exporter expects to receive an exportable model (where each layer's full quantization parameters
     can be retrieved), and convert it into a quantized model where weights and activations are represented
     as integer data type.
     """
@@ -71,15 +70,15 @@
         """
         super().__init__(model,
                          is_layer_exportable_fn,
                          save_model_path)
 
         self.exported_model = None
 
-    def _get_pointwise_layer_to_replace_dense(self, wrapped_layer: qi.KerasQuantizationWrapper) -> keras.layers.Layer:
+    def _get_pointwise_layer_to_replace_dense(self, wrapped_layer: KerasQuantizationWrapper) -> keras.layers.Layer:
         # First we create a pointwise configuration based on the Dense layer's configuration
         dense_cfg = wrapped_layer.layer.get_config()
 
         # List of pw attributes that should be taken from the dense layer as they are.
         pw_attr_list = [LAYER_NAME, ACTIVATION, USE_BIAS, BIAS_CONSTRAINT,
                         BIAS_INITIALIZER, BIAS_REGULARIZER, TRAINABLE, ACTIVITY_REGULARIZER,
                         KERNEL_INITIALIZER, KERNEL_REGULARIZER, KERNEL_CONSTRAINT]
@@ -90,15 +89,15 @@
         pw_cfg.update({KERNEL_SIZE: (1, 1),
                        STRIDES: (1, 1),
                        PADDING: PAD_VALID,
                        FILTERS: dense_cfg[UNITS]})
 
         # Create the point-wise layer
         pw_layer = Conv2D(**pw_cfg)
-        pw_layer.build(wrapped_layer.layer.input_shape)
+        pw_layer.build(wrapped_layer.input_shape)
 
         # Create and set the point-wise weights to assign
         dense_kernel = wrapped_layer.layer.kernel
         pw_weights = []
         pw_kernel = np.reshape(wrapped_layer.get_weights()[0],
                                (1, 1, dense_kernel.get_shape()[0], dense_cfg[UNITS]))
 
@@ -106,68 +105,70 @@
         if wrapped_layer.layer.use_bias:
             pw_bias = wrapped_layer.get_weights()[2]
             pw_weights.append(pw_bias)
 
         pw_layer.set_weights(pw_weights)
 
         # Now that we have the point-wise to replace the dense layer,
-        # we need to wrap it using qi.KerasQuantizationWrapper with a new
+        # we need to wrap it using KerasQuantizationWrapper with a new
         # relevant quantizers.
         # Create new kernel quantizer
         pw_kernel_quantizer_cfg = wrapped_layer.weights_quantizers[KERNEL].get_config()
 
         # In Conv2D channel axis is 3 and not 1 as in Dense
         pw_kernel_quantizer_cfg[keras_inferable_constants.CHANNEL_AXIS] = CONV_KERNEL_CHANNEL_AXIS
 
         # Unquantized weight to conv layer has 4 dimensions (unlike dense which varies)
         pw_kernel_quantizer_cfg[keras_inferable_constants.INPUT_RANK] = CONV_INPUT_CHANNELS_DIM
 
-        assert isinstance(pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD], np.ndarray), f'Expected to find threshold which is a numpy array, but found: {type(pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD])}'
-        pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD] = list(pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD])
+        assert isinstance(pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD],
+                          list), f'Expected to find threshold which is a list, but found: {type(pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD])}'
+        pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD] = list(
+            pw_kernel_quantizer_cfg[keras_inferable_constants.THRESHOLD])
 
         # Now that we have the point-wise quantizer we can instantiate it
         quantizer_class = type(wrapped_layer.weights_quantizers[KERNEL])
         pw_quantizer = quantizer_class(**pw_kernel_quantizer_cfg)
         pw_weights_quantizers = copy.deepcopy(wrapped_layer.weights_quantizers)
         pw_weights_quantizers[KERNEL] = pw_quantizer
 
         # Wrap pw with the new quantizers (the activation is not affected thus we take the Dense quantizers)
-        wrapped_pw = qi.KerasQuantizationWrapper(pw_layer,
-                                                 pw_weights_quantizers,
-                                                 wrapped_layer.activation_quantizers)
+        wrapped_pw = KerasQuantizationWrapper(pw_layer,
+                                              pw_weights_quantizers)
 
         # Compute the shape that the input to the new layer should be reshaped into
         # Example: Dense kernel with the following shape (3, 20) expects to have input with the
         # next dimensions (BATCH_SIZE, x0, x1, ..., xn, 20).
         # Conv layer expects 4-rank input. Thus, the input is reshaped to (BATCH_SIZE, 1, x0*x1*...*xn, 20)
-        dim = wrapped_layer.layer.input_shape[1:-1]
+        dim = wrapped_layer.input_shape[1:-1]
         target_shape = (1, int(np.prod(dim))) + (dense_kernel.get_shape()[0],)
 
         return Sequential([
             Reshape(target_shape=target_shape),
             wrapped_pw,
-            Reshape(wrapped_layer.layer.output_shape[1:])
+            Reshape(wrapped_layer.output_shape[1:])
         ])
 
     def export(self) -> None:
         """
         Export a fully quantized model to its int8 tflite model.
         """
 
-        def _substitute_model(wrapped_layer: qi.KerasQuantizationWrapper) -> keras.layers.Layer:
+        def _substitute_model(layer_to_substitue: keras.layers.Layer) -> keras.layers.Layer:
             assert self.is_layer_exportable_fn(
-                wrapped_layer), f'Layer {wrapped_layer.get_config()} did not pass validation'
+                layer_to_substitue), f'Layer {layer_to_substitue.get_config()} did not pass validation'
 
             # In order to support dense quantization using per-channel quantization (which is
             # unsupported in TFLITE int models) we substitute each dense layer to its equivalent
             # point-wise convolution.
-            if isinstance(wrapped_layer.layer, Dense):
-                return self._get_pointwise_layer_to_replace_dense(wrapped_layer)
+            if isinstance(layer_to_substitue, KerasQuantizationWrapper):
+                if isinstance(layer_to_substitue.layer, Dense):
+                    return self._get_pointwise_layer_to_replace_dense(layer_to_substitue)
 
-            return wrapped_layer
+            return layer_to_substitue
 
         # Transform the model to a new model that can be converted to int8 models.
         # For example: replace dense layers with point-wise layers (to support per-channel quantization)
         self.transformed_model = clone_model(self.model,
                                              clone_function=_substitute_model)
 
         # Convert model to int8 representation
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,18 @@
 from typing import Dict, Any
 
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.constants import THRESHOLD, RANGE_MIN, RANGE_MAX, SIGNED, CLUSTER_CENTERS, SCALE_PER_CHANNEL
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import get_inferable_quantizer_class
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import constants as qi_keras_consts
+from mct_quantizers import QuantizationTarget
+from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
+from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
+from mct_quantizers import constants as qi_keras_consts
 
 def get_inferable_quantizer_kwargs(node: BaseNode,
                                    quantization_target: QuantizationTarget) -> Dict[str, Any]:
     """
     Get the quantization parameters for an inferable quantizer.
     Args:
         node: The node for which the quantizer is being created.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/validate_layer.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Any
 
-
-from model_compression_toolkit.logger import Logger
+from mct_quantizers import BaseInferableQuantizer, KerasActivationQuantizationHolder
 from model_compression_toolkit.constants import FOUND_TF
-
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import BaseInferableQuantizer
-
+from model_compression_toolkit.logger import Logger
 
 if FOUND_TF:
+    from keras.engine.base_layer import Layer
     from keras.engine.input_layer import InputLayer
-    from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
+    from mct_quantizers import KerasQuantizationWrapper
 
     def is_keras_layer_exportable(layer: Any) -> bool:
         """
         Check whether a Keras layer is a valid exportable layer or not.
 
         Args:
             layer: Keras layer to check if considered to be valid for exporting.
@@ -35,48 +33,42 @@
         Returns:
             Check whether a Keras layer is a valid exportable layer or not.
         """
         # Keras Input layers are not wrapped
         if isinstance(layer, InputLayer):
             return True
 
-        valid_layer = isinstance(layer, KerasQuantizationWrapper)
+        valid_layer = isinstance(layer, Layer)
         if not valid_layer:
             Logger.error(
-                f'Exportable layer must be wrapped using KerasQuantizationWrapper, but layer {layer.name} is of type '
+                f'Exportable layer must be a Keras layer, but layer {layer.name} is of type '
                 f'{type(layer)}') # pragma: no cover
 
-        valid_weights_quantizers = isinstance(layer.weights_quantizers, dict)
-        if not valid_weights_quantizers:
-            Logger.error(
-                f'KerasQuantizationWrapper must have a weights_quantizers but has a '
-                f'{type(layer.weights_quantizers)} object') # pragma: no cover
-
-        for _, weights_quantizer in layer.weights_quantizers.items():
-            if not isinstance(weights_quantizer, BaseInferableQuantizer):
+        if isinstance(layer, KerasQuantizationWrapper):
+            valid_weights_quantizers = isinstance(layer.weights_quantizers, dict)
+            if not valid_weights_quantizers:
                 Logger.error(
-                    f'weights_quantizer must be a BaseInferableQuantizer object but has a '
-                    f'{type(weights_quantizer)} object')  # pragma: no cover
+                    f'KerasQuantizationWrapper must have a weights_quantizers but has a '
+                    f'{type(layer.weights_quantizers)} object') # pragma: no cover
 
-        valid_activation_quantizers = isinstance(layer.activation_quantizers, list)
-        if not valid_activation_quantizers:
-            Logger.error(
-                f'KerasQuantizationWrapper must have a activation_quantizers list but has a '
-                f'{type(layer.activation_quantizers)} object') # pragma: no cover
+            if len(layer.weights_quantizers) == 0:
+                Logger.error(f'KerasQuantizationWrapper must have at least one weight quantizer, but found {len(layer.weights_quantizers)} quantizers. If layer is not quantized it should be a Keras layer.')
 
-        for activation_quantizers in layer.activation_quantizers:
-            if not isinstance(activation_quantizers, BaseInferableQuantizer):
-                Logger.error(
-                    f'activation_quantizers must be a BaseInferableQuantizer object but has a '
-                    f'{type(activation_quantizers)} object')  # pragma: no cover
+            for _, weights_quantizer in layer.weights_quantizers.items():
+                if not isinstance(weights_quantizer, BaseInferableQuantizer):
+                    Logger.error(
+                        f'weights_quantizer must be a BaseInferableQuantizer object but has a '
+                        f'{type(weights_quantizer)} object')  # pragma: no cover
 
-        quantizers = layer.activation_quantizers + list(layer.weights_quantizers.values())
-        is_valid_quantizers = all([isinstance(x, BaseInferableQuantizer) for x in quantizers])
-        if not is_valid_quantizers:
-            Logger.error(f'Found a quantizer that is not of type BaseInferableQuantizer') # pragma: no cover
+        if isinstance(layer, KerasActivationQuantizationHolder):
+            if not isinstance(layer.activation_holder_quantizer, BaseInferableQuantizer):
+                Logger.error(
+                    f'activation quantizer in KerasActivationQuantizationHolder'
+                    f' must be a BaseInferableQuantizer object but has a '
+                    f'{type(layer.activation_holder_quantizer)} object')  # pragma: no cover
 
         return True
 else:
     def is_keras_layer_exportable(*args, **kwargs):  # pragma: no cover
         Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
                      'when using is_keras_layer_exportable. '
                      'Could not find Tensorflow package.')
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/fully_quantized_model_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,54 +9,66 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
+import operator
 
-from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common import Graph
-from model_compression_toolkit.constants import FOUND_TORCH
-from model_compression_toolkit.logger import Logger
-
-if FOUND_TORCH:
-    import torch
-    from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
-    from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.node_to_quantizers import \
-        get_quantization_quantizers
-
-    def fully_quantized_wrapper(node: common.BaseNode, module: torch.nn.Module) -> qi.PytorchQuantizationWrapper:
-        """
-        A function which takes a computational graph node and a pytorch module and
-        perform the quantization wrapping
-
-        Args:
-            node: A node of mct graph.
-            module: A Pytorch module
-
-        Returns: Wrapped layer
-
-        """
-        weight_quantizers, activation_quantizers = get_quantization_quantizers(node)
-        wrapped_layer = qi.PytorchQuantizationWrapper(module, weight_quantizers, activation_quantizers)
-        return wrapped_layer
-
-
-    def get_exportable_pytorch_model(graph: Graph):
-        """
-        Convert graph to fully quantized PyTorch model.
-
-        Args:
-            graph: Graph to convert to a PyTorch model.
-
-        Returns:
-            Fully quantized PyTorch model.
-        """
-        return PyTorchModelBuilder(graph=graph,
-                                   wrapper=fully_quantized_wrapper).build_model()
-else:
-    def get_exportable_pytorch_model(*args, **kwargs):  # pragma: no cover
-        Logger.error('Installing torch is mandatory '
-                     'when using get_exportable_pytorch_model. '
-                     'Could not find PyTorch package.')
+import torch
+from torch import flatten, reshape, split, unsqueeze, dropout, chunk
+from torch.nn import Conv2d, BatchNorm2d
+from torch.nn import Dropout, Flatten
+from torch.nn import ReLU, ReLU6
+from torch.nn.functional import relu, relu6
+
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1.tp_model import get_tp_model
+import model_compression_toolkit as mct
+from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1 import __version__ as TPC_VERSION
+
+tp = mct.target_platform
+
+
+def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
+    """
+    get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
+    Returns: a Pytorch TargetPlatformCapabilities object for the given TargetPlatformModel.
+    """
+    default_tp_model = get_tp_model()
+    return generate_pytorch_tpc(name='default_pytorch_tpc', tp_model=default_tp_model)
+
+
+def generate_pytorch_tpc(name: str, tp_model: tp.TargetPlatformModel):
+    """
+    Generates a TargetPlatformCapabilities object with default operation sets to layers mapping.
+    Args:
+        name: Name of the TargetPlatformModel.
+        tp_model: TargetPlatformModel object.
+    Returns: a TargetPlatformCapabilities object for the given TargetPlatformModel.
+    """
+
+    pytorch_tpc = tp.TargetPlatformCapabilities(tp_model,
+                                                name=name,
+                                                version=TPC_VERSION)
+
+    with pytorch_tpc:
+        tp.OperationsSetToLayers("NoQuantization", [Dropout,
+                                                    Flatten,
+                                                    dropout,
+                                                    flatten,
+                                                    split,
+                                                    operator.getitem,
+                                                    reshape,
+                                                    unsqueeze,
+                                                    BatchNorm2d,
+                                                    chunk,
+                                                    torch.Tensor.size])
+
+        tp.OperationsSetToLayers("Conv", [Conv2d])
+        tp.OperationsSetToLayers("AnyReLU", [torch.relu,
+                                             ReLU,
+                                             ReLU6,
+                                             relu,
+                                             relu6])
+
+    return pytorch_tpc
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from typing import Dict, Any
 
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.constants import THRESHOLD, SIGNED, RANGE_MIN, RANGE_MAX, \
     SCALE_PER_CHANNEL, CLUSTER_CENTERS
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
-    get_inferable_quantizer_class
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
-    constants as qi_inferable_quantizers_constants, BasePyTorchInferableQuantizer
+from mct_quantizers import QuantizationTarget
+from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
+from mct_quantizers import \
+    constants as qi_inferable_quantizers_constants
+from mct_quantizers.pytorch.quantizers import BasePyTorchInferableQuantizer
 import numpy as np
 
 
 def get_weights_inferable_quantizer_kwargs(node: BaseNode) -> Dict[str, Any]:
     # Get the weights quantization configuration for the node
     node_w_qc = node.final_weights_quantization_cfg
     quantization_method = node_w_qc.weights_quantization_method
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/pytorch/builder/node_to_quantizers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig, RoundingType, GradientPTQConfigV2
+from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig, RoundingType, GradientPTQConfigV2, GPTQHessianWeightsConfig
 from model_compression_toolkit.gptq.keras.quantization_facade import keras_gradient_post_training_quantization_experimental
 from model_compression_toolkit.gptq.keras.quantization_facade import get_keras_gptq_config
 from model_compression_toolkit.gptq.pytorch.quantization_facade import pytorch_gradient_post_training_quantization_experimental
 from model_compression_toolkit.gptq.pytorch.quantization_facade import get_pytorch_gptq_config
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
                  norm_weights: bool = True,
                  log_norm: bool = True,
                  scale_log_norm: bool = False,
                  hessians_n_iter: int = 50):
 
         """
         Initialize a GPTQHessianWeightsConfig.
+
         Args:
             hessians_num_samples (int): Number of samples to use for computing the Hessian-based weights.
             norm_weights (bool): Whether to normalize the returned weights (to get values between 0 and 1).
             log_norm (bool): Whether to use log normalization to the GPTQ Hessian-based weights.
             scale_log_norm (bool): Whether to scale the final vector of the Hessian weights.
             hessians_n_iter (int): Number of random iterations to run Hessian approximation for GPTQ weights.
         """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_framework_implementation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_framework_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_graph.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_graph.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/common/gptq_training.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/common/gptq_training.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,31 +15,31 @@
 import copy
 from abc import ABC, abstractmethod
 import numpy as np
 from typing import Callable, List, Any
 from model_compression_toolkit.gptq.common.gptq_config import GradientPTQConfig
 from model_compression_toolkit.core.common import Graph, BaseNode
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.gptq.common.gptq_constants import QUANT_PARAM_LEARNING_STR
+from model_compression_toolkit.gptq.common.gptq_framework_implementation import GPTQFrameworkImplemantation
 from model_compression_toolkit.gptq.common.gptq_graph import get_compare_points
 from model_compression_toolkit.core.common.model_builder_mode import ModelBuilderMode
 from model_compression_toolkit.logger import Logger
 
 
 class GPTQTrainer(ABC):
     """
     Abstract GPTQ training class for fine-tuning a quantized model
     """
 
     def __init__(self,
                  graph_float: Graph,
                  graph_quant: Graph,
                  gptq_config: GradientPTQConfig,
-                 fw_impl: FrameworkImplementation,
+                 fw_impl: GPTQFrameworkImplemantation,
                  fw_info: FrameworkInfo):
         """
         Build two models from a graph: A teacher network (float model) and a student network (quantized model).
         Use the dataset generator to pass images through the teacher and student networks to get intermediate
         layers outputs. Use the outputs to compute the observed loss and to back-propagate the error
         in the student network, to minimize it in the next similar steps.
         All parameters (such as number of iterations, optimizer, etc.) are in GradientPTQConfig.
@@ -256,15 +256,15 @@
         return replacement_outputs
 
 
 def gptq_training(graph_float: Graph,
                   graph_quant: Graph,
                   gptq_config: GradientPTQConfig,
                   representative_data_gen: Callable,
-                  fw_impl: FrameworkImplementation,
+                  fw_impl: GPTQFrameworkImplemantation,
                   fw_info: FrameworkInfo) -> Graph:
     """
     GPTQ training process using knowledge distillation with a teacher network (float model) and a student network (quantized model).
     Args:
         graph_float: Graph to build a float networks from.
         graph_quant: Graph to build a quantized networks from.
         gptq_config: GradientPTQConfig with parameters about the tuning process.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/gptq_keras_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_loss.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/gptq_training.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/gptq_training.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,26 +12,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Callable, List, Tuple, Union
 
 import tensorflow as tf
 from keras import Model
+from packaging import version
 from tensorflow.keras.layers import Layer
 from tqdm import tqdm
 
 # As from Tensorflow 2.6, keras is a separate package and some classes should be imported differently.
 from model_compression_toolkit.core.common.user_info import UserInformation
 from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
-from packaging import version
-
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.keras.quantizer.quantization_builder import quantization_builder
 from model_compression_toolkit.logger import Logger
-from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
+from mct_quantizers import KerasQuantizationWrapper, KerasActivationQuantizationHolder
 
 if version.parse(tf.__version__) < version.parse("2.6"):
     from tensorflow.python.keras.engine.base_layer import TensorFlowOpLayer
 else:
     from keras.engine.base_layer import TensorFlowOpLayer
 
 from model_compression_toolkit.core import common
@@ -41,15 +40,14 @@
 from model_compression_toolkit.gptq.keras.graph_info import get_weights_for_loss, get_gptq_trainable_parameters
 from model_compression_toolkit.gptq.keras.quantizer.regularization_factory import get_regularization
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 import numpy as np
 import copy
 from model_compression_toolkit.core.keras.constants import BIAS, USE_BIAS
-from model_compression_toolkit import quantizers_infrastructure as qi
 
 
 class KerasGPTQTrainer(GPTQTrainer):
     """
     Keras GPTQ training class for fine-tuning a quantized model
     """
 
@@ -110,16 +108,16 @@
         else:
             self.input_scale = self.gptq_user_info.input_scale
 
         self.weights_for_average_loss = self.compute_hessian_based_weights(representative_data_gen)
 
         self.reg_func = get_regularization(self.gptq_config, representative_data_gen)
 
-    def _is_gptq_applicable(self,
-                            node: common.BaseNode) -> bool:
+    def _is_gptq_weights_trainable(self,
+                                   node: common.BaseNode) -> bool:
         """
         A function for deciding if a layer should be fine-tuned during GPTQ.
 
         Args:
             node (BaseNode): Node for quantization decision
 
         Returns:
@@ -127,46 +125,73 @@
         """
 
         if node.is_weights_quantization_enabled() and not self.fw_info.is_kernel_op(node.type):
             Logger.error(f"GPTQ Error: Quantizing node {node.name} of type {node.type} "
                                 f"without a kernel isn't supported")
         return node.is_weights_quantization_enabled()
 
-    def gptq_wrapper(self, n: common.BaseNode, layer: Layer) -> Union[qi.KerasQuantizationWrapper, Layer]:
+    def gptq_wrapper(self,
+                     n: common.BaseNode,
+                     layer: Layer) -> Union[KerasQuantizationWrapper, Layer]:
         """
         A function which takes a computational graph node and a keras layer and perform the quantization wrapping.
 
         Args:
             n: A node of mct graph.
             layer: A keras layer
 
         Returns: Wrapped layer if the layer should be wrap, otherwise returns the layer as is.
 
         """
-        if self._is_gptq_applicable(n):
-            weights_quantizers, activation_quantizers = quantization_builder(n, self.gptq_config)
-            return qi.KerasQuantizationWrapper(layer,
-                                               weights_quantizers=weights_quantizers,
-                                               activation_quantizers=activation_quantizers)
-        else:
-            return layer
+        if self._is_gptq_weights_trainable(n):
+            weights_quantizers, _ = quantization_builder(n,
+                                                         self.gptq_config) # TODO: split quantizers building into two functions: for weights and activations
+            if len(weights_quantizers) > 0:
+                return KerasQuantizationWrapper(layer,
+                                                   weights_quantizers=weights_quantizers)
+        return layer
+
+    def get_activation_quantizer_holder(self, n: common.BaseNode) -> Callable:
+        """
+        Retrieve a KerasActivationQuantizationHolder layer to use for activation quantization for a node.
+        If the layer is not supposed to be wrapped with activation quantizers - return None.
+
+        Args:
+            n: Node to get KerasActivationQuantizationHolder to attach in its output.
+
+        Returns:
+            A KerasActivationQuantizationHolder layer for the node activation quantization.
+        """
+        _, activation_quantizers = quantization_builder(n, self.gptq_config) # TODO: split quantizers building into two functions: for weights and activations
+
+        # Holder by definition uses a single quantizer for the activation quantization
+        # thus we make sure this is the only possible case (unless it's a node with no activation
+        # quantization, which in this case has an empty list).
+        if len(activation_quantizers) == 1:
+            return KerasActivationQuantizationHolder(activation_quantizers[0])
+
+        Logger.error(
+            f'KerasActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers '
+            f'were found for node {n}')
+
 
     def build_gptq_model(self) -> Tuple[Model, UserInformation]:
         """
         Build the GPTQ model with QuantizationWrappers
 
         Returns:
             Quantized graph for GPTQ fine-tuning, GPTQ graph user info
         """
 
         gptq_model, gptq_user_info = KerasModelBuilder(graph=self.graph_quant,
                                                        append2output=self.compare_points,
                                                        fw_info=self.fw_info,
                                                        return_float_outputs=True,
-                                                       wrapper=self.gptq_wrapper).build_model()
+                                                       wrapper=self.gptq_wrapper,
+                                                       get_activation_quantizer_holder_fn=self.get_activation_quantizer_holder).build_model()
 
         return gptq_model, gptq_user_info
 
     def compute_gradients(self, in_y_float: List[tf.Tensor], input_data: List[np.ndarray],
                           in_optimizer_with_param: List,
                           training=True) -> Tuple[tf.Tensor, List[tf.Tensor]]:
         """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/graph_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/graph_info.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,16 +16,17 @@
 import tensorflow as tf
 from typing import Tuple, List
 from model_compression_toolkit.core.keras.constants import USE_BIAS
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from tensorflow.keras.models import Model
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
-from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.logger import Logger
+from mct_quantizers import KerasQuantizationWrapper
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def get_gptq_trainable_parameters(fxp_model: Model,
                                   fw_info: FrameworkInfo,
                                   add_bias: bool = False) -> (
         List[tf.Variable], List[tf.Variable], List[tf.Variable]):
     """
@@ -46,14 +47,17 @@
 
     for layer in fxp_model.layers:
         if isinstance(layer, KerasQuantizationWrapper):
             kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=type(layer.layer),
                                                                   fw_info=DEFAULT_KERAS_INFO)
 
             # collect trainable weights per quantizer
+            if kernel_attribute not in layer.weights_quantizers:
+                Logger.error(f'{kernel_attribute} was not found in weight quantizers of layer {layer.layer}')
+
             quantizer_trainable_weights = layer.weights_quantizers[kernel_attribute].get_trainable_variables(VariableGroup.WEIGHTS)
             quantizer_trainable_threshold = layer.weights_quantizers[kernel_attribute].get_trainable_variables(VariableGroup.QPARAMS)
             trainable_weights.append(quantizer_trainable_weights)
             trainable_threshold.extend(quantizer_trainable_threshold)
 
             if add_bias:
                 kernel_ops_attrs = fw_info.kernel_ops_attributes_mapping.get(type(layer.layer))
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantization_facade.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,15 @@
                                                                representative_data_gen: Callable,
                                                                gptq_config: GradientPTQConfigV2,
                                                                gptq_representative_data_gen: Callable = None,
                                                                target_kpi: KPI = None,
                                                                core_config: CoreConfig = CoreConfig(),
                                                                fw_info: FrameworkInfo = DEFAULT_KERAS_INFO,
                                                                target_platform_capabilities: TargetPlatformCapabilities = DEFAULT_KERAS_TPC,
-                                                               new_experimental_exporter: bool = False) -> \
-    Tuple[Model, UserInformation]:
+                                                               new_experimental_exporter: bool = True) -> Tuple[Model, UserInformation]:
         """
         Quantize a trained Keras model using post-training quantization. The model is quantized using a
         symmetric constraint quantization thresholds (power of two).
         The model is first optimized using several transformations (e.g. BatchNormalization folding to
         preceding layers). Then, using a given dataset, statistics (e.g. min/max, histogram, etc.) are
         being collected for each layer's output (and input, depends on the quantization configuration).
         For each possible bit width (per layer) a threshold is then being calculated using the collected
@@ -137,15 +136,15 @@
             representative_data_gen (Callable): Dataset used for calibration.
             gptq_config (GradientPTQConfigV2): Configuration for using gptq (e.g. optimizer).
             gptq_representative_data_gen (Callable): Dataset used for GPTQ training. If None defaults to representative_data_gen
             target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
             core_config (CoreConfig): Configuration object containing parameters of how the model should be quantized, including mixed precision parameters.
             fw_info (FrameworkInfo): Information needed for quantization about the specific framework (e.g., kernel channels indices, groups of layers by how they should be quantized, etc.). `Default Keras info <https://github.com/sony/model_optimization/blob/main/model_compression_toolkit/core/keras/default_framework_info.py>`_
             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
-            new_experimental_exporter (bool): Whether exporting the quantized model using new exporter or not (in progress. Avoiding it for now is recommended).
+            new_experimental_exporter (bool): Whether to wrap the quantized model using quantization information or not. Enabled by default. Experimental and subject to future changes.
 
         Returns:
 
             A quantized model and information the user may need to handle the quantized model.
 
         Examples:
 
@@ -196,14 +195,15 @@
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
                 Logger.error("Given quantization config to mixed-precision facade is not of type "
                                     "MixedPrecisionQuantizationConfigV2. Please use keras_post_training_quantization "
                                     "API, or pass a valid mixed precision configuration.")  # pragma: no cover
 
             Logger.info("Using experimental mixed-precision quantization. "
                                "If you encounter an issue please file a bug.")
+
         tb_w = _init_tensorboard_writer(fw_info)
 
         fw_impl = GPTQKerasImplemantation()
 
         tg, bit_widths_config = core_runner(in_model=in_model,
                                             representative_data_gen=representative_data_gen,
                                             core_config=core_config,
@@ -222,16 +222,19 @@
                               fw_impl,
                               tb_w)
 
         if core_config.debug_config.analyze_similarity:
             analyzer_model_quantization(representative_data_gen, tb_w, tg_gptq, fw_impl, fw_info)
 
         if new_experimental_exporter:
-            Logger.warning('Using new experimental exported models. '
-                           'Please do not use unless you are familiar with what you are doing')
+            Logger.warning('Using new experimental wrapped and ready for export models. To '
+                           'disable it, please set new_experimental_exporter to False when '
+                           'calling keras_gradient_post_training_quantization_experimental. '
+                           'If you encounter an issue please file a bug.')
+
             return get_exportable_keras_model(tg_gptq)
 
         return export_model(tg_gptq,
                             fw_info,
                             fw_impl,
                             tb_w,
                             bit_widths_config)
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/base_keras_gptq_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,23 +15,22 @@
 from abc import abstractmethod
 from typing import Union, Dict, List
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.gptq.common.gptq_constants import WEIGHTS_QUANTIZATION_PARAMS
 
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
-    TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer
 
 if FOUND_TF:
     import tensorflow as tf
 
-    from model_compression_toolkit.quantizers_infrastructure import BaseKerasTrainableQuantizer, \
-        KerasQuantizationWrapper
+    from model_compression_toolkit.trainable_infrastructure import BaseKerasTrainableQuantizer
+    from mct_quantizers import KerasQuantizationWrapper
 
     class BaseKerasGPTQTrainableQuantizer(BaseKerasTrainableQuantizer):
         """
         A base class for trainable Keras quantizer for GPTQ.
         """
 
         def __init__(self,
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/quantization_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,22 +17,20 @@
 from model_compression_toolkit.gptq import GradientPTQConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizer import \
     get_inferable_quantizer_kwargs
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
-    get_inferable_quantizer_class
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer import \
-    BaseKerasInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizer_config import \
+from mct_quantizers import QuantizationTarget
+from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
+from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizer_config import \
     get_trainable_quantizer_weights_config
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizers import \
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizers import \
     get_trainable_quantizer_class
 
 
 def quantization_builder(n: common.BaseNode,
                          gptq_config: GradientPTQConfigV2
                          ) -> Tuple[Dict[str, BaseKerasGPTQTrainableQuantizer], List[BaseKerasInferableQuantizer]]:
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from typing import List
 
 import tensorflow as tf
 from keras import Model
 
 from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
-from model_compression_toolkit.quantizers_infrastructure import KerasQuantizationWrapper
+from mct_quantizers import KerasQuantizationWrapper
 
 
 class LinearTempDecay:
     """
     Annealing process for the soft quantizer regularization temperature term.
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,29 +13,29 @@
 # limitations under the License.
 # ==============================================================================
 
 import tensorflow as tf
 import numpy as np
 
 from model_compression_toolkit.gptq import RoundingType
-from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.core.common import max_power_of_two
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget
 from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, \
     SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
 from typing import Dict, Any
 from model_compression_toolkit.constants import THRESHOLD, MIN_THRESHOLD
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
 from model_compression_toolkit.gptq.keras.quantizer.quant_utils import power_of_two_max, clip, calculate_delta
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def soft_rounding_symmetric_quantizer(input_tensor: tf.Tensor,
                                       auxvar_tensor: tf.Variable,
                                       threshold_tensor: tf.Tensor,
                                       num_bits: int,
                                       signed: bool,
@@ -62,15 +62,15 @@
     input_tensor_int = tf.floor(input_tensor / delta)
     tensor_q = input_tensor_int + auxvar_tensor
     min_int = -int(signed) * (2 ** (num_bits - int(signed)))
     max_int = (2 ** (num_bits - int(signed))) - 1
     return delta * clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.SoftQuantizer)
 class SymmetricSoftRoundingGPTQ(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
@@ -213,26 +213,28 @@
                                                          threshold_tensor=ptq_threshold_tensor_hat,
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
             if self.quantization_parameter_learning and not self.power_of_two:
                 scale = tf.reshape(self.get_quantizer_variable(SCALE_PTQ), reshape_shape)
+                scale = tf.where(scale <= 0, MIN_THRESHOLD, scale)
                 q_tensor *= scale
 
         else:
             q_tensor = soft_rounding_symmetric_quantizer(input_tensor=inputs,
                                                          auxvar_tensor=aux_var,
                                                          threshold_tensor=ptq_threshold_tensor.value(),
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
             if self.quantization_parameter_learning and not self.power_of_two:
                 scale = self.get_quantizer_variable(SCALE_PTQ)
+                scale = tf.where(scale <= 0, MIN_THRESHOLD, scale)
                 q_tensor *= scale
 
         return q_tensor
 
     def get_quant_config(self) -> Dict[str, np.ndarray]:
         """
         Returns the config used to edit NodeQuantizationConfig after GPTQ retraining
@@ -245,12 +247,15 @@
         if self.power_of_two:
             old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
             old_threshold = max_power_of_two(old_threshold, MIN_THRESHOLD)
 
         else:
             old_threshold = self.get_quantizer_variable(PTQ_THRESHOLD)
             if self.quantization_parameter_learning:
-                scale = tf.reshape(self.get_quantizer_variable(SCALE_PTQ), self.threshold_shape)
+                scale = self.get_quantizer_variable(SCALE_PTQ)
+                if self.per_channel:
+                    scale = tf.reshape(scale, self.threshold_shape)
+                scale = tf.where(scale <= 0, MIN_THRESHOLD, scale)
                 old_threshold = old_threshold * scale
             old_threshold = old_threshold.numpy()
         old_threshold = old_threshold.reshape(self.threshold_shape)
         return {THRESHOLD: old_threshold}
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # limitations under the License.
 # ==============================================================================
 
 import tensorflow as tf
 import numpy as np
 
 from model_compression_toolkit.gptq import RoundingType
-from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.trainable_infrastructure.common.constants import FQ_MIN, FQ_MAX
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget
 from model_compression_toolkit.gptq.common.gptq_constants import \
     SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
 from typing import Dict, Any
 from model_compression_toolkit.constants import RANGE_MIN, RANGE_MAX
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def soft_rounding_uniform_quantizer(input_tensor: tf.Tensor,
                                     auxvar_tensor: tf.Variable,
                                     min_tensor: tf.Tensor,
                                     max_tensor: tf.Tensor,
                                     num_bits: int) -> tf.Tensor:
@@ -57,15 +57,15 @@
     input_tensor_int = qutils.ste_floor((input_tensor - min_range) / delta)
     tensor_q = input_tensor_int + auxvar_tensor
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=0,
                                    max_val=2 ** num_bits - 1) + min_range
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=RoundingType.SoftQuantizer)
 class UniformSoftRoundingGPTQ(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable uniform quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,26 +15,26 @@
 
 from typing import Dict, Any
 
 import numpy as np
 import tensorflow as tf
 
 from model_compression_toolkit.gptq import RoundingType
-from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget
 from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD
 from model_compression_toolkit.gptq.keras.quantizer import quant_utils as qutils
 from model_compression_toolkit.constants import THRESHOLD
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 from model_compression_toolkit.gptq.keras.quantizer.base_keras_gptq_quantizer import BaseKerasGPTQTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def pertubation_symmetric_quantizer(input_tensor: tf.Tensor,
                                     auxvar_tensor: tf.Variable,
                                     max_tensor: tf.Tensor,
                                     num_bits: int,
                                     signed: bool,
@@ -63,15 +63,15 @@
     tensor_q = qutils.ste_round(
         input_tensor_int + qutils.ste_clip(auxvar_tensor, max_val=max_lsbs_change * delta) / delta)
     min_int = -int(signed) * (2 ** (num_bits - int(signed)))
     max_int = (2 ** (num_bits - int(signed))) - 1
     return delta * qutils.ste_clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.STE)
 class STEWeightGPTQQuantizer(BaseKerasGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to quantize a layer weights.
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_loss.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/gptq_loss.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/gptq_pytorch_implementation.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/gptq_training.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/gptq_training.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,16 @@
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.framework_implementation import FrameworkImplementation
 from model_compression_toolkit.core.pytorch.constants import BIAS
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, set_model, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.graph_info import get_gptq_trainable_parameters, \
     get_weights_for_loss
 from model_compression_toolkit.gptq.pytorch.quantizer.quantization_builder import quantization_builder
-from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.gptq.pytorch.quantizer.regularization_factory import get_regularization
-from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
+from mct_quantizers import PytorchQuantizationWrapper, PytorchActivationQuantizationHolder
 
 
 class PytorchGPTQTrainer(GPTQTrainer):
     """
     Pytorch GPTQ training class for fine-tuning a quantized model
     """
 
@@ -86,59 +85,80 @@
                                                                   trainable_bias,
                                                                   trainable_threshold)
 
         self.weights_for_average_loss = to_torch_tensor(self.compute_hessian_based_weights(representative_data_gen))
 
         self.reg_func = get_regularization(self.gptq_config, representative_data_gen)
 
-    def _is_gptq_applicable(self,
-                            node: BaseNode) -> bool:
+    def _is_gptq_weights_trainable(self,
+                                   node: BaseNode) -> bool:
         """
         A function for deciding if a layer should be fine-tuned during GPTQ.
         Args:
             node (BaseNode): Node for quantization decision
         Returns:
             A boolean whether the layer is to be wrapped with a Quantization Wrapper.
         """
 
         if node.is_weights_quantization_enabled() and not self.fw_info.is_kernel_op(node.type):
             Logger.error(f"GPTQ Error: Quantizing node {node.name} of type {node.type} "
                          f"without a kernel isn't supported.")
         return node.is_weights_quantization_enabled()
 
-    def gptq_wrapper(self, n: BaseNode, layer: Module) -> Union[qi.PytorchQuantizationWrapper, Module]:
+    def gptq_wrapper(self,
+                     n: BaseNode,
+                     layer: Module) -> Union[PytorchQuantizationWrapper, Module]:
         """
         A function which takes a computational graph node and a pytorch layer and perform the quantization wrapping.
 
         Args:
             n: A node of mct graph.
             layer: A pytorch layer
 
         Returns: Wrapped layer if the layer should be wrap, otherwise returns the layer as is.
         """
 
-        if self._is_gptq_applicable(n):
+        if self._is_gptq_weights_trainable(n):
             weights_quantizers, activation_quantizers = quantization_builder(n, self.gptq_config)
-            return qi.PytorchQuantizationWrapper(layer,
-                                                 weights_quantizers=weights_quantizers,
-                                                 activation_quantizers=activation_quantizers)
+            return PytorchQuantizationWrapper(layer,
+                                              weights_quantizers=weights_quantizers)
         else:
             return layer
 
+    def get_activation_quantizer_holder(self, n: BaseNode) -> Callable:
+        """
+        Retrieve a PytorchActivationQuantizationHolder layer to use for activation quantization of a node.
+        If the layer is not supposed to be wrapped with an activation quantizer - return None.
+        Args:
+            n: Node to attach a PytorchActivationQuantizationHolder to its output.
+        Returns:
+            A PytorchActivationQuantizationHolder module for the node's activation quantization.
+        """
+        _, activation_quantizers = quantization_builder(n, self.gptq_config)
+        # Holder by definition uses a single quantizer for the activation quantization
+        # thus we make sure this is the only possible case (unless it's a node we no activation
+        # quantization, which in this case has an empty list).
+        if len(activation_quantizers) == 1:
+            return PytorchActivationQuantizationHolder(activation_quantizers[0])
+        Logger.error(
+            f'PytorchActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers '
+            f'were found for node {n}')
+
     def build_gptq_model(self):
         """
         Build the GPTQ model with QuantizationWrappers
         Returns:
             Quantized graph for GPTQ fine-tuning, GPTQ graph user info
         """
         gptq_model, gptq_user_info = PyTorchModelBuilder(graph=self.graph_quant,
                                                          append2output=self.compare_points,
                                                          fw_info=self.fw_info,
                                                          wrapper=self.gptq_wrapper,
-                                                         return_float_outputs=True).build_model()
+                                                         return_float_outputs=True,
+                                                         get_activation_quantizer_holder_fn=self.get_activation_quantizer_holder).build_model()
 
         return gptq_model, gptq_user_info
 
     def train(self, representative_data_gen: Callable):
         """
           GPTQ Training using pytorch framework
           Args:
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/graph_info.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/graph_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,16 +14,17 @@
 # ==============================================================================
 import torch
 import torch.nn as nn
 from typing import List
 from model_compression_toolkit.core.pytorch.constants import BIAS
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
-from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.logger import Logger
+from mct_quantizers import PytorchQuantizationWrapper
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def get_gptq_trainable_parameters(fxp_model: nn.Module,
                                   add_bias: bool = False,
                                   ) -> (List[nn.Parameter], List[nn.Parameter], List[nn.Parameter]):
     """
     Get trainable parameters from all layers in a model
@@ -42,14 +43,16 @@
 
     for layer in fxp_model.modules():
         if isinstance(layer, PytorchQuantizationWrapper):
             kernel_attribute = get_kernel_attribute_name_for_gptq(layer_type=type(layer.layer),
                                                                   fw_info=DEFAULT_PYTORCH_INFO)
 
             # collect trainable weights per quantizer
+            if kernel_attribute not in layer.weights_quantizers:
+                Logger.error(f'{kernel_attribute} was not found in weight quantizers of layer {layer.layer}')
             quantizer_trainable_weights = layer.weights_quantizers[kernel_attribute].get_trainable_variables(VariableGroup.WEIGHTS)
             quantizer_trainable_threshold = layer.weights_quantizers[kernel_attribute].get_trainable_variables(VariableGroup.QPARAMS)
             trainable_aux_weights.extend(quantizer_trainable_weights)
             trainable_threshold.extend(quantizer_trainable_threshold)
 
             if add_bias and hasattr(layer.layer, BIAS):
                 bias = getattr(layer.layer, BIAS)
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantization_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,24 +49,26 @@
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
 
     def get_pytorch_gptq_config(n_epochs: int,
                                 optimizer: Optimizer = Adam([torch.Tensor([])], lr=LR_DEFAULT),
                                 optimizer_rest: Optimizer = Adam([torch.Tensor([])], lr=LR_REST_DEFAULT),
                                 loss: Callable = multiple_tensors_mse_loss,
-                                log_function: Callable = None) -> GradientPTQConfigV2:
+                                log_function: Callable = None,
+                                use_hessian_based_weights: bool = True) -> GradientPTQConfigV2:
         """
         Create a GradientPTQConfigV2 instance for Pytorch models.
 
         args:
             n_epochs (int): Number of epochs for running the representative dataset for fine-tuning.
             optimizer (Optimizer): Pytorch optimizer to use for fine-tuning for auxiliry variable.
             optimizer_rest (Optimizer): Pytorch optimizer to use for fine-tuning of the bias variable.
             loss (Callable): loss to use during fine-tuning. should accept 4 lists of tensors. 1st list of quantized tensors, the 2nd list is the float tensors, the 3rd is a list of quantized weights and the 4th is a list of float weights.
             log_function (Callable): Function to log information about the gptq process.
+            use_hessian_based_weights (bool): Whether to use Hessian-based weights for weighted average loss.
 
         returns:
             a GradientPTQConfigV2 object to use when fine-tuning the quantized model using gptq.
 
         Examples:
 
             Import MCT and Create a GradientPTQConfigV2 to run for 5 epochs:
@@ -80,25 +82,25 @@
             >>> gptq_conf = mct.gptq.get_pytorch_gptq_config(n_epochs=3, optimizer=torch.optim.Adam([torch.Tensor(1)]))
 
             The configuration can be passed to :func:`~model_compression_toolkit.pytorch_post_training_quantization` in order to quantize a pytorch model using gptq.
 
         """
         bias_optimizer = torch.optim.SGD([torch.Tensor([])], lr=LR_BIAS_DEFAULT, momentum=GPTQ_MOMENTUM)
         return GradientPTQConfigV2(n_epochs, optimizer, optimizer_rest=optimizer_rest, loss=loss,
-                                   log_function=log_function, train_bias=True, optimizer_bias=bias_optimizer)
+                                   log_function=log_function, train_bias=True, optimizer_bias=bias_optimizer, use_hessian_based_weights=use_hessian_based_weights)
 
 
     def pytorch_gradient_post_training_quantization_experimental(model: Module,
                                                                  representative_data_gen: Callable,
                                                                  target_kpi: KPI = None,
                                                                  core_config: CoreConfig = CoreConfig(),
                                                                  gptq_config: GradientPTQConfigV2 = None,
                                                                  gptq_representative_data_gen: Callable = None,
                                                                  target_platform_capabilities: TargetPlatformCapabilities = DEFAULT_PYTORCH_TPC,
-                                                                 new_experimental_exporter: bool = False):
+                                                                 new_experimental_exporter: bool = True):
         """
         Quantize a trained Pytorch module using post-training quantization.
         By default, the module is quantized using a symmetric constraint quantization thresholds
         (power of two) as defined in the default TargetPlatformCapabilities.
         The module is first optimized using several transformations (e.g. BatchNormalization folding to
         preceding layers). Then, using a given dataset, statistics (e.g. min/max, histogram, etc.) are
         being collected for each layer's output (and input, depends on the quantization configuration).
@@ -115,15 +117,15 @@
             model (Module): Pytorch model to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
             core_config (CoreConfig): Configuration object containing parameters of how the model should be quantized, including mixed precision parameters.
             gptq_config (GradientPTQConfigV2): Configuration for using gptq (e.g. optimizer).
             gptq_representative_data_gen (Callable): Dataset used for GPTQ training. If None defaults to representative_data_gen
             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to.
-            new_experimental_exporter (bool): Whether exporting the quantized model using new exporter or not (in progress. Avoiding it for now is recommended).
+            new_experimental_exporter (bool): Whether to wrap the quantized model using quantization information or not. Enabled by default. Experimental and subject to future changes.
 
         Returns:
             A quantized module and information the user may need to handle the quantized module.
 
         Examples:
 
             Import a Pytorch module:
@@ -185,16 +187,18 @@
         if core_config.debug_config.analyze_similarity:
             analyzer_model_quantization(representative_data_gen, tb_w, graph_gptq, fw_impl, DEFAULT_PYTORCH_INFO)
 
         # ---------------------- #
         # Export
         # ---------------------- #
         if new_experimental_exporter:
-            Logger.warning('Using new experimental exported models. '
-                           'Please do not use unless you are familiar with what you are doing')
+            Logger.warning('Using new experimental wrapped and ready for export models. To '
+                           'disable it, please set new_experimental_exporter to False when '
+                           'calling pytorch_gradient_post_training_quantization_experimental. '
+                           'If you encounter an issue please file a bug.')
 
             return get_exportable_pytorch_model(graph_gptq)
 
         return export_model(graph_gptq,
                             DEFAULT_PYTORCH_INFO,
                             fw_impl,
                             tb_w,
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/base_pytorch_gptq_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,24 +15,24 @@
 from abc import abstractmethod
 from typing import Union, Dict
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TORCH
 from model_compression_toolkit.gptq.common.gptq_constants import WEIGHTS_QUANTIZATION_PARAMS
 
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import \
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import \
     BaseTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
+from model_compression_toolkit.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
     BasePytorchTrainableQuantizer
 
 if FOUND_TORCH:
     from torch import Tensor
-    from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
+    from mct_quantizers import PytorchQuantizationWrapper
 
     class BasePytorchGPTQTrainableQuantizer(BasePytorchTrainableQuantizer):
         """
         A base class for trainable Pytorch quantizer for GPTQ.
         """
 
         def __init__(self,
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/quantization_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,23 +17,21 @@
 from model_compression_toolkit.gptq import GradientPTQConfigV2
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.pytorch.constants import KERNEL
 from model_compression_toolkit.exporter.model_wrapper.pytorch.builder.node_to_quantizer import \
     get_activation_inferable_quantizer_kwargs
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_quantizers import \
-    get_inferable_quantizer_class
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
-    BasePyTorchInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizer_config import \
+from mct_quantizers import QuantizationTarget
+from mct_quantizers.common.get_quantizers import get_inferable_quantizer_class
+from mct_quantizers.pytorch.quantizers import BasePyTorchInferableQuantizer
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizer_config import \
     get_trainable_quantizer_weights_config
 from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizers import \
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizers import \
     get_trainable_quantizer_class
 
 
 def quantization_builder(n: common.BaseNode,
                          gptq_config: GradientPTQConfigV2,
                          ) -> Tuple[Dict[str, BasePytorchQATTrainableQuantizer],
                                     List[BasePyTorchInferableQuantizer]]:
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/regularization_factory.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/soft_quantizer_reg.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import torch
 import numpy as np
 from torch import nn
 
 from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.gptq.common.gptq_graph import get_kernel_attribute_name_for_gptq
-from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
+from mct_quantizers import PytorchQuantizationWrapper
 
 
 class LinearTempDecay:
     """
     Annealing process for the soft quantizer regularization temperature term.
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/symmetric_soft_quantizer.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,29 +14,29 @@
 # ==============================================================================
 import torch
 import torch.nn as nn
 from typing import Dict
 import numpy as np
 
 from model_compression_toolkit.core.common import max_power_of_two
-from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget, PytorchQuantizationWrapper
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import PTQ_THRESHOLD, SCALE_PTQ, \
     SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.constants import THRESHOLD, MIN_THRESHOLD
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
 def soft_rounding_symmetric_quantizer(input_tensor: torch.Tensor,
                                       auxvar_tensor: torch.Tensor,
                                       threshold_tensor: torch.Tensor,
                                       num_bits: int,
                                       signed: bool,
@@ -64,15 +64,15 @@
     tensor_q = input_tensor_int + auxvar_tensor
     int_threshold = 2 ** (num_bits - int(signed))
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=-int(signed) * int_threshold,
                                    max_val=int_threshold - 1)
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.SoftQuantizer)
 class SymmetricSoftRoundingGPTQ(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
@@ -106,15 +106,15 @@
         self.zeta = SOFT_ROUNDING_ZETA
 
         self.quantizer_parameters = {}
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
@@ -174,14 +174,15 @@
         old_threshold = torch_tensor_to_numpy(self.get_quantizer_variable(PTQ_THRESHOLD))
         old_threshold = np.resize(old_threshold, self.threshold_shape)
         if self.power_of_two:
             old_threshold = max_power_of_two(old_threshold, MIN_THRESHOLD)
         else:
             if self.quantization_parameter_learning:
                 scale = torch.reshape(self.get_quantizer_variable(SCALE_PTQ), self.threshold_shape)
+                scale = torch.where(scale <= 0, torch.tensor(MIN_THRESHOLD, device=scale.device), scale)
                 old_threshold = old_threshold * torch_tensor_to_numpy(scale)
         old_threshold = old_threshold.reshape(self.threshold_shape)
         return {THRESHOLD: old_threshold}
 
     def __call__(self,
                  inputs: nn.Parameter,
                  training: bool) -> torch.Tensor:
@@ -223,22 +224,24 @@
                                                          threshold_tensor=ptq_threshold_tensor_hat,
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
             if self.quantization_parameter_learning and not self.power_of_two:
                 scale = torch.reshape(self.get_quantizer_variable(SCALE_PTQ), reshape_shape)
+                scale = torch.where(scale <= 0, torch.tensor(MIN_THRESHOLD, device=scale.device), scale)
                 q_tensor *= scale
 
         else:
             q_tensor = soft_rounding_symmetric_quantizer(input_tensor=inputs,
                                                          auxvar_tensor=aux_var,
                                                          threshold_tensor=ptq_threshold_tensor,
                                                          num_bits=self.num_bits,
                                                          signed=True,
                                                          power_of_two=self.power_of_two)
 
             if self.quantization_parameter_learning and not self.power_of_two:
                 scale = self.get_quantizer_variable(SCALE_PTQ)
+                scale = torch.where(scale <= 0, torch.tensor(MIN_THRESHOLD, device=scale.device), scale)
                 q_tensor *= scale
 
         return q_tensor
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/soft_rounding/uniform_soft_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 # limitations under the License.
 # ==============================================================================
 import torch
 import torch.nn as nn
 from typing import Dict
 import numpy as np
 
-from model_compression_toolkit import quantizers_infrastructure as qi
-from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.trainable_infrastructure.common.constants import FQ_MIN, FQ_MAX
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget, PytorchQuantizationWrapper
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import SOFT_ROUNDING_GAMMA, SOFT_ROUNDING_ZETA, AUXVAR
 from model_compression_toolkit.gptq.pytorch.quantizer.quant_utils import fix_range_to_include_zero
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
-    mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import \
     VariableGroup
 from model_compression_toolkit.constants import RANGE_MAX, RANGE_MIN
 
 
 def soft_rounding_unifrom_quantizer(input_tensor: torch.Tensor,
                                     auxvar_tensor: torch.Tensor,
                                     min_range: torch.Tensor,
@@ -59,15 +58,15 @@
     input_tensor_int = qutils.ste_floor((input_tensor - min_range) / delta)
     tensor_q = input_tensor_int + auxvar_tensor
     return delta * qutils.ste_clip(tensor_q,
                                    min_val=0,
                                    max_val=2 ** num_bits - 1) + min_range
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=RoundingType.SoftQuantizer)
 class UniformSoftRoundingGPTQ(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable uniform quantizer to optimize the rounding of the quantized values using a soft quantization method.
     """
 
@@ -96,15 +95,15 @@
         # See: https://arxiv.org/pdf/2004.10568.pdf
         self.gamma = SOFT_ROUNDING_GAMMA
         self.zeta = SOFT_ROUNDING_ZETA
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,27 @@
 # ==============================================================================
 import torch
 import torch.nn as nn
 from typing import Dict
 import numpy as np
 from model_compression_toolkit.core.common.defaultdict import DefaultDict
 
-from model_compression_toolkit import quantizers_infrastructure as qi
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget, PytorchQuantizationWrapper
 from model_compression_toolkit.gptq.common.gptq_config import RoundingType
 from model_compression_toolkit.gptq.pytorch.quantizer.base_pytorch_gptq_quantizer import \
     BasePytorchGPTQTrainableQuantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor, torch_tensor_to_numpy
 from model_compression_toolkit.gptq.pytorch.quantizer import quant_utils as qutils
 from model_compression_toolkit.gptq.common.gptq_constants import AUXVAR, PTQ_THRESHOLD, MAX_LSB_CHANGE
 from model_compression_toolkit.constants import THRESHOLD
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
-    mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.quant_utils import \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig
+from mct_quantizers import mark_quantizer
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.quant_utils import \
     get_threshold_reshape_shape
 
 
 def pertubation_symmetric_quantizer(input_tensor: torch.Tensor,
                                     auxvar_tensor: nn.Parameter,
                                     max_tensor: torch.Tensor,
                                     num_bits: int,
@@ -71,15 +70,15 @@
     input_tensor_int = torch.round(input_tensor / delta).detach()
 
     tensor_q = qutils.ste_round(qutils.ste_round(input_tensor_int + tensor_clipped))
 
     return delta * qutils.ste_clip(tensor_q, max_val=max_int, min_val=min_int)
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=RoundingType.STE)
 class STEWeightGPTQQuantizer(BasePytorchGPTQTrainableQuantizer):
     """
     Trainable symmetric quantizer to quantize a layer weights.
     """
 
@@ -105,15 +104,15 @@
         self.power_of_two = quantization_config.weights_quantization_method == QuantizationMethod.POWER_OF_TWO
         self.max_lsbs_change = max_lsbs_change_map.get(self.num_bits)
 
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/gptq/runner.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/gptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/keras_quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/keras_quantization_facade.py`

 * *Files 7% similar despite different names*

```diff
@@ -99,14 +99,17 @@
 
             Import mct and pass the model with the representative dataset generator to get a quantized model:
 
             >>> import model_compression_toolkit as mct
             >>> quantized_model, quantization_info = mct.keras_post_training_quantization(model, repr_datagen, n_iter=1)
 
         """
+        Logger.warning('keras_post_training_quantization is deprecated and will be removed '
+                       'in the future. Please use mct.ptq.keras_post_training_quantization_experimental instead.')
+
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         core_config = CoreConfig(quantization_config=quant_config,
                                  debug_config=DebugConfig(analyze_similarity=analyze_similarity,
                                                           network_editor=network_editor)
                                  )
@@ -220,14 +223,17 @@
              quantized model:
 
              >>> quantized_model, quantization_info = mct.keras_post_training_quantization_mixed_precision(model,repr_datagen, target_kpi=kpi, n_iter=10, quant_config=config)
 
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/experimental_api_docs/modules/mixed_precision_quantization_config.html#model_compression_toolkit.MixedPrecisionQuantizationConfigV2>`_.
 
          """
+        Logger.warning('keras_post_training_quantization_mixed_precision is deprecated and will be removed '
+                       'in the future. Please use mct.ptq.keras_post_training_quantization_experimental instead.')
+
         KerasModelValidation(model=in_model,
                              fw_info=fw_info).validate()
 
         if not isinstance(quant_config, MixedPrecisionQuantizationConfig):
             Logger.error("Given quantization config to mixed-precision facade is not of type "
                                 "MixedPrecisionQuantizationConfig. Please use keras_post_training_quantization API,"
                                 "or pass a valid mixed precision configuration.")
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/legacy/pytorch_quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/legacy/pytorch_quantization_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,16 @@
 
             Import mct and pass the module with the representative dataset generator to get a quantized module:
 
             >>> import model_compression_toolkit as mct
             >>> quantized_module, quantization_info = mct.pytorch_post_training_quantization(module, repr_datagen)
 
         """
+        Logger.warning('pytorch_post_training_quantization is deprecated and will be removed '
+                       'in the future. Please use mct.ptq.pytorch_post_training_quantization_experimental instead.')
 
         core_config = CoreConfig(quant_config,
                                  debug_config=DebugConfig(analyze_similarity=analyze_similarity,
                                                           network_editor=network_editor))
 
         tb_w = _init_tensorboard_writer(fw_info)
 
@@ -211,14 +213,17 @@
 
              >>> quantized_model, quantization_info = mct.pytorch_post_training_quantization_mixed_precision(module, repr_datagen, n_iter=10, quant_config=config, target_kpi=kpi)
 
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/experimental_api_docs/modules/mixed_precision_quantization_config.html#model_compression_toolkit.MixedPrecisionQuantizationConfigV2>`_.
 
          """
 
+        Logger.warning('pytorch_post_training_quantization_mixed_precision is deprecated and will be removed '
+                       'in the future. Please use mct.ptq.pytorch_post_training_quantization_experimental instead.')
+
         if not isinstance(quant_config, MixedPrecisionQuantizationConfig):
             Logger.error("Given quantization config to mixed-precision facade is not of type "
                                 "MixedPrecisionQuantizationConfig. Please use pytorch_post_training_quantization API, "
                                 "or pass a valid mixed precision configuration.")
 
         Logger.info("Using experimental mixed-precision quantization. "
                            "If you encounter an issue please file a bug.")
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/logger.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/logger.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/keras/quantization_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 
     def keras_post_training_quantization_experimental(in_model: Model,
                                                       representative_data_gen: Callable,
                                                       target_kpi: KPI = None,
                                                       core_config: CoreConfig = CoreConfig(),
                                                       target_platform_capabilities: TargetPlatformCapabilities = DEFAULT_KERAS_TPC,
-                                                      new_experimental_exporter: bool = False):
+                                                      new_experimental_exporter: bool = True):
         """
          Quantize a trained Keras model using post-training quantization. The model is quantized using a
          symmetric constraint quantization thresholds (power of two).
          The model is first optimized using several transformations (e.g. BatchNormalization folding to
          preceding layers). Then, using a given dataset, statistics (e.g. min/max, histogram, etc.) are
          being collected for each layer's output (and input, depends on the quantization configuration).
          For each possible bit width (per layer) a threshold is then being calculated using the collected
@@ -60,15 +60,15 @@
 
          Args:
              in_model (Model): Keras model to quantize.
              representative_data_gen (Callable): Dataset used for calibration.
              target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
              core_config (CoreConfig): Configuration object containing parameters of how the model should be quantized, including mixed precision parameters.
              target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the Keras model according to.
-             new_experimental_exporter (bool): Whether exporting the quantized model using new exporter or not (in progress. Avoiding it for now is recommended).
+             new_experimental_exporter (bool): Whether to wrap the quantized model using quantization information or not. Enabled by default. Experimental and subject to future changes.
 
          Returns:
 
              A quantized model and information the user may need to handle the quantized model.
 
          Examples:
 
@@ -148,16 +148,19 @@
         if core_config.debug_config.analyze_similarity:
             analyzer_model_quantization(representative_data_gen,
                                         tb_w, tg,
                                         fw_impl,
                                         fw_info)
 
         if new_experimental_exporter:
-            Logger.warning('Using new experimental exported models. '
-                           'Please do not use unless you are familiar with what you are doing')
+            Logger.warning('Using new experimental wrapped and ready for export models. To '
+                           'disable it, please set new_experimental_exporter to False when '
+                           'calling keras_post_training_quantization_experimental. '
+                           'If you encounter an issue please file a bug.')
+
             return get_exportable_keras_model(tg)
 
         return export_model(tg,
                             fw_info,
                             fw_impl,
                             tb_w,
                             bit_widths_config)
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/pytorch/quantization_facade.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
     def pytorch_post_training_quantization_experimental(in_module: Module,
                                                         representative_data_gen: Callable,
                                                         target_kpi: KPI = None,
                                                         core_config: CoreConfig = CoreConfig(),
                                                         target_platform_capabilities: TargetPlatformCapabilities = DEFAULT_PYTORCH_TPC,
-                                                        new_experimental_exporter: bool = False):
+                                                        new_experimental_exporter: bool = True):
         """
         Quantize a trained Pytorch module using post-training quantization.
         By default, the module is quantized using a symmetric constraint quantization thresholds
         (power of two) as defined in the default TargetPlatformCapabilities.
         The module is first optimized using several transformations (e.g. BatchNormalization folding to
         preceding layers). Then, using a given dataset, statistics (e.g. min/max, histogram, etc.) are
         being collected for each layer's output (and input, depends on the quantization configuration).
@@ -59,15 +59,15 @@
 
         Args:
             in_module (Module): Pytorch module to quantize.
             representative_data_gen (Callable): Dataset used for calibration.
             target_kpi (KPI): KPI object to limit the search of the mixed-precision configuration as desired.
             core_config (CoreConfig): Configuration object containing parameters of how the model should be quantized, including mixed precision parameters.
             target_platform_capabilities (TargetPlatformCapabilities): TargetPlatformCapabilities to optimize the PyTorch model according to.
-            new_experimental_exporter (bool): Whether exporting the quantized model using new exporter or not (in progress. Avoiding it for now is recommended).
+            new_experimental_exporter (bool): Whether to wrap the quantized model using quantization information or not. Enabled by default. Experimental and subject to future changes.
 
         Returns:
             A quantized module and information the user may need to handle the quantized module.
 
         Examples:
 
             Import a Pytorch module:
@@ -121,16 +121,18 @@
             analyzer_model_quantization(representative_data_gen,
                                         tb_w,
                                         tg,
                                         fw_impl,
                                         DEFAULT_PYTORCH_INFO)
 
         if new_experimental_exporter:
-            Logger.warning('Using new experimental exported models. '
-                           'Please do not use unless you are familiar with what you are doing')
+            Logger.warning('Using new experimental wrapped and ready for export models. To '
+                           'disable it, please set new_experimental_exporter to False when '
+                           'calling pytorch_post_training_quantization_experimental. '
+                           'If you encounter an issue please file a bug.')
 
             return get_exportable_pytorch_model(tg)
 
         quantized_model, user_info = export_model(tg,
                                                   DEFAULT_PYTORCH_INFO,
                                                   fw_impl,
                                                   tb_w,
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/ptq/runner.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/ptq/runner.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,8 +8,7 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.quantizers_infrastructure.constants import THRESHOLD_TENSOR, WEIGHTS_QUANTIZATION_PARAMS
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/common/qat_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/common/qat_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,16 +16,16 @@
 from typing import Dict
 from enum import Enum
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.logger import Logger
 
 
-def _is_qat_applicable(node: common.BaseNode,
-                       fw_info: FrameworkInfo) -> bool:
+def is_qat_applicable(node: common.BaseNode,
+                      fw_info: FrameworkInfo) -> bool:
     """
     A function for deciding if a layer should be fine-tuned during QAT
     Args:
         node (BaseNode): Node for quantization decision
         fw_info (FrameworkInfo): Pytorch quantization information
 
     Returns:
@@ -38,16 +38,20 @@
 
 
 class TrainingMethod(Enum):
     """
     An enum for selecting a QAT training method
 
     STE - Standard straight-through estimator. Includes PowerOfTwo, symmetric & uniform quantizers
+
+    DQA -  DNN Quantization with Attention. Includes a smooth quantization introduces by DQA method
+
     """
     STE = "STE",
+    DQA = "DQA"
 
 
 class QATConfig:
     """
     QAT configuration class.
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantization_facade.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TF
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
+from mct_quantizers import KerasActivationQuantizationHolder, KerasQuantizationWrapper
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.ptq.runner import ptq_runner
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.keras.layers import Layer
@@ -35,46 +36,50 @@
     from model_compression_toolkit.core.keras.keras_implementation import KerasImplementation
     from model_compression_toolkit.core.keras.keras_model_validation import KerasModelValidation
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
 
     from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
 
     from model_compression_toolkit import get_target_platform_capabilities
-    from model_compression_toolkit import quantizers_infrastructure as qi
 
     from model_compression_toolkit import get_target_platform_capabilities
     from model_compression_toolkit.core import common
     from model_compression_toolkit.core.common import BaseNode
     from model_compression_toolkit.constants import TENSORFLOW
     from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-    from model_compression_toolkit.qat.common.qat_config import _is_qat_applicable
+    from model_compression_toolkit.qat.common.qat_config import is_qat_applicable
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
-    from model_compression_toolkit.qat.keras.quantizer.quantization_builder import quantization_builder
+    from model_compression_toolkit.qat.keras.quantizer.quantization_builder import quantization_builder, \
+    get_activation_quantizer_holder
     from model_compression_toolkit.qat.common.qat_config import QATConfig
-    from model_compression_toolkit import quantizers_infrastructure as qi
 
     DEFAULT_KERAS_TPC = get_target_platform_capabilities(TENSORFLOW, DEFAULT_TP_MODEL)
 
 
-    def qat_wrapper(n: common.BaseNode, layer: Layer, qat_config):
+    def qat_wrapper(n: common.BaseNode,
+                    layer: Layer,
+                    qat_config: QATConfig):
         """
         A function which takes a computational graph node and a keras layer and perform the quantization wrapping
         Args:
+            qat_config: Configuration of QAT (such as training methods for example).
             n: A node of mct graph.
-            layer: A keras layer
+            layer: A keras layer.
 
         Returns: Wrapped layer
 
         """
-        if _is_qat_applicable(n, DEFAULT_KERAS_INFO):
-            weights_quantizers, activation_quantizers = quantization_builder(n, qat_config, DEFAULT_KERAS_INFO)
-            return qi.KerasQuantizationWrapper(layer, weights_quantizers, activation_quantizers)
-        else:
-            return layer
+        if is_qat_applicable(n, DEFAULT_KERAS_INFO):
+            weights_quantizers, _ = quantization_builder(n,
+                                                         qat_config,
+                                                         DEFAULT_KERAS_INFO)
+            if len(weights_quantizers) > 0:
+                return KerasQuantizationWrapper(layer, weights_quantizers)
+        return layer
 
 
     def keras_quantization_aware_training_init(in_model: Model,
                                                representative_data_gen: Callable,
                                                target_kpi: KPI = None,
                                                core_config: CoreConfig = CoreConfig(),
                                                qat_config: QATConfig = QATConfig(),
@@ -182,15 +187,19 @@
                                             tpc=target_platform_capabilities,
                                             target_kpi=target_kpi,
                                             tb_w=tb_w)
 
         tg = ptq_runner(tg, representative_data_gen, core_config, fw_info, fw_impl, tb_w)
 
         _qat_wrapper = partial(qat_wrapper, qat_config=qat_config)
-        qat_model, user_info = KerasModelBuilder(graph=tg, fw_info=fw_info, wrapper=_qat_wrapper).build_model()
+        qat_model, user_info = KerasModelBuilder(graph=tg,
+                                                 fw_info=fw_info,
+                                                 wrapper=_qat_wrapper,
+                                                 get_activation_quantizer_holder_fn=partial(get_activation_quantizer_holder,
+                                                                                            qat_config=qat_config)).build_model()
 
         user_info.mixed_precision_cfg = bit_widths_config
         #TODO: remove the last output after updating documentation.
         return qat_model, user_info, {}
 
 
     def keras_quantization_aware_training_finalize(in_model: Model) -> Model:
@@ -243,16 +252,25 @@
              Use the quantized model for fine-tuning. For loading the model from file, use the custom_objects dictionary:
 
              >>> quantized_model = tf.keras.models.load_model(model_file, custom_objects=custom_objects)
              >>> quantized_model = mct.qat.keras_quantization_aware_training_finalize(quantized_model)
 
          """
         def _export(layer):
-            if isinstance(layer, qi.KerasQuantizationWrapper):
-                layer.convert_to_inferable_quantizers()
+            if isinstance(layer, KerasQuantizationWrapper):
+                layer = layer.convert_to_inferable_quantizers()
+            # In the KerasActivationQuantizationHolder case - converting the quantizers only
+            # is not enough. We need to create a new layer with inferable quantizers. The reason for that
+            # is that if we only convert the quantizers, the layer will have some weights (such as min, max,
+            # threshold) that do not match the configuration, thus loading such a model will fail.
+            # To overcome this, the convert_to_inferable_quantizers of KerasActivationQuantizationHolder
+            # creates a new layer from its new configuration after converting the trainable quantizer
+            # to an inferable quantizer.
+            elif isinstance(layer, KerasActivationQuantizationHolder):
+                layer = layer.convert_to_inferable_quantizers()
             return layer
 
         # clone each layer in the model and apply _export to layers with TrainableQuantizeWrappers
         exported_model = tf.keras.models.clone_model(in_model, input_tensors=None, clone_function=_export)
 
         return exported_model
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/base_keras_qat_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 # ==============================================================================
 from typing import Union
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TF
 
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig, BaseKerasTrainableQuantizer
 
 if FOUND_TF:
 
     class BaseKerasQATTrainableQuantizer(BaseKerasTrainableQuantizer):
         """
         A base class for trainable Keras quantizer for QAT.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quant_utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/quantization_builder.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,55 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import Tuple, Dict, List
+from typing import Tuple, Dict, List, Callable
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizer_config import \
+from model_compression_toolkit.core.keras.default_framework_info import DEFAULT_KERAS_INFO
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.qat.common.qat_config import QATConfig
+from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
+from mct_quantizers import QuantizationTarget, KerasActivationQuantizationHolder
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizer_config import \
     get_trainable_quantizer_weights_config, get_trainable_quantizer_activation_config, \
     get_trainable_quantizer_quantization_candidates
-from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
-from model_compression_toolkit.qat.common.qat_config import QATConfig
-from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizers import \
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizers import \
     get_trainable_quantizer_class
 
 
+def get_activation_quantizer_holder(n: common.BaseNode,
+                                    qat_config: QATConfig) -> Callable:
+    """
+    Retrieve a KerasActivationQuantizationHolder layer to use for activation quantization for a node.
+    If the layer is not supposed to be wrapped with activation quantizers - return None.
+
+    Args:
+        n: Node to get KerasActivationQuantizationHolder to attach in its output.
+        qat_config: Configuration of QAT (such as training methods for example).
+
+    Returns:
+        A KerasActivationQuantizationHolder layer for the node activation quantization.
+    """
+    _, activation_quantizers = quantization_builder(n,
+                                                    qat_config,
+                                                    DEFAULT_KERAS_INFO)
+
+    # Holder by definition uses a single quantizer for the activation quantization
+    # thus we make sure this is the only possible case (unless it's a node with no activation
+    # quantization, which in this case has an empty list).
+    if len(activation_quantizers) == 1:
+        return KerasActivationQuantizationHolder(activation_quantizers[0])
+    Logger.error(f'KerasActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers were found for node {n}')
+
+
 def quantization_builder(n: common.BaseNode,
                          qat_config: QATConfig,
                          fw_info: FrameworkInfo,
                          ) -> Tuple[Dict[str, BaseKerasQATTrainableQuantizer], List[BaseKerasQATTrainableQuantizer]]:
     """
     Build quantizers for a node according to its quantization configuration.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,33 +15,32 @@
 
 from typing import Union
 
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.framework.tensor_shape import TensorShape
 from model_compression_toolkit.constants import SIGNED
-from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.trainable_infrastructure.common.constants import FQ_MIN, FQ_MAX
 
 from model_compression_toolkit.qat import TrainingMethod
 
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import QuantizationTarget, mark_quantizer, KerasQuantizationWrapper
 from model_compression_toolkit.qat.common import THRESHOLD_TENSOR
-from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+from model_compression_toolkit import constants as C
 
 from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
-    WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, ActivationPOTInferableQuantizer, \
-    ActivationSymmetricInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from mct_quantizers.keras.quantizers import WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, \
+    ActivationPOTInferableQuantizer, ActivationSymmetricInferableQuantizer
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=TrainingMethod.STE)
 class STEWeightQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer inputs.
     """
 
@@ -80,15 +79,15 @@
         self.min = delta * min_int
         self.max = delta * max_int
 
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper):
+                                layer: KerasQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
@@ -167,15 +166,15 @@
             return WeightsSymmetricInferableQuantizer(num_bits=self.num_bits,
                                                       threshold=list(self.get_quantizer_variable(THRESHOLD_TENSOR).numpy().flatten()),
                                                       per_channel=self.per_channel,
                                                       channel_axis=self.channel_axis,
                                                       input_rank=len(self.threshold_shape))
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Activation,
+@mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=TrainingMethod.STE)
 class STEActivationQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer outputs.
     """
 
@@ -202,15 +201,15 @@
         max_int = (2 ** (self.num_bits - int(self.signed))) - 1
         self.min = delta * min_int
         self.max = delta * max_int
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper):
+                                layer: KerasQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/keras/quantizer/ste_rounding/uniform_ste.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,33 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 import tensorflow as tf
 from tensorflow.python.framework.tensor_shape import TensorShape
 from model_compression_toolkit.constants import RANGE_MIN, RANGE_MAX
-from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.trainable_infrastructure.common.constants import FQ_MIN, FQ_MAX
 from model_compression_toolkit.qat import TrainingMethod
-from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+
+from mct_quantizers import mark_quantizer, QuantizationMethod, QuantizationTarget, KerasQuantizationWrapper
+from mct_quantizers.keras.quantizers import \
+    BaseKerasInferableQuantizer, WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
 
 from model_compression_toolkit.qat.keras.quantizer.quant_utils import adjust_range_to_include_zero
 from model_compression_toolkit.core.common.quantization.quantizers.quantizers_helpers import fix_range_to_include_zero
-from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+from model_compression_toolkit import constants as C
 
 from model_compression_toolkit.qat.keras.quantizer.base_keras_qat_quantizer import BaseKerasQATTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import \
-    mark_quantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers import \
-    BaseKerasInferableQuantizer, WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=TrainingMethod.STE)
 class STEUniformWeightQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer inputs.
     """
 
@@ -69,15 +68,15 @@
             self.perm_vec[len(self.min_max_shape) - 1] = self.channel_axis
         else:
             self.perm_vec = None
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper):
+                                layer: KerasQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
@@ -144,15 +143,15 @@
                                                 min_range=list(min_range.flatten()),
                                                 max_range=list(max_range.flatten()),
                                                 per_channel=self.per_channel,
                                                 channel_axis=self.channel_axis,
                                                 input_rank=len(self.min_max_shape))
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Activation,
+@mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=TrainingMethod.STE)
 class STEUniformActivationQATQuantizer(BaseKerasQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer outputs.
     """
 
@@ -169,15 +168,15 @@
         self.num_bits = quantization_config.activation_n_bits
         self.min_range = quantization_config.activation_quantization_params[C.RANGE_MIN]
         self.max_range = quantization_config.activation_quantization_params[C.RANGE_MAX]
 
     def initialize_quantization(self,
                                 tensor_shape: TensorShape,
                                 name: str,
-                                layer: qi.KerasQuantizationWrapper):
+                                layer: KerasQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantization_facade.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantization_facade.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,50 +21,54 @@
 from model_compression_toolkit.core import CoreConfig
 from model_compression_toolkit.core import common
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.core.common.framework_info import FrameworkInfo
 from model_compression_toolkit.core.common.mixed_precision.kpi_tools.kpi import KPI
 from model_compression_toolkit.core.common.mixed_precision.mixed_precision_quantization_config import \
     MixedPrecisionQuantizationConfigV2
-from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import TargetPlatformCapabilities
+from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import \
+    TargetPlatformCapabilities
 from model_compression_toolkit.core.runner import core_runner, _init_tensorboard_writer
 from model_compression_toolkit.ptq.runner import ptq_runner
 
-
 if FOUND_TORCH:
     import torch.nn as nn
     from torch.nn import Module
+    from mct_quantizers import PytorchActivationQuantizationHolder
     from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
     from model_compression_toolkit.target_platform_capabilities.constants import DEFAULT_TP_MODEL
     from model_compression_toolkit.core.pytorch.pytorch_implementation import PytorchImplementation
-    from model_compression_toolkit.qat.common.qat_config import _is_qat_applicable
+    from model_compression_toolkit.qat.common.qat_config import is_qat_applicable
     from model_compression_toolkit.core.pytorch.back2framework.pytorch_model_builder import PyTorchModelBuilder
-    from model_compression_toolkit.quantizers_infrastructure import PytorchQuantizationWrapper
-    from model_compression_toolkit import quantizers_infrastructure as qi
+    from mct_quantizers import PytorchQuantizationWrapper
     from model_compression_toolkit import get_target_platform_capabilities
     from model_compression_toolkit.qat.common.qat_config import QATConfig
+    from model_compression_toolkit.qat.pytorch.quantizer.quantization_builder import get_activation_quantizer_holder
     from model_compression_toolkit.qat.pytorch.quantizer.quantization_builder import quantization_builder
+
     DEFAULT_PYTORCH_TPC = get_target_platform_capabilities(PYTORCH, DEFAULT_TP_MODEL)
 
 
-    def qat_wrapper(n: common.BaseNode, module: nn.Module, qat_config: QATConfig):
+    def qat_wrapper(n: common.BaseNode,
+                    module: nn.Module,
+                    qat_config: QATConfig):
         """
         A function which takes a computational graph node and a pytorch module and perform the quantization wrapping
         Args:
             n: A node of mct graph.
             module: A Pytorch module
             qat_config (QATConfig): QAT configuration
         Returns: Wrapped layer
 
         """
-        if _is_qat_applicable(n, DEFAULT_PYTORCH_INFO):
-            weights_quantizers, activation_quantizers = quantization_builder(n, qat_config, DEFAULT_PYTORCH_INFO)
-            return qi.PytorchQuantizationWrapper(module, weights_quantizers, activation_quantizers)
-        else:
-            return module
+        if is_qat_applicable(n, DEFAULT_PYTORCH_INFO):
+            weights_quantizers, _ = quantization_builder(n, qat_config, DEFAULT_PYTORCH_INFO)
+            if len(weights_quantizers) > 0:
+                return PytorchQuantizationWrapper(module, weights_quantizers)
+        return module
 
 
     def pytorch_quantization_aware_training_init(in_model: Module,
                                                  representative_data_gen: Callable,
                                                  target_kpi: KPI = None,
                                                  core_config: CoreConfig = CoreConfig(),
                                                  qat_config: QATConfig = QATConfig(),
@@ -131,19 +135,19 @@
              For more configuration options, please take a look at our `API documentation <https://sony.github.io/model_optimization/api/api_docs/modules/mixed_precision_quantization_config.html>`_.
 
          """
 
         if core_config.mixed_precision_enable:
             if not isinstance(core_config.mixed_precision_config, MixedPrecisionQuantizationConfigV2):
                 Logger.error("Given quantization config to mixed-precision facade is not of type "
-                                    "MixedPrecisionQuantizationConfigV2. Please use pytorch_post_training_quantization API,"
-                                    "or pass a valid mixed precision configuration.")
+                             "MixedPrecisionQuantizationConfigV2. Please use pytorch_post_training_quantization API,"
+                             "or pass a valid mixed precision configuration.")
 
             Logger.info("Using experimental mixed-precision quantization. "
-                               "If you encounter an issue please file a bug.")
+                        "If you encounter an issue please file a bug.")
 
         tb_w = _init_tensorboard_writer(fw_info)
 
         fw_impl = PytorchImplementation()
 
         tg, bit_widths_config = core_runner(in_model=in_model,
                                             representative_data_gen=representative_data_gen,
@@ -154,20 +158,29 @@
                                             target_kpi=target_kpi,
                                             tb_w=tb_w)
 
         tg = ptq_runner(tg, representative_data_gen, core_config, fw_info, fw_impl, tb_w)
 
         _qat_wrapper = partial(qat_wrapper, qat_config=qat_config)
 
-        qat_model, user_info = PyTorchModelBuilder(graph=tg, fw_info=fw_info, wrapper=_qat_wrapper).build_model()
+        qat_model, user_info = PyTorchModelBuilder(graph=tg,
+                                                   fw_info=fw_info,
+                                                   wrapper=_qat_wrapper,
+                                                   get_activation_quantizer_holder_fn=partial(
+                                                       get_activation_quantizer_holder,
+                                                       qat_config=qat_config)).build_model()
 
         user_info.mixed_precision_cfg = bit_widths_config
 
+        # Remove fw_info from graph to enable saving the pytorch model (fw_info can not be pickled)
+        delattr(qat_model.graph, 'fw_info')
+
         return qat_model, user_info
 
+
     def pytorch_quantization_aware_training_finalize(in_model: Module):
         """
          Convert a model fine-tuned by the user to a network with QuantizeWrappers containing
          InferableQuantizers, that quantizes both the layers weights and outputs
 
          Args:
              in_model (Model): Pytorch model to remove QuantizeWrappers.
@@ -201,27 +214,27 @@
              >>> quantized_model, quantization_info = pytorch_quantization_aware_training_init(model, repr_datagen, core_config=config)
 
              Use the quantized model for fine-tuning. Finally, remove the quantizer wrappers and keep a quantize model ready for inference.
 
              >>> quantized_model = mct.pytorch_quantization_aware_training_finalize(quantized_model)
 
          """
-        exported_model = copy.deepcopy(in_model)
-        for _, layer in exported_model.named_children():
-            if isinstance(layer, PytorchQuantizationWrapper):
+        for _, layer in in_model.named_children():
+            if isinstance(layer, (PytorchQuantizationWrapper, PytorchActivationQuantizationHolder)):
                 layer.convert_to_inferable_quantizers()
 
-        return exported_model
+        return in_model
 
 
 else:
     # If torch is not installed,
     # we raise an exception when trying to use these functions.
     def pytorch_quantization_aware_training_init(*args, **kwargs):
         Logger.critical('Installing Pytorch is mandatory '
                         'when using pytorch_quantization_aware_training_init. '
                         'Could not find the torch package.')  # pragma: no cover
 
+
     def pytorch_quantization_aware_training_finalize(*args, **kwargs):
         Logger.critical('Installing Pytorch is mandatory '
                         'when using pytorch_quantization_aware_training_finalize. '
                         'Could not find the torch package.')  # pragma: no cover
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/base_pytorch_qat_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 # limitations under the License.
 # ==============================================================================
 from typing import Union
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TORCH
 
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
+from model_compression_toolkit.trainable_infrastructure.pytorch.base_pytorch_quantizer import \
     BasePytorchTrainableQuantizer
 
 if FOUND_TORCH:
 
     class BasePytorchQATTrainableQuantizer(BasePytorchTrainableQuantizer):
         """
         A base class for trainable Keras quantizer for QAT.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/exporter/model_wrapper/keras/builder/fully_quantized_model_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,67 +8,87 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from typing import List, Dict, Tuple
 
+from typing import Tuple, Callable
 from model_compression_toolkit.core import common
-from model_compression_toolkit.core.common.framework_info import FrameworkInfo
-from model_compression_toolkit.qat.common.qat_config import QATConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizer_config import \
-    get_trainable_quantizer_quantization_candidates, get_trainable_quantizer_weights_config, \
-    get_trainable_quantizer_activation_config
-from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.get_quantizers import \
-    get_trainable_quantizer_class
-
-
-def quantization_builder(n: common.BaseNode,
-                         qat_config: QATConfig,
-                         fw_info: FrameworkInfo,
-                         ) -> Tuple[Dict[str, BasePytorchQATTrainableQuantizer],
-                                    List[BasePytorchQATTrainableQuantizer]]:
-    """
-    Build quantizers for a node according to its quantization configuration.
-
-    Args:
-        n: Node to build its QuantizeConfig.
-        qat_config (QATConfig): QAT configuration
-        fw_info: Framework information (e.g., mapping from layers to their attributes to quantize).
-
-    Returns:
-        weights_quantizers: A dictionary between a weight's name to its quantizer.
-        activation_quantizers: A list of activations quantization, one for each layer output.).
-    """
-    if len(n.candidates_quantization_cfg) > 1:
-        wq_cand, aq_cand = get_trainable_quantizer_quantization_candidates(n)
-    else:
-        wq_cand, aq_cand = None, None
-
-    weight_quantizers = {}
-    if n.is_weights_quantization_enabled():
-        quant_method = n.final_weights_quantization_cfg.weights_quantization_method
-        quantizer_class = get_trainable_quantizer_class(QuantizationTarget.Weights,
-                                                        qat_config.weight_training_method,
-                                                        quant_method,
-                                                        BasePytorchQATTrainableQuantizer)
-        attributes = fw_info.get_kernel_op_attributes(n.type)
-        for attr in attributes:
-            weight_quantizers.update({attr: quantizer_class(get_trainable_quantizer_weights_config(n, wq_cand),
-                                                           **qat_config.weight_quantizer_params_override)})
-
-    activation_quantizers = []
-    if n.is_activation_quantization_enabled():
-        quant_method = n.final_activation_quantization_cfg.activation_quantization_method
-        quantizer_class = get_trainable_quantizer_class(QuantizationTarget.Activation,
-                                                        qat_config.activation_training_method,
-                                                        quant_method,
-                                                        BasePytorchQATTrainableQuantizer)
-
-        activation_quantizers = [quantizer_class(get_trainable_quantizer_activation_config(n, aq_cand),
-                                                 **qat_config.activation_quantizer_params_override)]
-
-    return weight_quantizers, activation_quantizers
+from model_compression_toolkit.core.common import Graph
+from model_compression_toolkit.constants import FOUND_TF
+from model_compression_toolkit.core.common.user_info import UserInformation
+from model_compression_toolkit.logger import Logger
+from mct_quantizers import KerasActivationQuantizationHolder
+
+if FOUND_TF:
+    import tensorflow as tf
+    from tensorflow.keras.layers import Layer
+    from model_compression_toolkit.core.keras.back2framework.keras_model_builder import KerasModelBuilder
+    from model_compression_toolkit.exporter.model_wrapper.keras.builder.node_to_quantizers import get_quantization_quantizers
+    from mct_quantizers import KerasQuantizationWrapper
+
+    def _get_wrapper(node: common.BaseNode,
+                     layer: Layer) -> Layer:
+        """
+        A function which takes a computational graph node and a keras layer and perform the quantization wrapping
+        Args:
+            node: A node of mct graph.
+            layer: A keras layer
+
+        Returns: Wrapped layer with weights quantizers and activation quantizers
+
+        """
+        weights_quantizers, _ = get_quantization_quantizers(node)
+        if len(weights_quantizers) > 0:
+            return KerasQuantizationWrapper(layer,
+                                            weights_quantizers)
+        return layer
+
+
+    def get_activation_quantizer_holder(node: common.BaseNode) -> Callable:
+        """
+        Retrieve a ActivationQuantizationHolder layer to use for activation quantization for a node.
+
+        Args:
+            node: Node to get ActivationQuantizationHolder to attach in its output.
+
+        Returns:
+            A ActivationQuantizationHolder layer for the node activation quantization.
+        """
+        _, activation_quantizers = get_quantization_quantizers(node)
+
+        # Holder by definition uses a single quantizer for the activation quantization
+        # thus we make sure this is the only possible case (unless it's a node with no activation
+        # quantization, which in this case has an empty list).
+        if len(activation_quantizers) == 1:
+            return KerasActivationQuantizationHolder(activation_quantizers[0])
+
+        Logger.error(
+            f'ActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers '
+            f'were found for node {node}')
+
+
+
+    def get_exportable_keras_model(graph: Graph) -> Tuple[tf.keras.models.Model, UserInformation]:
+        """
+        Convert graph to an exportable Keras model (model with all quantization parameters).
+        An exportable model can then be exported using model_exporter, to retrieve the
+        final exported model.
+
+        Args:
+            graph: Graph to convert to an exportable Keras model.
+
+        Returns:
+            Exportable Keras model and user information.
+        """
+        exportable_model, user_info = KerasModelBuilder(graph=graph,
+                                                        wrapper=_get_wrapper,
+                                                        get_activation_quantizer_holder_fn=get_activation_quantizer_holder).build_model()
+        exportable_model.trainable = False
+        return exportable_model, user_info
+else:
+    def get_exportable_keras_model(*args, **kwargs):  # pragma: no cover
+        Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+                     'when using get_exportable_keras_model. '
+                     'Could not find Tensorflow package.')
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/symmetric_ste.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,30 +16,31 @@
 
 import numpy as np
 import torch
 import torch.nn as nn
 
 from model_compression_toolkit.qat import TrainingMethod
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
+from mct_quantizers import PytorchQuantizationWrapper
 from model_compression_toolkit.qat.common import THRESHOLD_TENSOR
-from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+from model_compression_toolkit import constants as C
 from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
 
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.qat.pytorch.quantizer.quantizer_utils import ste_round, ste_clip, symmetric_quantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
+from mct_quantizers.pytorch.quantizers import \
     WeightsPOTInferableQuantizer, WeightsSymmetricInferableQuantizer, ActivationPOTInferableQuantizer, \
     ActivationSymmetricInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
+from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=TrainingMethod.STE)
 class STEWeightQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer weights.
     """
 
@@ -69,15 +70,15 @@
         self.min = delta * self.min_int
         self.max = delta * self.max_int
 
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
@@ -125,15 +126,15 @@
             return WeightsSymmetricInferableQuantizer(num_bits=self.num_bits,
                                                       threshold=np_threshold,
                                                       per_channel=self.quantization_config.weights_per_channel_threshold,
                                                       channel_axis=self.quantization_config.weights_channels_axis)
 
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Activation,
+@mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.POWER_OF_TWO, QuantizationMethod.SYMMETRIC],
                 quantizer_type=TrainingMethod.STE)
 class STEActivationQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer activations.
     """
 
@@ -151,15 +152,15 @@
         np_threshold_values = quantization_config.activation_quantization_params[C.THRESHOLD]
         self.threshold_tensor = torch.Tensor([np_threshold_values])
         self.num_bits = quantization_config.activation_n_bits
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/ste_rounding/uniform_ste.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,32 +14,33 @@
 # ==============================================================================
 import numpy as np
 import torch
 import torch.nn as nn
 from torch import Tensor
 
 from model_compression_toolkit.constants import RANGE_MAX, RANGE_MIN
-from model_compression_toolkit.quantizers_infrastructure.constants import FQ_MIN, FQ_MAX
+from model_compression_toolkit.trainable_infrastructure.common.constants import FQ_MIN, FQ_MAX
 
 from model_compression_toolkit.qat import TrainingMethod
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit import quantizers_infrastructure as qi, constants as C
+from mct_quantizers import QuantizationTarget, PytorchQuantizationWrapper
+from model_compression_toolkit import constants as C
 
 from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import mark_quantizer
+from mct_quantizers import mark_quantizer
 from model_compression_toolkit.core.pytorch.utils import to_torch_tensor
 from model_compression_toolkit.qat.pytorch.quantizer.quantizer_utils import uniform_quantizer
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers import \
+from mct_quantizers.pytorch.quantizers import \
     WeightsUniformInferableQuantizer, ActivationUniformInferableQuantizer
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
+from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Weights,
+@mark_quantizer(quantization_target=QuantizationTarget.Weights,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=TrainingMethod.STE)
 class STEUniformWeightQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer inputs.
     """
 
@@ -65,15 +66,15 @@
                               [-1]) if self.quantization_config.weights_per_channel_threshold else float(
             self.min_values)
 
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
@@ -113,15 +114,15 @@
 
         return WeightsUniformInferableQuantizer(num_bits=self.num_bits,
                                                 min_range=_min, max_range=_max,
                                                 per_channel=self.quantization_config.weights_per_channel_threshold,
                                                 channel_axis=self.quantization_config.weights_channels_axis)
 
 
-@mark_quantizer(quantization_target=qi.QuantizationTarget.Activation,
+@mark_quantizer(quantization_target=QuantizationTarget.Activation,
                 quantization_method=[QuantizationMethod.UNIFORM],
                 quantizer_type=TrainingMethod.STE)
 class STEUniformActivationQATQuantizer(BasePytorchQATTrainableQuantizer):
     """
     Trainable constrained quantizer to quantize a layer activations.
     """
 
@@ -140,15 +141,15 @@
         self.min_range_tensor = torch.Tensor([np_min_range])
         self.max_range_tensor = torch.Tensor([np_max_range])
         self.num_bits = quantization_config.activation_n_bits
 
     def initialize_quantization(self,
                                 tensor_shape: torch.Size,
                                 name: str,
-                                layer: qi.PytorchQuantizationWrapper):
+                                layer: PytorchQuantizationWrapper):
         """
         Add quantizer parameters to the quantizer parameters dictionary
 
         Args:
             tensor_shape: tensor shape of the quantized tensor.
             name: Tensor name.
             layer: Layer to quantize.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/constants.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/common/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/load_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/load_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,71 +1,64 @@
-# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from model_compression_toolkit.logger import Logger
+from typing import Any
+
+import mct_quantizers
+from mct_quantizers.common.get_all_subclasses import get_all_subclasses
+
 from model_compression_toolkit.constants import FOUND_TF
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_all_subclasses import get_all_subclasses
+from model_compression_toolkit.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
-    from model_compression_toolkit import quantizers_infrastructure as qi
-    from model_compression_toolkit.quantizers_infrastructure import BaseKerasTrainableQuantizer
-    from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.keras.quantizers.base_keras_inferable_quantizer \
-        import \
-        BaseKerasInferableQuantizer
+    from tensorflow.python.saved_model.load_options import LoadOptions
+    from model_compression_toolkit.trainable_infrastructure import BaseKerasTrainableQuantizer
     keras = tf.keras
 
-    def keras_load_quantized_model(filepath, custom_objects=None, compile=True, options=None):
+    def keras_load_quantized_model(filepath: str, custom_objects: Any = None, compile: bool = True,
+                                   options: LoadOptions = None):
         """
-        This function wraps the keras load model and MCT quantization custom class to it.
+        This function wraps the keras load model and adds trainable quantizers classes to its custom objects.
 
         Args:
             filepath: the model file path.
             custom_objects: Additional custom objects
             compile: Boolean, whether to compile the model after loading.
             options: Optional `tf.saved_model.LoadOptions` object that specifies options for loading from SavedModel.
 
         Returns: A keras Model
 
         """
-        qi_inferable_custom_objects = {subclass.__name__: subclass for subclass in
-                                       get_all_subclasses(BaseKerasInferableQuantizer)}
-        all_inferable_names = list(qi_inferable_custom_objects.keys())
-        if len(set(all_inferable_names)) < len(all_inferable_names):
-            Logger.error(f"Found multiple quantizers with the same name that inherit from BaseKerasInferableQuantizer"
-                         f"while trying to load a model.")
 
         qi_trainable_custom_objects = {subclass.__name__: subclass for subclass in
                                        get_all_subclasses(BaseKerasTrainableQuantizer)}
         all_trainable_names = list(qi_trainable_custom_objects.keys())
         if len(set(all_trainable_names)) < len(all_trainable_names):
             Logger.error(f"Found multiple quantizers with the same name that inherit from BaseKerasTrainableQuantizer"
                          f"while trying to load a model.")
 
-        # Merge dictionaries into one dict
-        qi_custom_objects = {**qi_inferable_custom_objects, **qi_trainable_custom_objects}
+        qi_custom_objects = {**qi_trainable_custom_objects}
 
-        # Add non-quantizers custom objects
-        qi_custom_objects.update({qi.KerasQuantizationWrapper.__name__: qi.KerasQuantizationWrapper})
         if custom_objects is not None:
             qi_custom_objects.update(custom_objects)
-        return tf.keras.models.load_model(filepath,
-                                          custom_objects=qi_custom_objects, compile=compile,
-                                          options=options)
+        return mct_quantizers.keras_load_quantized_model(filepath,
+                                                         custom_objects=qi_custom_objects, compile=compile,
+                                                         options=options)
 else:
     def keras_load_quantized_model(filepath, custom_objects=None, compile=True, options=None):
         """
         This function wraps the keras load model and MCT quantization custom class to it.
 
         Args:
             filepath: the model file path.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/immutable.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,53 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from abc import abstractmethod
-
-from model_compression_toolkit.constants import FOUND_TF
-from model_compression_toolkit.quantizers_infrastructure import BaseInferableQuantizer
-
-if FOUND_TF:
-    import tensorflow as tf
-
-    class BaseKerasInferableQuantizer(BaseInferableQuantizer):
-        def __init__(self):
-            """
-            This class is a base quantizer for Keras quantizers for inference only.
-            """
-            super(BaseKerasInferableQuantizer, self).__init__()
-
-        @abstractmethod
-        def get_config(self):
-            """
-            Return a dictionary with the configuration of the quantizer.
-            """
-            raise NotImplemented(f'{self.__class__.__name__} did not implement get_config')  # pragma: no cover
-
-        @abstractmethod
-        def __call__(self, inputs: tf.Tensor):
-            """
-            Quantize the given inputs using the quantizer parameters.
-
-            Args:
-                inputs: input tensor to quantize
-
-            Returns:
-                quantized tensor.
-            """
-            raise NotImplemented(f'{self.__class__.__name__} did not implement __call__')  # pragma: no cover
-else:
-    class BaseKerasInferableQuantizer:  # pragma: no cover
-        def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
-                            'when using BaseKerasInferableQuantizer. '
-                            'Could not find Tensorflow package.')
+from typing import Any
 
 
+class ImmutableClass(object):
+    """
+    Class to make inherits classes immutable.
+    """
+    _initialized = False
+
+    def __init__(self):
+        self._initialized = False
+
+    def __setattr__(self,
+                    *args: Any,
+                    **kwargs: Any):
+        """
+        Use this method to enforce immutability when object is finalized.
+
+        Args:
+            *args: Arguments to set to attribute.
+            **kwargs: Keyword-arguments to set to attribute.
+
+        """
+        if self._initialized:
+            raise Exception('Immutable class. Can\'t edit attributes')
+        else:
+            object.__setattr__(self,
+                               *args,
+                               **kwargs)
+
+    def initialized_done(self):
+        """
+
+        Method to use when object should be immutable.
+
+        """
+        if self._initialized:
+            raise Exception('reinitialized')  # Can not get finalized again.
+        self._initialized = True  # Finalize object.
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/constants.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,17 +9,19 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-# Inferable keras quantizer signature parameters:
-NUM_BITS = 'num_bits'
-SIGNED = 'signed'
-THRESHOLD = 'threshold'
-PER_CHANNEL = 'per_channel'
-MIN_RANGE = 'min_range'
-MAX_RANGE = 'max_range'
-CHANNEL_AXIS = 'channel_axis'
-INPUT_RANK = 'input_rank'
-CLUSTER_CENTERS = 'cluster_centers'
+# TP Model constants
+OPS_SET_LIST = 'ops_set_list'
+
+# Version
+LATEST = 'latest'
+
+
+# Supported TP models names:
+DEFAULT_TP_MODEL = 'default'
+IMX500_TP_MODEL = 'imx500'
+TFLITE_TP_MODEL = 'tflite'
+QNNPACK_TP_MODEL = 'qnnpack'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
+__version__ = 'v2'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
+__version__ = 'v5'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/inferable_infrastructure/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/pytorch/quantizer/quantization_builder.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,106 +1,101 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from typing import List, Dict, Tuple, Callable
 
-import numpy as np
+from mct_quantizers import PytorchActivationQuantizationHolder, QuantizationTarget
 
-from model_compression_toolkit.constants import FOUND_TORCH
-from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer \
-    import mark_quantizer, \
-    QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
-    import MULTIPLIER_N_BITS, EPS
-
-if FOUND_TORCH:
-    import torch
-    from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizer_utils \
-        import to_torch_tensor, get_working_device, lut_quantizer
-    from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.pytorch.quantizers \
-        .base_lut_symmetric_inferable_quantizer import BaseLUTSymmetricInferableQuantizer
-
-
-    @mark_quantizer(quantization_target=QuantizationTarget.Weights,
-                    quantization_method=[QuantizationMethod.LUT_SYM_QUANTIZER],
-                    quantizer_type=None)
-    class WeightsLUTSymmetricInferableQuantizer(BaseLUTSymmetricInferableQuantizer):
-        """
-        Class for quantizing weights using a lut symmetric quantizer
-        """
-
-        def __init__(self,
-                     num_bits: int,
-                     cluster_centers: np.ndarray,
-                     threshold: np.ndarray,
-                     per_channel: bool,
-                     channel_axis: int = None,
-                     multiplier_n_bits: int = MULTIPLIER_N_BITS,
-                     eps: float = EPS):
-            """
-            Initialize the quantizer with the specified parameters.
-
-            Args:
-                num_bits: number of bits to use for quantization
-                cluster_centers: the cluster centers to assign the weights
-                threshold: threshold for quantizing weights
-                per_channel: whether to use per-channel quantization
-                channel_axis: Axis of input to apply per-channel quantization on
-                multiplier_n_bits: Number of bits that determines the quantization range
-                eps: Small value for numerical stability in division
-            """
-
-            super(WeightsLUTSymmetricInferableQuantizer, self).__init__(threshold=threshold,
-                                                                        num_bits=num_bits,
-                                                                        cluster_centers=cluster_centers,
-                                                                        signed=True,
-                                                                        multiplier_n_bits=multiplier_n_bits,
-                                                                        eps=eps)
-
-            if per_channel:
-                assert channel_axis is not None, f'Channel axis is missing in per channel quantization'
-                assert len(
-                    threshold) >= 1, f'In per-channel quantization threshold should be of length >= 1 but is ' \
-                                     f'{len(threshold)}'
-            else:
-                assert len(
-                    threshold) == 1, f'In per-tensor quantization threshold should be of length 1 but is ' \
-                                     f'{len(threshold)}'
-
-            self.per_channel = per_channel
-            self.channel_axis = channel_axis
-
-            self.threshold = to_torch_tensor(self.threshold).to(get_working_device())
-            self.cluster_centers = to_torch_tensor(self.cluster_centers).to(get_working_device())
-
-        def __call__(self, inputs: torch.Tensor) -> torch.Tensor:
-            """
-            Quantize the given inputs using the quantizer parameters.
-
-            Args:
-                inputs: input tensor to quantize
-
-            Returns:
-                quantized tensor.
-            """
-            inputs.requires_grad = False
-            return lut_quantizer(inputs, cluster_centers=self.cluster_centers, signed=True,
-                                 threshold=self.threshold, multiplier_n_bits=self.multiplier_n_bits, eps=self.eps)
-
-
-else:
-    class WeightsLUTSymmetricInferableQuantizer:  # pragma: no cover
-        def __init__(self, *args, **kwargs):
-            raise Exception('Installing torch is mandatory '
-                            'when using WeightsLUTSymmetricInferableQuantizer. '
-                            'Could not find torch package.')
+from model_compression_toolkit.core import common
+from model_compression_toolkit.core.common.framework_info import FrameworkInfo
+from model_compression_toolkit.qat.common.qat_config import QATConfig
+from model_compression_toolkit.core.pytorch.default_framework_info import DEFAULT_PYTORCH_INFO
+from model_compression_toolkit.logger import Logger
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizer_config import \
+    get_trainable_quantizer_quantization_candidates, get_trainable_quantizer_weights_config, \
+    get_trainable_quantizer_activation_config
+from model_compression_toolkit.qat.pytorch.quantizer.base_pytorch_qat_quantizer import BasePytorchQATTrainableQuantizer
+from model_compression_toolkit.trainable_infrastructure.common.get_quantizers import \
+    get_trainable_quantizer_class
+
+def get_activation_quantizer_holder(n: common.BaseNode,
+                                    qat_config: QATConfig) -> Callable:
+    """
+    Retrieve a ActivationQuantizationHolder layer to use for activation quantization for a node.
+    If the layer is not supposed to be wrapped with activation quantizers - return None.
+
+    Args:
+        n: Node for which to retrieve anActivationQuantizationHolder to attach to its output.
+        qat_config: QAT configuration (for example, training methods).
+
+    Returns:
+        A ActivationQuantizationHolder layer for the node's activation quantization.
+    """
+    _, activation_quantizers = quantization_builder(n,
+                                                    qat_config,
+                                                    DEFAULT_PYTORCH_INFO)
+
+    # Holder by definition uses a single quantizer for the activation quantization
+    # thus we make sure this is the only possible case (unless it's a node with no activation
+    # quantization, which in this case has an empty list).
+    if len(activation_quantizers) == 1:
+        return PytorchActivationQuantizationHolder(activation_quantizers[0])
+    Logger.error(f'ActivationQuantizationHolder supports a single quantizer but {len(activation_quantizers)} quantizers were found for node {n}')
+
+
+def quantization_builder(n: common.BaseNode,
+                         qat_config: QATConfig,
+                         fw_info: FrameworkInfo,
+                         ) -> Tuple[Dict[str, BasePytorchQATTrainableQuantizer],
+                                    List[BasePytorchQATTrainableQuantizer]]:
+    """
+    Build quantizers for a node according to its quantization configuration.
+
+    Args:
+        n: Node to build its QuantizeConfig.
+        qat_config (QATConfig): QAT configuration
+        fw_info: Framework information (e.g., mapping from layers to their attributes to quantize).
+
+    Returns:
+        weights_quantizers: A dictionary between a weight's name to its quantizer.
+        activation_quantizers: A list of activations quantization, one for each layer output.).
+    """
+    if len(n.candidates_quantization_cfg) > 1:
+        wq_cand, aq_cand = get_trainable_quantizer_quantization_candidates(n)
+    else:
+        wq_cand, aq_cand = None, None
+
+    weight_quantizers = {}
+    if n.is_weights_quantization_enabled():
+        quant_method = n.final_weights_quantization_cfg.weights_quantization_method
+        quantizer_class = get_trainable_quantizer_class(QuantizationTarget.Weights,
+                                                        qat_config.weight_training_method,
+                                                        quant_method,
+                                                        BasePytorchQATTrainableQuantizer)
+        attributes = fw_info.get_kernel_op_attributes(n.type)
+        for attr in attributes:
+            weight_quantizers.update({attr: quantizer_class(get_trainable_quantizer_weights_config(n, wq_cand),
+                                                           **qat_config.weight_quantizer_params_override)})
+
+    activation_quantizers = []
+    if n.is_activation_quantization_enabled():
+        quant_method = n.final_activation_quantization_cfg.activation_quantization_method
+        quantizer_class = get_trainable_quantizer_class(QuantizationTarget.Activation,
+                                                        qat_config.activation_training_method,
+                                                        quant_method,
+                                                        BasePytorchQATTrainableQuantizer)
+
+        activation_quantizers = [quantizer_class(get_trainable_quantizer_activation_config(n, aq_cand),
+                                                 **qat_config.activation_quantizer_params_override)]
+
+    return weight_quantizers, activation_quantizers
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,8 +7,10 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
+
+__version__ = 'v1'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
+
+__version__ = 'v3'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/base_trainable_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/base_trainable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from enum import Enum
 from typing import Union, List, Any
 from inspect import signature
 
 from model_compression_toolkit.core import common
 from model_compression_toolkit.logger import Logger
 
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.base_inferable_quantizer import BaseInferableQuantizer, \
+from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer, \
     QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
+from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerActivationConfig, TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants import QUANTIZATION_METHOD, \
+from mct_quantizers.common.constants import QUANTIZATION_METHOD, \
     QUANTIZATION_TARGET
 
 
 VAR = 'var'
 GROUP = 'group'
 
 class VariableGroup(Enum):
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizer_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/get_quantizer_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 from model_compression_toolkit.core.common import BaseNode
 from model_compression_toolkit.logger import Logger
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
+from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig, TrainableQuantizerCandidateConfig
 
 
 def get_trainable_quantizer_weights_config(
         n: BaseNode,
         weights_quantization_candidates: List[TrainableQuantizerCandidateConfig] = None
 ) -> TrainableQuantizerWeightsConfig:
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/get_quantizers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/get_quantizers.py`

 * *Files 21% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union, Any
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.quantizers_infrastructure import QuantizationTarget
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.constants \
+from mct_quantizers import QuantizationTarget
+from mct_quantizers.common.constants \
     import QUANTIZATION_TARGET, QUANTIZATION_METHOD, QUANTIZER_TYPE
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common.get_all_subclasses \
+from mct_quantizers.common.get_all_subclasses \
     import get_all_subclasses
 
 
 def get_trainable_quantizer_class(quant_target: QuantizationTarget,
                                   quantizer_type: Union[Any, Any],
                                   quant_method: QuantizationMethod,
                                   quantizer_base_class: type) -> type:
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/quant_utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/common/trainable_quantizer_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/common/trainable_quantizer_config.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
+
+__version__ = 'v1'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/base_keras_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/base_keras_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,31 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Dict, Any, Union, List
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TF
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 
 if FOUND_TF:
     QUANTIZATION_CONFIG = 'quantization_config'
-    from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.keras.config_serialization import config_serialization, \
+    from model_compression_toolkit.trainable_infrastructure.keras.config_serialization import config_serialization, \
         config_deserialization
     import tensorflow as tf
 
     class BaseKerasTrainableQuantizer(BaseTrainableQuantizer):
         def __init__(self,
                      quantization_config: Union[TrainableQuantizerWeightsConfig, TrainableQuantizerActivationConfig]):
             """
             This class is a base quantizer which validates provided quantization config and defines an abstract function which any quantizer needs to implement.
             This class adds to the base quantizer a get_config and from_config functions to enable loading and saving the keras model.
+
             Args:
                 quantization_config: quantizer config class contains all the information about a quantizer configuration.
             """
             super().__init__(quantization_config)
 
         def get_config(self) -> Dict[str, Any]:
             """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/config_serialization.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/config_serialization.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 # ==============================================================================
 import copy
 
 from typing import Any, Union
 from enum import Enum
 
 from model_compression_toolkit.target_platform_capabilities.target_platform import QuantizationMethod
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.trainable_quantizer_config import \
+from model_compression_toolkit.trainable_infrastructure.common.trainable_quantizer_config import \
     TrainableQuantizerActivationConfig, TrainableQuantizerWeightsConfig
-from model_compression_toolkit.quantizers_infrastructure.inferable_infrastructure.common import constants as C
+from mct_quantizers.common import constants as C
 
 
 def transform_enum(v: Any):
     """
     If an enum is received it value is return otherwise the input is returned.
     Args:
         v: Any type
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/keras/quantizer_utils.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# ==============================================================================
+# ==============================================================================
+
+__version__ = 'v4'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/quantizers_infrastructure/trainable_infrastructure/pytorch/base_pytorch_quantizer.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/trainable_infrastructure/pytorch/base_pytorch_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import Union, List
 
 from model_compression_toolkit.logger import Logger
 from model_compression_toolkit.constants import FOUND_TORCH
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
-from model_compression_toolkit.quantizers_infrastructure.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
-from model_compression_toolkit.quantizers_infrastructure import TrainableQuantizerWeightsConfig, \
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import VariableGroup
+from model_compression_toolkit.trainable_infrastructure.common.base_trainable_quantizer import BaseTrainableQuantizer, VAR, GROUP
+from model_compression_toolkit.trainable_infrastructure import TrainableQuantizerWeightsConfig, \
     TrainableQuantizerActivationConfig
 
 
 if FOUND_TORCH:
 
     import torch
 
@@ -34,15 +34,14 @@
             abstract function which any quantizer needs to implement.
 
             Args:
                 quantization_config: quantizer config class contains all the information about the quantizer configuration.
             """
             super().__init__(quantization_config)
 
-
         def get_trainable_variables(self, group: VariableGroup) -> List[torch.Tensor]:
             """
             Get trainable parameters with specific group from quantizer
 
             Args:
                 group: Enum of variable group
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,7 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
+__version__ = 'v4_lut'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/constants.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,20 +8,13 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+from enum import Enum
 
-# TP Model constants
-OPS_SET_LIST = 'ops_set_list'
 
-# Version
-LATEST = 'latest'
-
-
-# Supported TP models names:
-DEFAULT_TP_MODEL = 'default'
-IMX500_TP_MODEL = 'imx500'
-TFLITE_TP_MODEL = 'tflite'
-QNNPACK_TP_MODEL = 'qnnpack'
+class QuantizationFormat(Enum):
+    FAKELY_QUANT = 0
+    INT8 = 1
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,12 +17,13 @@
 from model_compression_toolkit.target_platform_capabilities.target_platform.targetplatform2framework import \
     TargetPlatformCapabilities, OperationsSetToLayers, Smaller, SmallerEq, NotEq, Eq, GreaterEq, Greater, LayerFilterParams, OperationsToLayers, get_current_tpc
 
 from model_compression_toolkit.target_platform_capabilities.target_platform.target_platform_model import \
     get_default_quantization_config_options, TargetPlatformModel
 
 from model_compression_toolkit.target_platform_capabilities.target_platform.op_quantization_config import OpQuantizationConfig, \
-    QuantizationConfigOptions, QuantizationMethod
+    QuantizationConfigOptions
 from model_compression_toolkit.target_platform_capabilities.target_platform.operators import OperatorsSet, OperatorSetConcat
 
+from mct_quantizers import QuantizationMethod
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/current_tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/fusing.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/op_quantization_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,41 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import copy
-from enum import Enum
 from typing import List
 
-
-class QuantizationMethod(Enum):
-    """
-    Method for quantization function selection:
-
-    POWER_OF_TWO - Symmetric, uniform, threshold is power of two quantization.
-
-    KMEANS - k-means quantization.
-
-    LUT_POT_QUANTIZER - quantization using a lookup table and power of 2 threshold.
-
-    SYMMETRIC - Symmetric, uniform, quantization.
-
-    UNIFORM - uniform quantization,
-
-    LUT_SYM_QUANTIZER - quantization using a lookup table and symmetric threshold.
-
-    """
-    POWER_OF_TWO = 0
-    KMEANS = 1
-    LUT_POT_QUANTIZER = 2
-    SYMMETRIC = 3
-    UNIFORM = 4
-    LUT_SYM_QUANTIZER = 5
+from mct_quantizers import QuantizationMethod
 
 
 class OpQuantizationConfig:
     """
     OpQuantizationConfig is a class to configure the quantization parameters of an operator.
     """
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/operators.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/quantization_format.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/qat/common/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,16 @@
-# Copyright 2023 Sony Semiconductor Israel, Inc. All rights reserved.
+# Copyright 2022 Sony Semiconductor Israel, Inc. All rights reserved.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from enum import Enum
-
-
-class QuantizationFormat(Enum):
-    FAKELY_QUANT = 0
-    INT8 = 1
+from model_compression_toolkit.trainable_infrastructure.common.constants import THRESHOLD_TENSOR, \
+    WEIGHTS_QUANTIZATION_PARAMS
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/target_platform_model_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/attribute_filter.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/current_tpc.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/layer_filter_params.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/operations_to_layers.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/target_platform/targetplatform2framework/target_platform_capabilities_component.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,7 +8,9 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
+
+__version__ = 'v1'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_pytorch.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,38 +8,32 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-
-import operator
-
 import torch
-from torch import flatten, reshape, split, unsqueeze, dropout, chunk
-from torch.nn import Conv2d, BatchNorm2d
-from torch.nn import Dropout, Flatten
-from torch.nn import ReLU, ReLU6
-from torch.nn.functional import relu, relu6
+from torch.nn import Conv2d, Linear, BatchNorm2d, ConvTranspose2d, Hardtanh, ReLU, ReLU6
+from torch.nn.functional import relu, relu6, hardtanh
 
-from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1.tp_model import get_tp_model
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1.tp_model import get_tp_model
 import model_compression_toolkit as mct
-from model_compression_toolkit.target_platform_capabilities.tpc_models.default_tpc.v1 import __version__ as TPC_VERSION
+from model_compression_toolkit.target_platform_capabilities.tpc_models.qnnpack_tpc.v1 import __version__ as TPC_VERSION
 
 tp = mct.target_platform
 
 
 def get_pytorch_tpc() -> tp.TargetPlatformCapabilities:
     """
     get a Pytorch TargetPlatformCapabilities object with default operation sets to layers mapping.
     Returns: a Pytorch TargetPlatformCapabilities object for the given TargetPlatformModel.
     """
-    default_tp_model = get_tp_model()
-    return generate_pytorch_tpc(name='default_pytorch_tpc', tp_model=default_tp_model)
+    qnnpack_pytorch = get_tp_model()
+    return generate_pytorch_tpc(name='qnnpack_pytorch', tp_model=qnnpack_pytorch)
 
 
 def generate_pytorch_tpc(name: str, tp_model: tp.TargetPlatformModel):
     """
     Generates a TargetPlatformCapabilities object with default operation sets to layers mapping.
     Args:
         name: Name of the TargetPlatformModel.
@@ -48,27 +42,25 @@
     """
 
     pytorch_tpc = tp.TargetPlatformCapabilities(tp_model,
                                                 name=name,
                                                 version=TPC_VERSION)
 
     with pytorch_tpc:
-        tp.OperationsSetToLayers("NoQuantization", [Dropout,
-                                                    Flatten,
-                                                    dropout,
-                                                    flatten,
-                                                    split,
-                                                    operator.getitem,
-                                                    reshape,
-                                                    unsqueeze,
-                                                    BatchNorm2d,
-                                                    chunk,
-                                                    torch.Tensor.size])
-
-        tp.OperationsSetToLayers("Conv", [Conv2d])
-        tp.OperationsSetToLayers("AnyReLU", [torch.relu,
-                                             ReLU,
-                                             ReLU6,
-                                             relu,
-                                             relu6])
+        tp.OperationsSetToLayers("Conv", [Conv2d,
+                                          torch.nn.functional.conv2d,
+                                          ConvTranspose2d,
+                                          torch.nn.functional.conv_transpose2d])
+
+        tp.OperationsSetToLayers("Linear", [Linear])
+
+        tp.OperationsSetToLayers("BatchNorm", [BatchNorm2d])
+
+        tp.OperationsSetToLayers("Relu", [torch.relu,
+                                          ReLU,
+                                          ReLU6,
+                                          relu,
+                                          relu6,
+                                          tp.LayerFilterParams(Hardtanh, min_val=0),
+                                          tp.LayerFilterParams(hardtanh, min_val=0)])
 
     return pytorch_tpc
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-__version__ = 'v2'
+__version__ = 'v3_lut'
```

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v2/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v3_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v4_lut/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/default_tpc/v5/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/get_target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/imx500_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/qnnpack_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/latest/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/target_platform_capabilities.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tp_model.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_keras.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py` & `mct-nightly-1.9.0.20230619.post414/model_compression_toolkit/target_platform_capabilities/tpc_models/tflite_tpc/v1/tpc_pytorch.py`

 * *Files identical despite different names*

### Comparing `mct-nightly-1.8.0.9052023.post348/setup.py` & `mct-nightly-1.9.0.20230619.post414/setup.py`

 * *Files identical despite different names*

