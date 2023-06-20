# Comparing `tmp/mlpf-0.0.5.5.tar.gz` & `tmp/mlpf-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.5.5.tar", last modified: Tue Jun 20 16:39:41 2023, max compression
+gzip compressed data, was "mlpf-0.0.5.6.tar", last modified: Tue Jun 20 16:51:16 2023, max compression
```

## Comparing `mlpf-0.0.5.5.tar` & `mlpf-0.0.5.6.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.701284 mlpf-0.0.5.5/
--rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.5/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3902 2023-06-20 16:39:41.701284 mlpf-0.0.5.5/PKG-INFO
--rw-rw-rw-   0        0        0     3262 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.637365 mlpf-0.0.5.5/examples/
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.637365 mlpf-0.0.5.5/examples/data/
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.649702 mlpf-0.0.5.5/examples/data/analysis/
--rw-rw-rw-   0        0        0     1390 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/data/analysis/describe_grid.py
--rw-rw-rw-   0        0        0     1238 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/data/analysis/describe_node.py
--rw-rw-rw-   0        0        0     1332 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/data/analysis/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     1249 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/data/analysis/node_pdf_estimates.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.651161 mlpf-0.0.5.5/examples/data/generate/
--rw-rw-rw-   0        0        0     1085 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/data/generate/uniform.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.637365 mlpf-0.0.5.5/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.651161 mlpf-0.0.5.5/examples/sklearn/loss/
--rw-rw-rw-   0        0        0      966 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/sklearn/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.652085 mlpf-0.0.5.5/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.5/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.637365 mlpf-0.0.5.5/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.652925 mlpf-0.0.5.5/examples/torch/loss/
--rw-rw-rw-   0        0        0     1091 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/examples/torch/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.653803 mlpf-0.0.5.5/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.5/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.5/examples/torch/supervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.654499 mlpf-0.0.5.5/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.672074 mlpf-0.0.5.5/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.672074 mlpf-0.0.5.5/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.675841 mlpf-0.0.5.5/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     1447 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     1396 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6433 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.677340 mlpf-0.0.5.5/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     3420 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     3473 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.679175 mlpf-0.0.5.5/mlpf/data/conversion/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.680288 mlpf-0.0.5.5/mlpf/data/conversion/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/conversion/numpy/__init__.py
--rw-rw-rw-   0        0        0     1788 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/conversion/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.680288 mlpf-0.0.5.5/mlpf/data/conversion/torch/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/conversion/torch/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/conversion/torch/power_flow.py
--rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.680288 mlpf-0.0.5.5/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.682911 mlpf-0.0.5.5/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.682911 mlpf-0.0.5.5/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     4033 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.685444 mlpf-0.0.5.5/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     3523 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.685444 mlpf-0.0.5.5/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.687725 mlpf-0.0.5.5/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.690943 mlpf-0.0.5.5/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1254 2023-06-20 15:43:08.000000 mlpf-0.0.5.5/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.693445 mlpf-0.0.5.5/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.695683 mlpf-0.0.5.5/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.697369 mlpf-0.0.5.5/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.697369 mlpf-0.0.5.5/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.5/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.5/mlpf/loss/torch/metrics/power_flow.py
--rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.5/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.700060 mlpf-0.0.5.5/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.5/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.672074 mlpf-0.0.5.5/mlpf.egg-info/
--rw-rw-rw-   0        0        0     3902 2023-06-20 16:39:41.000000 mlpf-0.0.5.5/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2476 2023-06-20 16:39:41.000000 mlpf-0.0.5.5/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       93 2023-06-20 16:39:41.000000 mlpf-0.0.5.5/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      175 2023-06-20 16:39:41.000000 mlpf-0.0.5.5/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 16:39:41.000000 mlpf-0.0.5.5/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 16:39:41.701284 mlpf-0.0.5.5/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-06-20 16:39:35.000000 mlpf-0.0.5.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 16:39:41.701284 mlpf-0.0.5.5/test/
--rw-rw-rw-   0        0        0     3020 2023-06-20 14:41:06.000000 mlpf-0.0.5.5/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/
+-rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.6/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3957 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3317 2023-06-20 16:41:41.000000 mlpf-0.0.5.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.590932 mlpf-0.0.5.6/examples/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.590932 mlpf-0.0.5.6/examples/data/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/examples/data/analysis/
+-rw-rw-rw-   0        0        0     1390 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/data/analysis/describe_grid.py
+-rw-rw-rw-   0        0        0     1238 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/data/analysis/describe_node.py
+-rw-rw-rw-   0        0        0     1332 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/data/analysis/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     1249 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/data/analysis/node_pdf_estimates.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/examples/data/generate/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/data/generate/uniform.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.590932 mlpf-0.0.5.6/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/examples/sklearn/loss/
+-rw-rw-rw-   0        0        0      966 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/sklearn/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/examples/sklearn/supervised_power_flow/
+-rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.6/examples/sklearn/supervised_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.590932 mlpf-0.0.5.6/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/examples/torch/loss/
+-rw-rw-rw-   0        0        0     1091 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/examples/torch/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/examples/torch/supervised_power_flow/
+-rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.6/examples/torch/supervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.6/examples/torch/supervised_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.610163 mlpf-0.0.5.6/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     1447 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     1396 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6433 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     3420 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     3473 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf/data/conversion/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf/data/conversion/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/conversion/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1788 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/conversion/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/conversion/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/conversion/torch/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/conversion/torch/power_flow.py
+-rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/data/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/data/numpy/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/data/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/data/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/data/torch/__init__.py
+-rw-rw-rw-   0        0        0     4033 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/data/torch/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     3523 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/utils/masks.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1254 2023-06-20 15:43:08.000000 mlpf-0.0.5.6/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.638471 mlpf-0.0.5.6/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/torch/bound_errors.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.6/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.6/mlpf/loss/torch/metrics/power_flow.py
+-rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.6/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.6/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.622756 mlpf-0.0.5.6/mlpf.egg-info/
+-rw-rw-rw-   0        0        0     3957 2023-06-20 16:51:16.000000 mlpf-0.0.5.6/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2023-06-20 16:51:16.000000 mlpf-0.0.5.6/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       93 2023-06-20 16:51:16.000000 mlpf-0.0.5.6/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2023-06-20 16:51:16.000000 mlpf-0.0.5.6/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 16:51:16.000000 mlpf-0.0.5.6/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/setup.cfg
+-rw-rw-rw-   0        0        0     1369 2023-06-20 16:51:04.000000 mlpf-0.0.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 16:51:16.654012 mlpf-0.0.5.6/test/
+-rw-rw-rw-   0        0        0     3020 2023-06-20 14:41:06.000000 mlpf-0.0.5.6/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.5.5/LICENCE.txt` & `mlpf-0.0.5.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/PKG-INFO` & `mlpf-0.0.5.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -32,15 +32,19 @@
 * visualization and description tools to take a quick look at your data
 
 Contributions welcome!
 
 ## Installation
 
 ```commandline
-pip install mlpf
+pip install -U pip
+
+pip install -U mlpf
+
+pip install -U mlpf[torch]
 ```
 
 ## Usage
 
 1. Load/create data and turn it into the [PYPOWER case format](https://rwl.github.io/PYPOWER/api/pypower.caseformat-module.html)
 2. From then on we provide functionality to express the data as numpy arrays or torch tensors.
 3. Feed that data into your ML (scikit-learn or torch) models and use our tried and tested loss functions to train, validate or monitor your model development.
```

### Comparing `mlpf-0.0.5.5/README.md` & `mlpf-0.0.5.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 * visualization and description tools to take a quick look at your data
 
 Contributions welcome!
 
 ## Installation
 
 ```commandline
-pip install mlpf
+pip install -U pip
+
+pip install -U mlpf
+
+pip install -U mlpf[torch]
 ```
 
 ## Usage
 
 1. Load/create data and turn it into the [PYPOWER case format](https://rwl.github.io/PYPOWER/api/pypower.caseformat-module.html)
 2. From then on we provide functionality to express the data as numpy arrays or torch tensors.
 3. Feed that data into your ML (scikit-learn or torch) models and use our tried and tested loss functions to train, validate or monitor your model development.
```

### Comparing `mlpf-0.0.5.5/examples/data/analysis/describe_grid.py` & `mlpf-0.0.5.6/examples/data/analysis/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/data/analysis/describe_node.py` & `mlpf-0.0.5.6/examples/data/analysis/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/data/analysis/grid_pdf_estimates.py` & `mlpf-0.0.5.6/examples/data/analysis/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/data/analysis/node_pdf_estimates.py` & `mlpf-0.0.5.6/examples/data/analysis/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/data/generate/uniform.py` & `mlpf-0.0.5.6/examples/data/generate/uniform.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/sklearn/loss/from_arrays.py` & `mlpf-0.0.5.6/examples/sklearn/loss/from_arrays.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/sklearn/supervised_power_flow/linear_regression.py` & `mlpf-0.0.5.6/examples/sklearn/supervised_power_flow/linear_regression.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/torch/loss/from_arrays.py` & `mlpf-0.0.5.6/examples/torch/loss/from_arrays.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.5.6/examples/torch/supervised_power_flow/gcn.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.5.6/examples/torch/supervised_power_flow/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.5.6/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.5.6/mlpf/data/analysis/description/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.5.6/mlpf/data/analysis/description/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/utils.py` & `mlpf-0.0.5.6/mlpf/data/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.5.6/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/visualization/node_pdf_estimates.py` & `mlpf-0.0.5.6/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.5.6/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/conversion/numpy/power_flow.py` & `mlpf-0.0.5.6/mlpf/data/conversion/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/conversion/torch/power_flow.py` & `mlpf-0.0.5.6/mlpf/data/conversion/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.5.6/mlpf/data/data/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/data/torch/power_flow.py` & `mlpf-0.0.5.6/mlpf/data/data/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/generate/generate_uniform_data.py` & `mlpf-0.0.5.6/mlpf/data/generate/generate_uniform_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/loading/load_data.py` & `mlpf-0.0.5.6/mlpf/data/loading/load_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/utils/masks.py` & `mlpf-0.0.5.6/mlpf/data/utils/masks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.5.6/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/data/utils/saving.py` & `mlpf-0.0.5.6/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/enumerations/generator_table.py` & `mlpf-0.0.5.6/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.5.6/mlpf/enumerations/ppc_tables.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.5.6/mlpf/loss/numpy/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/numpy/power_flow.py` & `mlpf-0.0.5.6/mlpf/loss/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/numpy/utils.py` & `mlpf-0.0.5.6/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/relative_values.py` & `mlpf-0.0.5.6/mlpf/loss/relative_values.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.5.6/mlpf/loss/torch/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/torch/metrics/power_flow.py` & `mlpf-0.0.5.6/mlpf/loss/torch/metrics/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/torch/power_flow.py` & `mlpf-0.0.5.6/mlpf/loss/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/loss/torch/utils.py` & `mlpf-0.0.5.6/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf/utils/standard_scaler.py` & `mlpf-0.0.5.6/mlpf/utils/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/mlpf.egg-info/PKG-INFO` & `mlpf-0.0.5.6/mlpf.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -32,15 +32,19 @@
 * visualization and description tools to take a quick look at your data
 
 Contributions welcome!
 
 ## Installation
 
 ```commandline
-pip install mlpf
+pip install -U pip
+
+pip install -U mlpf
+
+pip install -U mlpf[torch]
 ```
 
 ## Usage
 
 1. Load/create data and turn it into the [PYPOWER case format](https://rwl.github.io/PYPOWER/api/pypower.caseformat-module.html)
 2. From then on we provide functionality to express the data as numpy arrays or torch tensors.
 3. Feed that data into your ML (scikit-learn or torch) models and use our tried and tested loss functions to train, validate or monitor your model development.
```

### Comparing `mlpf-0.0.5.5/mlpf.egg-info/SOURCES.txt` & `mlpf-0.0.5.6/mlpf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.5/setup.py` & `mlpf-0.0.5.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,23 +12,23 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlpf',
-    version='0.0.5.5',
+    version='0.0.5.6',
     description='Machine learning for power flow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Viktor Todosijevic',
     author_email='todosijevicviktor998@gmail.com',
     license='MIT',
     classifiers=classifiers,
     keywords=['machine learning', 'power'],
     packages=find_packages(),
     install_requires=['numpy', 'pandapower', 'PYPOWER', 'scikit-learn', 'scipy', 'tqdm'],
-    extras_require={'torch': ['torch', 'torchvision', 'torchaudio', 'torchmetrics',
+    extras_require={'torch': ['torch==2.0.0', 'torchvision', 'torchaudio', 'torchmetrics',
                               'torch_geometric', 'torch_scatter', 'torch_sparse', 'torch_cluster', 'torch_spline_conv']},
     dependency_links=["https://data.pyg.org/whl/torch-2.0.0+cpu.html", "https://data.pyg.org/whl/torch-1.13.0+cpu.html"]  # TODO maybe make torch>=1.13
 )
```

### Comparing `mlpf-0.0.5.5/test/test_power_flow_loss.py` & `mlpf-0.0.5.6/test/test_power_flow_loss.py`

 * *Files identical despite different names*

