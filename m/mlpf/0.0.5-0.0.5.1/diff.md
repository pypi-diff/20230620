# Comparing `tmp/mlpf-0.0.5.tar.gz` & `tmp/mlpf-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.5.tar", last modified: Mon Jun 19 13:12:31 2023, max compression
+gzip compressed data, was "mlpf-0.0.5.1.tar", last modified: Tue Jun 20 14:13:54 2023, max compression
```

## Comparing `mlpf-0.0.5.tar` & `mlpf-0.0.5.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.247629 mlpf-0.0.5/
--rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3869 2023-06-19 13:12:31.247629 mlpf-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3254 2023-06-19 13:06:29.000000 mlpf-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.004611 mlpf-0.0.5/examples/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.004611 mlpf-0.0.5/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.020685 mlpf-0.0.5/examples/sklearn/loss/
--rw-rw-rw-   0        0        0      952 2023-06-19 12:21:05.000000 mlpf-0.0.5/examples/sklearn/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.020685 mlpf-0.0.5/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2711 2023-06-11 14:41:11.000000 mlpf-0.0.5/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.010466 mlpf-0.0.5/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.036188 mlpf-0.0.5/examples/torch/loss/
--rw-rw-rw-   0        0        0     1077 2023-06-19 12:29:11.000000 mlpf-0.0.5/examples/torch/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.058917 mlpf-0.0.5/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     4940 2023-06-17 16:14:26.000000 mlpf-0.0.5/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4180 2023-06-17 16:14:26.000000 mlpf-0.0.5/examples/torch/supervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.058917 mlpf-0.0.5/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.070708 mlpf-0.0.5/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.083967 mlpf-0.0.5/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.100813 mlpf-0.0.5/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.112435 mlpf-0.0.5/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.116442 mlpf-0.0.5/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.117811 mlpf-0.0.5/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     3961 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.121572 mlpf-0.0.5/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     4022 2023-06-11 16:38:41.000000 mlpf-0.0.5/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.126592 mlpf-0.0.5/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.127984 mlpf-0.0.5/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.139687 mlpf-0.0.5/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     3487 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/utils/conversion.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.180744 mlpf-0.0.5/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.180744 mlpf-0.0.5/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.210504 mlpf-0.0.5/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.226636 mlpf-0.0.5/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.242511 mlpf-0.0.5/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5/mlpf/loss/torch/metrics/power_flow.py
--rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.247629 mlpf-0.0.5/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.070708 mlpf-0.0.5/mlpf.egg-info/
--rw-rw-rw-   0        0        0     3869 2023-06-19 13:12:30.000000 mlpf-0.0.5/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2079 2023-06-19 13:12:30.000000 mlpf-0.0.5/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 13:12:30.000000 mlpf-0.0.5/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-19 13:12:30.000000 mlpf-0.0.5/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-19 13:12:30.000000 mlpf-0.0.5/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 13:12:31.247629 mlpf-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1014 2023-06-19 13:07:29.000000 mlpf-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 13:12:31.247629 mlpf-0.0.5/test/
--rw-rw-rw-   0        0        0     2994 2023-06-11 16:38:41.000000 mlpf-0.0.5/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.639053 mlpf-0.0.5.1/
+-rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.1/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3871 2023-06-20 14:13:54.639053 mlpf-0.0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3254 2023-06-19 13:06:29.000000 mlpf-0.0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.425591 mlpf-0.0.5.1/examples/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.425591 mlpf-0.0.5.1/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.448634 mlpf-0.0.5.1/examples/sklearn/loss/
+-rw-rw-rw-   0        0        0      952 2023-06-19 12:21:05.000000 mlpf-0.0.5.1/examples/sklearn/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.448634 mlpf-0.0.5.1/examples/sklearn/supervised_power_flow/
+-rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.1/examples/sklearn/supervised_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.425591 mlpf-0.0.5.1/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.453455 mlpf-0.0.5.1/examples/torch/loss/
+-rw-rw-rw-   0        0        0     1077 2023-06-19 12:29:11.000000 mlpf-0.0.5.1/examples/torch/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.464414 mlpf-0.0.5.1/examples/torch/supervised_power_flow/
+-rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.1/examples/torch/supervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.1/examples/torch/supervised_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.466649 mlpf-0.0.5.1/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.485077 mlpf-0.0.5.1/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.487635 mlpf-0.0.5.1/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.504953 mlpf-0.0.5.1/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.519662 mlpf-0.0.5.1/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.519662 mlpf-0.0.5.1/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.524125 mlpf-0.0.5.1/mlpf/data/data/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/data/numpy/__init__.py
+-rw-rw-rw-   0        0        0     3990 2023-06-20 14:09:15.000000 mlpf-0.0.5.1/mlpf/data/data/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.527818 mlpf-0.0.5.1/mlpf/data/data/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/data/torch/__init__.py
+-rw-rw-rw-   0        0        0     4022 2023-06-11 16:38:41.000000 mlpf-0.0.5.1/mlpf/data/data/torch/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.532201 mlpf-0.0.5.1/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.537268 mlpf-0.0.5.1/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.553868 mlpf-0.0.5.1/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     3487 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/conversion.py
+-rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/masks.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.581220 mlpf-0.0.5.1/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.581220 mlpf-0.0.5.1/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.594536 mlpf-0.0.5.1/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.614323 mlpf-0.0.5.1/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/torch/bound_errors.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.622952 mlpf-0.0.5.1/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.1/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.1/mlpf/loss/torch/metrics/power_flow.py
+-rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.1/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.630139 mlpf-0.0.5.1/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.1/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.485077 mlpf-0.0.5.1/mlpf.egg-info/
+-rw-rw-rw-   0        0        0     3871 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2079 2023-06-20 14:13:54.000000 mlpf-0.0.5.1/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 14:13:53.000000 mlpf-0.0.5.1/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:13:54.639053 mlpf-0.0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-06-20 14:11:46.000000 mlpf-0.0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:13:54.638150 mlpf-0.0.5.1/test/
+-rw-rw-rw-   0        0        0     2994 2023-06-11 16:38:41.000000 mlpf-0.0.5.1/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.5/LICENCE.txt` & `mlpf-0.0.5.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/PKG-INFO` & `mlpf-0.0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mlpf-0.0.5/README.md` & `mlpf-0.0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/examples/sklearn/loss/from_arrays.py` & `mlpf-0.0.5.1/examples/sklearn/loss/from_arrays.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/examples/sklearn/supervised_power_flow/linear_regression.py` & `mlpf-0.0.5.1/examples/sklearn/supervised_power_flow/linear_regression.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import random
 
 import numpy as np
