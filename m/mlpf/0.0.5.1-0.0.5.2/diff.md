# Comparing `tmp/mlpf-0.0.5.1.tar.gz` & `tmp/mlpf-0.0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.5.1.tar", last modified: Tue Jun 20 14:13:54 2023, max compression
+gzip compressed data, was "mlpf-0.0.5.2.tar", last modified: Tue Jun 20 14:34:27 2023, max compression
```

## Comparing `mlpf-0.0.5.1.tar` & `mlpf-0.0.5.2.tar`

### file list

```diff
@@ -1,95 +1,103 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.639053 mlpf-0.0.5.1/
--rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.1/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.1/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3871 2023-06-20 14:13:54.639053 mlpf-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3254 2023-06-19 13:06:29.000000 mlpf-0.0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.425591 mlpf-0.0.5.1/examples/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.425591 mlpf-0.0.5.1/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.448634 mlpf-0.0.5.1/examples/sklearn/loss/
--rw-rw-rw-   0        0        0      952 2023-06-19 12:21:05.000000 mlpf-0.0.5.1/examples/sklearn/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.448634 mlpf-0.0.5.1/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.1/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.425591 mlpf-0.0.5.1/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.453455 mlpf-0.0.5.1/examples/torch/loss/
--rw-rw-rw-   0        0        0     1077 2023-06-19 12:29:11.000000 mlpf-0.0.5.1/examples/torch/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.464414 mlpf-0.0.5.1/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.1/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.1/examples/torch/supervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.466649 mlpf-0.0.5.1/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.485077 mlpf-0.0.5.1/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.487635 mlpf-0.0.5.1/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.504953 mlpf-0.0.5.1/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.519662 mlpf-0.0.5.1/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.519662 mlpf-0.0.5.1/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.524125 mlpf-0.0.5.1/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     3990 2023-06-20 14:09:15.000000 mlpf-0.0.5.1/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.527818 mlpf-0.0.5.1/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     4022 2023-06-11 16:38:41.000000 mlpf-0.0.5.1/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.532201 mlpf-0.0.5.1/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.537268 mlpf-0.0.5.1/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.553868 mlpf-0.0.5.1/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/conversion.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.581220 mlpf-0.0.5.1/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.581220 mlpf-0.0.5.1/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.594536 mlpf-0.0.5.1/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.614323 mlpf-0.0.5.1/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.622952 mlpf-0.0.5.1/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.1/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.1/mlpf/loss/torch/metrics/power_flow.py
--rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.1/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.630139 mlpf-0.0.5.1/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.485077 mlpf-0.0.5.1/mlpf.egg-info/
--rw-rw-rw-   0        0        0     3871 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-06-20 14:13:54.000000 mlpf-0.0.5.1/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 14:13:54.639053 mlpf-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-06-20 14:11:46.000000 mlpf-0.0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.638150 mlpf-0.0.5.1/test/
--rw-rw-rw-   0        0        0     2994 2023-06-11 16:38:41.000000 mlpf-0.0.5.1/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.729261 mlpf-0.0.5.2/
+-rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.2/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3875 2023-06-20 14:34:27.727073 mlpf-0.0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3258 2023-06-20 14:33:56.000000 mlpf-0.0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.638694 mlpf-0.0.5.2/examples/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.638694 mlpf-0.0.5.2/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.658301 mlpf-0.0.5.2/examples/sklearn/loss/
+-rw-rw-rw-   0        0        0      963 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/examples/sklearn/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.659593 mlpf-0.0.5.2/examples/sklearn/supervised_power_flow/
+-rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.2/examples/sklearn/supervised_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.640060 mlpf-0.0.5.2/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.659593 mlpf-0.0.5.2/examples/torch/loss/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/examples/torch/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.660773 mlpf-0.0.5.2/examples/torch/supervised_power_flow/
+-rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.2/examples/torch/supervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.2/examples/torch/supervised_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.661858 mlpf-0.0.5.2/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.680080 mlpf-0.0.5.2/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.680080 mlpf-0.0.5.2/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.685006 mlpf-0.0.5.2/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.687441 mlpf-0.0.5.2/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/conversion/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:22:21.000000 mlpf-0.0.5.2/mlpf/data/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/conversion/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:25:02.000000 mlpf-0.0.5.2/mlpf/data/conversion/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1788 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/conversion/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/conversion/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:25:07.000000 mlpf-0.0.5.2/mlpf/data/conversion/torch/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/conversion/torch/power_flow.py
+-rw-rw-rw-   0        0        0      475 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.692007 mlpf-0.0.5.2/mlpf/data/data/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/data/numpy/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/data/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.692869 mlpf-0.0.5.2/mlpf/data/data/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/data/torch/__init__.py
+-rw-rw-rw-   0        0        0     4033 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/data/torch/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.692869 mlpf-0.0.5.2/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.694702 mlpf-0.0.5.2/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.696481 mlpf-0.0.5.2/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/masks.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.700871 mlpf-0.0.5.2/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.700871 mlpf-0.0.5.2/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.722978 mlpf-0.0.5.2/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.722978 mlpf-0.0.5.2/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/torch/bound_errors.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.725995 mlpf-0.0.5.2/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.2/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.2/mlpf/loss/torch/metrics/power_flow.py
+-rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.2/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.727073 mlpf-0.0.5.2/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.680080 mlpf-0.0.5.2/mlpf.egg-info/
+-rw-rw-rw-   0        0        0     3875 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2272 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:34:27.729261 mlpf-0.0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-06-20 14:31:29.000000 mlpf-0.0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.727073 mlpf-0.0.5.2/test/
+-rw-rw-rw-   0        0        0     3020 2023-06-20 14:33:52.000000 mlpf-0.0.5.2/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.5.1/LICENCE.txt` & `mlpf-0.0.5.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/PKG-INFO` & `mlpf-0.0.5.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -62,45 +62,47 @@
 ```
 
 ### Loss
 
 #### numpy / scikit-learn
 
 ```python
-from mlpf.data.utils.conversion import ppc2power_flow_arrays
+
+from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.loss.numpy.power_flow import power_flow_errors
 
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu, angles_rad,
-    conductances_pu,
+  edge_index,
+  active_powers_pu,
+  reactive_powers_pu,
+  voltages_pu, angles_rad,
+  conductances_pu,
     susceptances_pu
 )
 ```
 
 #### torch
 
 ```python
-from mlpf.data.utils.conversion import ppc2power_flow_tensors
+
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.loss.torch.power_flow import power_flow_errors
 
 # note: going from float64(standard in PYPOWER) to float32(standard in torch) will increase the PF loss significantly
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_tensors(ppc, dtype=torch.float64)
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu, angles_rad,
-    conductances_pu,
-    susceptances_pu
+  edge_index,
+  active_powers_pu,
+  reactive_powers_pu,
+  voltages_pu, angles_rad,
+  conductances_pu,
+  susceptances_pu
 )
 ```
 
 ### Data loading
 
 - [ ] TODO
```

### Comparing `mlpf-0.0.5.1/README.md` & `mlpf-0.0.5.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -44,45 +44,47 @@
 ```
 
 ### Loss
 
 #### numpy / scikit-learn
 
 ```python
-from mlpf.data.utils.conversion import ppc2power_flow_arrays
+
+from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.loss.numpy.power_flow import power_flow_errors
 
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu, angles_rad,
-    conductances_pu,
+  edge_index,
+  active_powers_pu,
+  reactive_powers_pu,
+  voltages_pu, angles_rad,
+  conductances_pu,
     susceptances_pu
 )
 ```
 
 #### torch
 
 ```python
-from mlpf.data.utils.conversion import ppc2power_flow_tensors
+
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.loss.torch.power_flow import power_flow_errors
 
 # note: going from float64(standard in PYPOWER) to float32(standard in torch) will increase the PF loss significantly
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_tensors(ppc, dtype=torch.float64)
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu, angles_rad,
-    conductances_pu,
-    susceptances_pu
+  edge_index,
+  active_powers_pu,
+  reactive_powers_pu,
+  voltages_pu, angles_rad,
+  conductances_pu,
+  susceptances_pu
 )
 ```
 
 ### Data loading
 
 - [ ] TODO
```

### Comparing `mlpf-0.0.5.1/examples/sklearn/loss/from_arrays.py` & `mlpf-0.0.5.2/examples/sklearn/loss/from_arrays.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import numpy as np
 import pandapower as pp
 import pandapower.networks as pn
 
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 
-from mlpf.data.utils.conversion import ppc2power_flow_arrays
+from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.loss.numpy.power_flow import power_flow_errors
 
 net = pn.case118()
 
 ppc = pp.converter.to_ppc(net, init="flat")
 
 ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