+import pandapower as pp
+import pandapower.networks as pn
 import pandas as pd
+
 from pandas import DataFrame
+from pypower.ppoption import ppoption
+from pypower.runpf import runpf
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import train_test_split
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import StandardScaler
 from tqdm import tqdm
 
 from mlpf.data.data.numpy.power_flow import power_flow_data, get_relative_power_flow_errors
-from mlpf.data.loading.load_data import autodetect_load_ppc
+from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 
 
 def main():
     # Random seeds
     np.random.seed(123)
     random.seed(123)
 
-    # Load ppcs and ppc -> Data
+    # Generate ppcs
+
+    net = pn.case118()
+    ppc = pp.converter.to_ppc(net, init="flat")
+
+    base_ppc, converged = runpf(ppc, ppopt=ppoption(OUT_ALL=0, VERBOSE=0))
 
-    ppc_list = autodetect_load_ppc("generated_ppcs", max_samples=1000, shuffle=True)
+    ppc_list = generate_uniform_ppcs(
+        base_ppc,
+        how_many=1000,
+        low=0.9,
+        high=1.1
+    )
 
+    # ppc -> Data
     pf_data_list = []
     for ppc in tqdm(ppc_list, ascii=True, desc="Converting ppcs to data"):
         pf_data_list.append(power_flow_data(ppc))
 
     data_train, data_val = train_test_split(pf_data_list, test_size=0.33, random_state=42)
 
     features_train = np.vstack([data.feature_vector for data in data_train])
@@ -41,16 +57,16 @@
     # backbone = MultiOutputRegressor(BayesianRidge())
 
     model = make_pipeline(StandardScaler(), backbone)
     model.fit(features_train, targets_train)
 
     # Evaluation
 
-    print(f"Train coefficient of determination = {model.score(features_train, targets_train)} (max is 1.0)")
-    print(f"Validation coefficient of determination = {model.score(features_val, targets_val)} (max is 1.0)\n")
+    print(f"Train R2 score = {model.score(features_train, targets_train)}")
+    print(f"Val R2 score = {model.score(features_val, targets_val)}\n")
 
     val_predictions = model.predict(features_val)
 
     # power flow evaluation
     relative_active_power_errors_list = []
     relative_reactive_power_errors_list = []
```

### Comparing `mlpf-0.0.5/examples/torch/loss/from_arrays.py` & `mlpf-0.0.5.1/examples/torch/loss/from_arrays.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.5.1/examples/torch/supervised_power_flow/gcn.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import torch
+
+import pandapower as pp
+import pandapower.networks as pn
 import torch.nn as nn
 import torch_geometric as pyg
+
 from pandas.io.json._normalize import nested_to_record