```

### Comparing `mlpf-0.0.5.1/examples/sklearn/supervised_power_flow/linear_regression.py` & `mlpf-0.0.5.2/examples/sklearn/supervised_power_flow/linear_regression.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/examples/torch/loss/from_arrays.py` & `mlpf-0.0.5.2/examples/torch/loss/from_arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import pandapower as pp
 import pandapower.networks as pn
 
 from pypower.ppoption import ppoption
 from pypower.runpf import runpf
 
-from mlpf.data.utils.conversion import ppc2power_flow_tensors
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.loss.torch.power_flow import power_flow_errors
 
 net = pn.case118()
 
 ppc = pp.converter.to_ppc(net, init="flat")
 
 ppopt = ppoption(OUT_ALL=0, VERBOSE=0)
```

### Comparing `mlpf-0.0.5.1/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.5.2/examples/torch/supervised_power_flow/gcn.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.5.2/examples/torch/supervised_power_flow/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.5.2/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.5.2/mlpf/data/analysis/description/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.5.2/mlpf/data/analysis/description/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/utils.py` & `mlpf-0.0.5.2/mlpf/data/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.5.2/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/visualization/node_pdf_estimates.py` & `mlpf-0.0.5.2/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.5.2/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.5.2/mlpf/data/data/numpy/power_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import copy
 from typing import Tuple
 
 import numpy as np
 from numpy import ndarray
 from types import SimpleNamespace
 
-from mlpf.data.utils.conversion import ppc2power_flow_arrays
+from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.data.utils.masks import create_feature_mask
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.power_flow_ids import PowerFlowFeatureIds
 from mlpf.loss.numpy.power_flow import power_flow_errors
 from mlpf.loss.relative_values import relative_values
 from mlpf.utils.ppc import ppc_runpf
```

### Comparing `mlpf-0.0.5.1/mlpf/data/data/torch/power_flow.py` & `mlpf-0.0.5.2/mlpf/data/data/torch/power_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Tuple
 
 import torch
 from torch import Tensor
 from torch_geometric.data import Data
 
-from mlpf.data.utils.conversion import ppc2power_flow_tensors
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.data.utils.masks import create_feature_mask
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.power_flow_ids import PowerFlowFeatureIds
 from mlpf.loss.relative_values import relative_values
 from mlpf.loss.torch.power_flow import power_flow_errors
 from mlpf.utils.ppc import ppc_runpf
```

### Comparing `mlpf-0.0.5.1/mlpf/data/generate/generate_uniform_data.py` & `mlpf-0.0.5.2/mlpf/data/generate/generate_uniform_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/loading/load_data.py` & `mlpf-0.0.5.2/mlpf/data/loading/load_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pickle
 import random
 
 from pandapower import from_json
 from tqdm import tqdm
 from typing import Any, Callable, Dict, List
 