+from pypower.ppoption import ppoption
+from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection, MeanSquaredError, R2Score
 from tqdm import tqdm
 
 from mlpf.data.data.torch.power_flow import power_flow_data
-from mlpf.data.loading.load_data import autodetect_load_ppc
+from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 from mlpf.loss.torch.metrics.power_flow import RelativePowerFlowError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 class GNN(torch.nn.Module):
     def __init__(self, in_channels, hidden_channels, num_layers, out_channels, standard_scaler):
         super(GNN, self).__init__()
@@ -25,31 +31,41 @@
         out = self.graph_encoder(x=out, edge_index=data.edge_index)
         out = self.linear(out)[~data.feature_mask].reshape(data.target_vector.shape)
 
         return out
 
 
 def main():
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
     # Random seeds
     pyg.seed_everything(123)
 
     # Hyperparameters
     num_epochs = 1000
     batch_size = 512
     hidden_channels = 100
     num_layers = 3
     learning_rate = 3e-4
 
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    # Generate ppcs
+
+    net = pn.case118()
+    ppc = pp.converter.to_ppc(net, init="flat")
 
-    # Load ppcs and ppc -> Data
+    base_ppc, converged = runpf(ppc, ppopt=ppoption(OUT_ALL=0, VERBOSE=0))
 
-    solved_ppc_list = autodetect_load_ppc("generated_ppcs", shuffle=True, max_samples=1000)
+    solved_ppc_list = generate_uniform_ppcs(
+        base_ppc,
+        how_many=1000,
+        low=0.9,
+        high=1.1
+    )
 
+    # ppc -> Data
     pf_data_list = []
     for solved_ppc in tqdm(solved_ppc_list, ascii=True, desc="Converting ppcs to data"):
         pf_data_list.append(power_flow_data(solved_ppc))
 
     for data in pf_data_list:
         data.x[~data.feature_mask] = 0.0  # delete the target info from the input features
```

### Comparing `mlpf-0.0.5/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.5.1/examples/torch/supervised_power_flow/mlp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,54 @@
 import torch
 
+import pandapower as pp
+import pandapower.networks as pn
 import torch.nn as nn
 import torch_geometric as pyg
 
 from pandas.io.json._normalize import nested_to_record
+from pypower.ppoption import ppoption
+from pypower.runpf import runpf
 from sklearn.model_selection import train_test_split
 from torch_geometric.loader import DataLoader
 from torchmetrics import MetricCollection, MeanSquaredError, R2Score
 from tqdm import tqdm
 
 from mlpf.data.data.torch.power_flow import power_flow_data
-from mlpf.data.loading.load_data import autodetect_load_ppc
+from mlpf.data.generate.generate_uniform_data import generate_uniform_ppcs
 from mlpf.loss.torch.metrics.power_flow import RelativePowerFlowError
 from mlpf.utils.standard_scaler import StandardScaler
 
 
 def main():
+    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+
     # Random seeds
     pyg.seed_everything(123)
 
     # Hyperparameters
     num_epochs = 1000
     batch_size = 512
     learning_rate = 3e-3
 
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+    # Generate ppcs
+
+    net = pn.case118()
+    ppc = pp.converter.to_ppc(net, init="flat")
 
-    # Load ppcs and ppc -> Data
+    base_ppc, converged = runpf(ppc, ppopt=ppoption(OUT_ALL=0, VERBOSE=0))
 
-    solved_ppc_list = autodetect_load_ppc("generated_ppcs", shuffle=True, max_samples=1000)
+    solved_ppc_list = generate_uniform_ppcs(
+        base_ppc,
+        how_many=1000,
+        low=0.9,
+        high=1.1
+    )
 
+    # ppc -> Data
     pf_data_list = []
     for solved_ppc in tqdm(solved_ppc_list, ascii=True, desc="Converting ppcs to data"):
         pf_data_list.append(power_flow_data(solved_ppc))
 
     data_train, data_val = train_test_split(pf_data_list, test_size=0.33, random_state=42)
 
     # Torch dataloaders
```

### Comparing `mlpf-0.0.5/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.5.1/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.5.1/mlpf/data/analysis/description/describe_grid.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.5.1/mlpf/data/analysis/description/describe_node.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/analysis/utils.py` & `mlpf-0.0.5.1/mlpf/data/analysis/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.5.1/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/analysis/visualization/node_pdf_estimates.py` & `mlpf-0.0.5.1/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.5.1/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.5.1/mlpf/data/data/numpy/power_flow.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 from typing import Tuple
 
 import numpy as np
 from numpy import ndarray
-from torch_geometric.data import Data
+from types import SimpleNamespace
 
 from mlpf.data.utils.conversion import ppc2power_flow_arrays
 from mlpf.data.utils.masks import create_feature_mask
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.power_flow_ids import PowerFlowFeatureIds
 from mlpf.loss.numpy.power_flow import power_flow_errors
 from mlpf.loss.relative_values import relative_values
@@ -28,28 +28,28 @@
     edge_index, active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad, conductances_pu, susceptances_pu = ppc2power_flow_arrays(ppc, dtype=dtype)
 
     PQVA_matrix = np.vstack((active_powers_pu, reactive_powers_pu, voltages_pu, angles_rad)).T
     feature_mask = create_feature_mask(ppc["bus"][:, BusTableIds.bus_type])
 
     edge_attributes = np.vstack((conductances_pu, susceptances_pu))
 
-    return Data(
+    return SimpleNamespace(
         edge_index=edge_index,
         x=PQVA_matrix,
         edge_attr=edge_attributes,
         PQVA_matrix=PQVA_matrix,
         feature_mask=feature_mask,
         conductances_pu=conductances_pu,
         susceptances_pu=susceptances_pu,
         feature_vector=PQVA_matrix[feature_mask],
         target_vector=PQVA_matrix[~feature_mask]
     )
 
 
-def get_power_flow_errors(predictions: ndarray, data: Data) -> Tuple[ndarray, ...]:
+def get_power_flow_errors(predictions: ndarray, data: SimpleNamespace) -> Tuple[ndarray, ...]:
     """
     Take model predictions and merge them with the corresponding data object.
     Calculate the power flow errors for the given predictions.
 
     :param predictions: Power flow unknown variable predictions.
     :param data: Data object from which the predictions came from.
     :return: (active power errors, reactive power errors, active power, reactive power)
@@ -70,15 +70,15 @@
         conductances=data.conductances_pu,
         susceptances=data.susceptances_pu
     )
 
     return active_power_errors, reactive_power_errors, active_powers, reactive_powers
 
 
-def get_relative_power_flow_errors(predictions: ndarray, data: Data) -> Tuple[ndarray, ...]:
+def get_relative_power_flow_errors(predictions: ndarray, data: SimpleNamespace) -> Tuple[ndarray, ...]:
     """
     Take model predictions and merge them with the corresponding data batch.
     Calculate the relative power flow errors for the given predictions.
 
     :param predictions: Power flow unknown variable predictions.
     :param data: Data object from which the predictions came from.
     :return: (relative active power errors, relative reactive power errors)
```

### Comparing `mlpf-0.0.5/mlpf/data/data/torch/power_flow.py` & `mlpf-0.0.5.1/mlpf/data/data/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/generate/generate_uniform_data.py` & `mlpf-0.0.5.1/mlpf/data/generate/generate_uniform_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/loading/load_data.py` & `mlpf-0.0.5.1/mlpf/data/loading/load_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/utils/conversion.py` & `mlpf-0.0.5.1/mlpf/data/utils/conversion.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/utils/masks.py` & `mlpf-0.0.5.1/mlpf/data/utils/masks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.5.1/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/data/utils/saving.py` & `mlpf-0.0.5.1/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/enumerations/generator_table.py` & `mlpf-0.0.5.1/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.5.1/mlpf/enumerations/ppc_tables.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.5.1/mlpf/loss/numpy/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/numpy/power_flow.py` & `mlpf-0.0.5.1/mlpf/loss/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/numpy/utils.py` & `mlpf-0.0.5.1/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/relative_values.py` & `mlpf-0.0.5.1/mlpf/loss/relative_values.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.5.1/mlpf/loss/torch/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/torch/metrics/power_flow.py` & `mlpf-0.0.5.1/mlpf/loss/torch/metrics/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/torch/power_flow.py` & `mlpf-0.0.5.1/mlpf/loss/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/loss/torch/utils.py` & `mlpf-0.0.5.1/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf/utils/standard_scaler.py` & `mlpf-0.0.5.1/mlpf/utils/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/mlpf.egg-info/PKG-INFO` & `mlpf-0.0.5.1/mlpf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5
+Version: 0.0.5.1
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `mlpf-0.0.5/mlpf.egg-info/SOURCES.txt` & `mlpf-0.0.5.1/mlpf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5/setup.py` & `mlpf-0.0.5.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlpf',
-    version='0.0.5',
+    version='0.0.5.1',
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
-    install_requires=['numpy', 'pandapower', 'PYPOWER', 'scikit-learn', 'scipy', 'tqdm', 'torchmetrics']
+    install_requires=['numpy', 'pandapower', 'PYPOWER', 'scikit-learn', 'scipy', 'tqdm']
 )
```

### Comparing `mlpf-0.0.5/test/test_power_flow_loss.py` & `mlpf-0.0.5.1/test/test_power_flow_loss.py`

 * *Files identical despite different names*