-from mlpf.data.utils.conversion import pandapower2ppc_list
+from mlpf.data.conversion.utils import pandapower2ppc_list
 
 
 def load_pickle_ppc(filepath: str) -> Dict:
     """
     The default way of loading a data sample(usually a PPC). Assumes that the file is a pickled object.
 
     :param filepath: Path to a file containing the pickled data sample.
```

### Comparing `mlpf-0.0.5.1/mlpf/data/utils/masks.py` & `mlpf-0.0.5.2/mlpf/data/utils/masks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.5.2/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/data/utils/saving.py` & `mlpf-0.0.5.2/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/enumerations/generator_table.py` & `mlpf-0.0.5.2/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.5.2/mlpf/enumerations/ppc_tables.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.5.2/mlpf/loss/numpy/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/numpy/power_flow.py` & `mlpf-0.0.5.2/mlpf/loss/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/numpy/utils.py` & `mlpf-0.0.5.2/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/relative_values.py` & `mlpf-0.0.5.2/mlpf/loss/relative_values.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.5.2/mlpf/loss/torch/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/torch/metrics/power_flow.py` & `mlpf-0.0.5.2/mlpf/loss/torch/metrics/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/torch/power_flow.py` & `mlpf-0.0.5.2/mlpf/loss/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/loss/torch/utils.py` & `mlpf-0.0.5.2/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf/utils/standard_scaler.py` & `mlpf-0.0.5.2/mlpf/utils/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.1/mlpf.egg-info/PKG-INFO` & `mlpf-0.0.5.2/mlpf.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5.1
+Version: 0.0.5.2
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -62,45 +62,47 @@
 ```
 
 ### Loss
 
 #### numpy / scikit-learn
 
 ```python
-from mlpf.data.utils.conversion import ppc2power_flow_arrays
+
+from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.loss.numpy.power_flow import power_flow_errors
 
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu, angles_rad,
-    conductances_pu,
+  edge_index,
+  active_powers_pu,
+  reactive_powers_pu,
+  voltages_pu, angles_rad,
+  conductances_pu,
     susceptances_pu
 )
 ```
 
 #### torch
 
 ```python
-from mlpf.data.utils.conversion import ppc2power_flow_tensors
+
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
 from mlpf.loss.torch.power_flow import power_flow_errors
 
 # note: going from float64(standard in PYPOWER) to float32(standard in torch) will increase the PF loss significantly
 edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_tensors(ppc, dtype=torch.float64)
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
-    edge_index,
-    active_powers_pu,
-    reactive_powers_pu,
-    voltages_pu, angles_rad,
-    conductances_pu,
-    susceptances_pu
+  edge_index,
+  active_powers_pu,
+  reactive_powers_pu,
+  voltages_pu, angles_rad,
+  conductances_pu,
+  susceptances_pu
 )
 ```
 
 ### Data loading
 
 - [ ] TODO
```

### Comparing `mlpf-0.0.5.1/mlpf.egg-info/SOURCES.txt` & `mlpf-0.0.5.2/mlpf.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -22,25 +22,30 @@
 mlpf/data/analysis/description/describe.py
 mlpf/data/analysis/description/describe_grid.py
 mlpf/data/analysis/description/describe_node.py
 mlpf/data/analysis/visualization/__init__.py
 mlpf/data/analysis/visualization/grid_pdf_estimates.py
 mlpf/data/analysis/visualization/node_pdf_estimates.py
 mlpf/data/analysis/visualization/visualize.py
+mlpf/data/conversion/__init__.py
+mlpf/data/conversion/utils.py
+mlpf/data/conversion/numpy/__init__.py
+mlpf/data/conversion/numpy/power_flow.py
+mlpf/data/conversion/torch/__init__.py
+mlpf/data/conversion/torch/power_flow.py
 mlpf/data/data/__init__.py
 mlpf/data/data/numpy/__init__.py
 mlpf/data/data/numpy/power_flow.py
 mlpf/data/data/torch/__init__.py
 mlpf/data/data/torch/power_flow.py
 mlpf/data/generate/__init__.py
 mlpf/data/generate/generate_uniform_data.py
 mlpf/data/loading/__init__.py
 mlpf/data/loading/load_data.py
 mlpf/data/utils/__init__.py
-mlpf/data/utils/conversion.py
 mlpf/data/utils/masks.py
 mlpf/data/utils/pandapower_networks.py
 mlpf/data/utils/saving.py
 mlpf/enumerations/__init__.py
 mlpf/enumerations/branch_table.py
 mlpf/enumerations/bus_table.py
 mlpf/enumerations/bus_type.py
```

### Comparing `mlpf-0.0.5.1/setup.py` & `mlpf-0.0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlpf',
-    version='0.0.5.1',
+    version='0.0.5.2',
     description='Machine learning for power flow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Viktor Todosijevic',
     author_email='todosijevicviktor998@gmail.com',
     license='MIT',
```

### Comparing `mlpf-0.0.5.1/test/test_power_flow_loss.py` & `mlpf-0.0.5.2/test/test_power_flow_loss.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import unittest
 import warnings
 from typing import Dict
 
 import pandapower as pp
 import torch
 
-from mlpf.data.utils.conversion import ppc2power_flow_tensors, ppc2power_flow_arrays
+from mlpf.data.conversion.torch.power_flow import ppc2power_flow_tensors
+from mlpf.data.conversion.numpy.power_flow import ppc2power_flow_arrays
 from mlpf.data.utils.pandapower_networks import get_all_pandapower_networks
 from mlpf.loss.numpy import power_flow as pf_numpy
 from mlpf.loss.torch import power_flow as pf_torch
 
 
 def torch_get_power_flow_loss(ppc: Dict, method="scatter", dtype: torch.dtype = torch.float64) -> float:
     """
@@ -37,15 +38,14 @@
 
 def numpy_get_power_flow_loss(ppc: Dict, method="sparse") -> float:
     """
     Get power flow loss from a ppc.
 
     :param ppc: pypower case format
     :param method: To use scatter operations on arrays or to multiply with sparse matrices.
-    :param dtype: torch data type
     :return: loss
     """
     edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc)
 
     active_power_losses_pu, reactive_power_losses_pu = pf_numpy.power_flow_errors(
         edge_index,
         active_powers_pu,
```

