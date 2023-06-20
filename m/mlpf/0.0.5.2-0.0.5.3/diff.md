# Comparing `tmp/mlpf-0.0.5.2.tar.gz` & `tmp/mlpf-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlpf-0.0.5.2.tar", last modified: Tue Jun 20 14:34:27 2023, max compression
+gzip compressed data, was "mlpf-0.0.5.3.tar", last modified: Tue Jun 20 15:12:39 2023, max compression
```

## Comparing `mlpf-0.0.5.2.tar` & `mlpf-0.0.5.3.tar`

### file list

```diff
@@ -1,103 +1,111 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.729261 mlpf-0.0.5.2/
--rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.2/CHANGELOG.md
--rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.2/LICENCE.txt
--rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.2/MANIFEST.in
--rw-rw-rw-   0        0        0     3875 2023-06-20 14:34:27.727073 mlpf-0.0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3258 2023-06-20 14:33:56.000000 mlpf-0.0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.638694 mlpf-0.0.5.2/examples/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.638694 mlpf-0.0.5.2/examples/sklearn/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.658301 mlpf-0.0.5.2/examples/sklearn/loss/
--rw-rw-rw-   0        0        0      963 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/examples/sklearn/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.659593 mlpf-0.0.5.2/examples/sklearn/supervised_power_flow/
--rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.2/examples/sklearn/supervised_power_flow/linear_regression.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.640060 mlpf-0.0.5.2/examples/torch/
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.659593 mlpf-0.0.5.2/examples/torch/loss/
--rw-rw-rw-   0        0        0     1088 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/examples/torch/loss/from_arrays.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.660773 mlpf-0.0.5.2/examples/torch/supervised_power_flow/
--rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.2/examples/torch/supervised_power_flow/gcn.py
--rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.2/examples/torch/supervised_power_flow/mlp.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.661858 mlpf-0.0.5.2/mlpf/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.680080 mlpf-0.0.5.2/mlpf/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.680080 mlpf-0.0.5.2/mlpf/data/analysis/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.685006 mlpf-0.0.5.2/mlpf/data/analysis/description/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/__init__.py
--rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/describe.py
--rw-rw-rw-   0        0        0     2723 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/describe_grid.py
--rw-rw-rw-   0        0        0     2570 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/description/describe_node.py
--rw-rw-rw-   0        0        0     6511 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.687441 mlpf-0.0.5.2/mlpf/data/analysis/visualization/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/__init__.py
--rw-rw-rw-   0        0        0     4564 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/grid_pdf_estimates.py
--rw-rw-rw-   0        0        0     4585 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/node_pdf_estimates.py
--rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/analysis/visualization/visualize.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/conversion/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:22:21.000000 mlpf-0.0.5.2/mlpf/data/conversion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/conversion/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:25:02.000000 mlpf-0.0.5.2/mlpf/data/conversion/numpy/__init__.py
--rw-rw-rw-   0        0        0     1788 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/conversion/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/conversion/torch/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:25:07.000000 mlpf-0.0.5.2/mlpf/data/conversion/torch/__init__.py
--rw-rw-rw-   0        0        0     1360 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/conversion/torch/power_flow.py
--rw-rw-rw-   0        0        0      475 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/conversion/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.688564 mlpf-0.0.5.2/mlpf/data/data/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.692007 mlpf-0.0.5.2/mlpf/data/data/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/data/numpy/__init__.py
--rw-rw-rw-   0        0        0     4001 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/data/numpy/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.692869 mlpf-0.0.5.2/mlpf/data/data/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/data/torch/__init__.py
--rw-rw-rw-   0        0        0     4033 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/data/torch/power_flow.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.692869 mlpf-0.0.5.2/mlpf/data/generate/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/generate/__init__.py
--rw-rw-rw-   0        0        0     4509 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/generate/generate_uniform_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.694702 mlpf-0.0.5.2/mlpf/data/loading/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/loading/__init__.py
--rw-rw-rw-   0        0        0     3604 2023-06-20 14:27:26.000000 mlpf-0.0.5.2/mlpf/data/loading/load_data.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.696481 mlpf-0.0.5.2/mlpf/data/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/__init__.py
--rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/masks.py
--rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/pandapower_networks.py
--rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/data/utils/saving.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.700871 mlpf-0.0.5.2/mlpf/enumerations/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/__init__.py
--rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/branch_table.py
--rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/bus_table.py
--rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/bus_type.py
--rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/gencost_table.py
--rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/generator_table.py
--rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/power_flow_ids.py
--rw-rw-rw-   0        0        0     1327 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/enumerations/ppc_tables.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.700871 mlpf-0.0.5.2/mlpf/loss/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.722978 mlpf-0.0.5.2/mlpf/loss/numpy/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/__init__.py
--rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/bound_errors.py
--rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/power_flow.py
--rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/numpy/utils.py
--rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/relative_values.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.722978 mlpf-0.0.5.2/mlpf/loss/torch/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/torch/__init__.py
--rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/torch/bound_errors.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.725995 mlpf-0.0.5.2/mlpf/loss/torch/metrics/
--rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.2/mlpf/loss/torch/metrics/__init__.py
--rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.2/mlpf/loss/torch/metrics/power_flow.py
--rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.2/mlpf/loss/torch/power_flow.py
--rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/loss/torch/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.727073 mlpf-0.0.5.2/mlpf/utils/
--rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/utils/__init__.py
--rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/utils/ppc.py
--rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.2/mlpf/utils/standard_scaler.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.680080 mlpf-0.0.5.2/mlpf.egg-info/
--rw-rw-rw-   0        0        0     3875 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2272 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-20 14:34:27.000000 mlpf-0.0.5.2/mlpf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 14:34:27.729261 mlpf-0.0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1000 2023-06-20 14:31:29.000000 mlpf-0.0.5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:34:27.727073 mlpf-0.0.5.2/test/
--rw-rw-rw-   0        0        0     3020 2023-06-20 14:33:52.000000 mlpf-0.0.5.2/test/test_power_flow_loss.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.048492 mlpf-0.0.5.3/
+-rw-rw-rw-   0        0        0      121 2023-06-19 13:08:07.000000 mlpf-0.0.5.3/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1075 2023-06-17 23:02:26.000000 mlpf-0.0.5.3/LICENCE.txt
+-rw-rw-rw-   0        0        0       30 2023-06-17 23:02:26.000000 mlpf-0.0.5.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     3873 2023-06-20 15:12:39.048492 mlpf-0.0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3256 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.978350 mlpf-0.0.5.3/examples/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.976916 mlpf-0.0.5.3/examples/data/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.990460 mlpf-0.0.5.3/examples/data/analysis/
+-rw-rw-rw-   0        0        0     1390 2023-06-20 14:58:12.000000 mlpf-0.0.5.3/examples/data/analysis/describe_grid.py
+-rw-rw-rw-   0        0        0     1238 2023-06-20 14:58:12.000000 mlpf-0.0.5.3/examples/data/analysis/describe_node.py
+-rw-rw-rw-   0        0        0     1332 2023-06-20 14:58:12.000000 mlpf-0.0.5.3/examples/data/analysis/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     1249 2023-06-20 14:58:12.000000 mlpf-0.0.5.3/examples/data/analysis/node_pdf_estimates.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.990460 mlpf-0.0.5.3/examples/data/generate/
+-rw-rw-rw-   0        0        0     1085 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/examples/data/generate/uniform.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.978350 mlpf-0.0.5.3/examples/sklearn/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.991727 mlpf-0.0.5.3/examples/sklearn/loss/
+-rw-rw-rw-   0        0        0      963 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/examples/sklearn/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.991727 mlpf-0.0.5.3/examples/sklearn/supervised_power_flow/
+-rw-rw-rw-   0        0        0     2985 2023-06-20 13:03:26.000000 mlpf-0.0.5.3/examples/sklearn/supervised_power_flow/linear_regression.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.979038 mlpf-0.0.5.3/examples/torch/
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.992938 mlpf-0.0.5.3/examples/torch/loss/
+-rw-rw-rw-   0        0        0     1088 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/examples/torch/loss/from_arrays.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.993940 mlpf-0.0.5.3/examples/torch/supervised_power_flow/
+-rw-rw-rw-   0        0        0     5287 2023-06-20 13:18:24.000000 mlpf-0.0.5.3/examples/torch/supervised_power_flow/gcn.py
+-rw-rw-rw-   0        0        0     4525 2023-06-20 13:15:42.000000 mlpf-0.0.5.3/examples/torch/supervised_power_flow/mlp.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:38.993940 mlpf-0.0.5.3/mlpf/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.020707 mlpf-0.0.5.3/mlpf/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.021717 mlpf-0.0.5.3/mlpf/data/analysis/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/analysis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.023872 mlpf-0.0.5.3/mlpf/data/analysis/description/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/analysis/description/__init__.py
+-rw-rw-rw-   0        0        0     1214 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/analysis/description/describe.py
+-rw-rw-rw-   0        0        0     1447 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/data/analysis/description/describe_grid.py
+-rw-rw-rw-   0        0        0     1396 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/data/analysis/description/describe_node.py
+-rw-rw-rw-   0        0        0     6433 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/data/analysis/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.025898 mlpf-0.0.5.3/mlpf/data/analysis/visualization/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/analysis/visualization/__init__.py
+-rw-rw-rw-   0        0        0     3420 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/data/analysis/visualization/grid_pdf_estimates.py
+-rw-rw-rw-   0        0        0     3473 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/data/analysis/visualization/node_pdf_estimates.py
+-rw-rw-rw-   0        0        0     4580 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/analysis/visualization/visualize.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.027229 mlpf-0.0.5.3/mlpf/data/conversion/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/conversion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.028283 mlpf-0.0.5.3/mlpf/data/conversion/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/conversion/numpy/__init__.py
+-rw-rw-rw-   0        0        0     1788 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/conversion/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.029744 mlpf-0.0.5.3/mlpf/data/conversion/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/conversion/torch/__init__.py
+-rw-rw-rw-   0        0        0     1360 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/conversion/torch/power_flow.py
+-rw-rw-rw-   0        0        0      475 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/conversion/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.029744 mlpf-0.0.5.3/mlpf/data/data/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.031139 mlpf-0.0.5.3/mlpf/data/data/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/data/numpy/__init__.py
+-rw-rw-rw-   0        0        0     4001 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/data/numpy/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.032141 mlpf-0.0.5.3/mlpf/data/data/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/data/torch/__init__.py
+-rw-rw-rw-   0        0        0     4033 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/data/torch/power_flow.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.032141 mlpf-0.0.5.3/mlpf/data/generate/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/generate/__init__.py
+-rw-rw-rw-   0        0        0     3523 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/data/generate/generate_uniform_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.033584 mlpf-0.0.5.3/mlpf/data/loading/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/loading/__init__.py
+-rw-rw-rw-   0        0        0     3604 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/mlpf/data/loading/load_data.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.035587 mlpf-0.0.5.3/mlpf/data/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/utils/__init__.py
+-rw-rw-rw-   0        0        0     1428 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/utils/masks.py
+-rw-rw-rw-   0        0        0     3748 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/utils/pandapower_networks.py
+-rw-rw-rw-   0        0        0     1208 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/data/utils/saving.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.039587 mlpf-0.0.5.3/mlpf/enumerations/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/__init__.py
+-rw-rw-rw-   0        0        0      483 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/branch_table.py
+-rw-rw-rw-   0        0        0      443 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/bus_table.py
+-rw-rw-rw-   0        0        0      169 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/bus_type.py
+-rw-rw-rw-   0        0        0      240 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/gencost_table.py
+-rw-rw-rw-   0        0        0      703 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/generator_table.py
+-rw-rw-rw-   0        0        0      295 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/enumerations/power_flow_ids.py
+-rw-rw-rw-   0        0        0     1254 2023-06-20 15:07:50.000000 mlpf-0.0.5.3/mlpf/enumerations/ppc_tables.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.039587 mlpf-0.0.5.3/mlpf/loss/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.042068 mlpf-0.0.5.3/mlpf/loss/numpy/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/numpy/__init__.py
+-rw-rw-rw-   0        0        0     2286 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/numpy/bound_errors.py
+-rw-rw-rw-   0        0        0     3609 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/numpy/power_flow.py
+-rw-rw-rw-   0        0        0      868 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/numpy/utils.py
+-rw-rw-rw-   0        0        0     1141 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/relative_values.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.044658 mlpf-0.0.5.3/mlpf/loss/torch/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/torch/__init__.py
+-rw-rw-rw-   0        0        0     2289 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/torch/bound_errors.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.045662 mlpf-0.0.5.3/mlpf/loss/torch/metrics/
+-rw-rw-rw-   0        0        0        0 2023-06-17 16:14:26.000000 mlpf-0.0.5.3/mlpf/loss/torch/metrics/__init__.py
+-rw-rw-rw-   0        0        0     2699 2023-06-17 16:14:26.000000 mlpf-0.0.5.3/mlpf/loss/torch/metrics/power_flow.py
+-rw-rw-rw-   0        0        0     5349 2023-06-11 16:38:41.000000 mlpf-0.0.5.3/mlpf/loss/torch/power_flow.py
+-rw-rw-rw-   0        0        0      820 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/loss/torch/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.046662 mlpf-0.0.5.3/mlpf/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/utils/__init__.py
+-rw-rw-rw-   0        0        0      449 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/utils/ppc.py
+-rw-rw-rw-   0        0        0      655 2023-06-11 14:41:11.000000 mlpf-0.0.5.3/mlpf/utils/standard_scaler.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.020707 mlpf-0.0.5.3/mlpf.egg-info/
+-rw-rw-rw-   0        0        0     3873 2023-06-20 15:12:38.000000 mlpf-0.0.5.3/mlpf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2476 2023-06-20 15:12:38.000000 mlpf-0.0.5.3/mlpf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 15:12:38.000000 mlpf-0.0.5.3/mlpf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-06-20 15:12:38.000000 mlpf-0.0.5.3/mlpf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-06-20 15:12:38.000000 mlpf-0.0.5.3/mlpf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      421 2023-06-17 16:14:26.000000 mlpf-0.0.5.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 15:12:39.048492 mlpf-0.0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1000 2023-06-20 15:06:29.000000 mlpf-0.0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 15:12:39.047835 mlpf-0.0.5.3/test/
+-rw-rw-rw-   0        0        0     3020 2023-06-20 14:41:06.000000 mlpf-0.0.5.3/test/test_power_flow_loss.py
```

### Comparing `mlpf-0.0.5.2/LICENCE.txt` & `mlpf-0.0.5.3/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/PKG-INFO` & `mlpf-0.0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -74,15 +74,15 @@
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
   edge_index,
   active_powers_pu,
   reactive_powers_pu,
   voltages_pu, angles_rad,
   conductances_pu,
-    susceptances_pu
+  susceptances_pu
 )
 ```
 
 #### torch
 
 ```python
```

### Comparing `mlpf-0.0.5.2/README.md` & `mlpf-0.0.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
   edge_index,
   active_powers_pu,
   reactive_powers_pu,
   voltages_pu, angles_rad,
   conductances_pu,
-    susceptances_pu
+  susceptances_pu
 )
 ```
 
 #### torch
 
 ```python
```

### Comparing `mlpf-0.0.5.2/examples/sklearn/loss/from_arrays.py` & `mlpf-0.0.5.3/examples/sklearn/loss/from_arrays.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/examples/sklearn/supervised_power_flow/linear_regression.py` & `mlpf-0.0.5.3/examples/sklearn/supervised_power_flow/linear_regression.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/examples/torch/loss/from_arrays.py` & `mlpf-0.0.5.3/examples/torch/loss/from_arrays.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/examples/torch/supervised_power_flow/gcn.py` & `mlpf-0.0.5.3/examples/torch/supervised_power_flow/gcn.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/examples/torch/supervised_power_flow/mlp.py` & `mlpf-0.0.5.3/examples/torch/supervised_power_flow/mlp.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/analysis/description/describe.py` & `mlpf-0.0.5.3/mlpf/data/analysis/description/describe.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/analysis/description/describe_grid.py` & `mlpf-0.0.5.3/mlpf/data/analysis/description/describe_grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,19 @@
-import hydra
-import warnings
-
-import pandas as pd
+from typing import Dict, List, Union
 
 from pandas import DataFrame
-from typing import Dict, List, Union
 
-from mlpf.data.analysis.utils import ppc_list_extract_bus_type, table_and_columns_from_config
 from mlpf.data.analysis.description.describe import generate_description
-from mlpf.data.loading.load_data import load_data, autodetect_load_ppc
+from mlpf.data.analysis.utils import ppc_list_extract_bus_type
 from mlpf.enumerations.branch_table import BranchTableIds
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.bus_type import BusTypeIds
 from mlpf.enumerations.gencost_table import GeneratorCostTableIds
 from mlpf.enumerations.generator_table import GeneratorTableIds
-from mlpf.enumerations.ppc_tables import get_table_ids, PPCTables
+from mlpf.enumerations.ppc_tables import PPCTables
 
 
 def describe_grid(ppc_list: List[Dict],
                   table: PPCTables,
                   bus_type: BusTypeIds = None,
                   columns: List[Union[BusTableIds, GeneratorTableIds, BranchTableIds, GeneratorCostTableIds]] = None) -> DataFrame:
     """
@@ -30,39 +25,7 @@
     :param columns: List of table id enums specifying which columns to describe.
     :return: DataFrame object containing the description. To view the stats summary print the description DataFrame.
     """
 
     dataset = ppc_list_extract_bus_type(ppc_list, table, bus_type)
 
     return generate_description(dataset, table, columns)
-
-
-@hydra.main(version_base=None, config_path="../configs", config_name="default")
-def main(cfg):
-    """
-    Load the dataset and describe it. Use the hydra config default or overwrite the command line args.
-
-    :param cfg: Hydra config. The config has the following fields:
-    * bus_type: int or null; the values follow the ppc convention
-    * columns: List[int] or null; the columns of the specified table
-    * data_path: str; where to find the dataset
-    * table: str; ppc table string
-    :return:
-    """
-    ppc_list = autodetect_load_ppc(cfg.data_path)
-
-    bus_type = BusTypeIds(cfg.bus_type) if cfg.bus_type is not None else None
-    table, columns = table_and_columns_from_config(cfg)
-
-    pd.options.display.max_columns = None
-
-    description = describe_grid(ppc_list, table=table, bus_type=bus_type, columns=columns)
-    pd.set_option('display.max_columns', None)
-    pd.set_option('display.width', None)
-
-    print()
-    print("Bus type:", bus_type.name if bus_type is not None else "all")
-    print(description)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `mlpf-0.0.5.2/mlpf/data/analysis/description/describe_node.py` & `mlpf-0.0.5.3/mlpf/data/analysis/visualization/node_pdf_estimates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,65 +1,68 @@
-import hydra
-import warnings
-
-import pandas as pd
-
-from pandas import DataFrame
 from typing import Dict, List, Union
 
-from mlpf.data.analysis.utils import ppc_list_extract_nodes, table_and_columns_from_config
-from mlpf.data.analysis.description.describe import generate_description
-from mlpf.data.loading.load_data import load_data, autodetect_load_ppc
+from matplotlib.axes import Axes
+from numpy import ndarray
+
+from mlpf.data.analysis.utils import generate_data_frame, ppc_list_extract_nodes
+from mlpf.data.analysis.visualization.visualize import visualize_pdf_data_frame, visualize_histogram_data_frame
 from mlpf.enumerations.branch_table import BranchTableIds
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.gencost_table import GeneratorCostTableIds
 from mlpf.enumerations.generator_table import GeneratorTableIds
-from mlpf.enumerations.ppc_tables import get_table_ids, PPCTables
+from mlpf.enumerations.ppc_tables import PPCTables
 
 
-def describe_nodes(ppc_list: List[Dict],
-                   table: PPCTables,
-                   node_numbers: List[int],
-                   columns: List[Union[BusTableIds, GeneratorTableIds, BranchTableIds, GeneratorCostTableIds]] = None) -> DataFrame:
+# TODO test for crashes on all grids
+def visualize_node_pdfs(ppc_list: List[Dict],
+                        table: PPCTables,
+                        node_numbers: List[int],
+                        columns: List[Union[BusTableIds, GeneratorTableIds, BranchTableIds, GeneratorCostTableIds]] = None,
+                        kernel: str = "tophat",
+                        bandwidth_coeff: float = 0.05,
+                        axes: ndarray[Axes] = None):
     """
-    Return a description DataFrame similar to pandas' _describe_ function.
+    Estimate and plot the probability density function of each specified column for the specified node and table in the ppc list. If no axes list is provided
+    new figures will be created.
 
     :param ppc_list: List of pypower case files.
     :param table: PPCTables object specifying which table to describe.
     :param node_numbers: The bus number in the bus table of the node to describe.
     :param columns: List of table id enums specifying which columns to describe.
-    :return: DataFrame object containing the description. To view the stats summary print the description DataFrame.
+    :param kernel: Name of kernel method to use. The function calls sklearn.neighbors.KernelDensity so it must
+    be one supported by this function.
+    :param bandwidth_coeff: A parameter that effects the resolution of the pdf estimate. Too small of a value
+    will overfit to the given samples. To large of a value will not capture enough detail.
+    :param axes: A numpy array of Matplotlib.PyPlot.Axes objects onto which to plot the estimates. If None,
+    new figures will be created for every column.
+    :return:
     """
 
-    dataset = ppc_list_extract_nodes(ppc_list, table, node_numbers)
-    return generate_description(dataset, table, columns)
+    dataset = ppc_list_extract_nodes(ppc_list, table, node_numbers=node_numbers)
+    data_frame = generate_data_frame(dataset, table, columns)
 
+    visualize_pdf_data_frame(data_frame, kernel, bandwidth_coeff, axes)
 
-@hydra.main(version_base=None, config_path="../configs", config_name="default")
-def main(cfg):
+
+def visualize_node_histograms(ppc_list: List[Dict],
+                              table: PPCTables,
+                              node_numbers: List[int],
+                              columns: List[Union[BusTableIds, GeneratorTableIds, BranchTableIds, GeneratorCostTableIds]] = None,
+                              bins: int = 10,
+                              axes: ndarray[Axes] = None):
     """
-    Load the dataset and describe a node in it. Use the hydra config default or overwrite the command line args.
+    Estimate and plot the histogram of each specified column for the specified node and table in the ppc list.
 
-    :param cfg: Hydra config. The config has the following fields:
-    * columns: List[int] or null; the columns of the specified table
-    * data_path: str; where to find the dataset
-    * node_number: List[int]; which node to describe
-    * table: str; ppc table string
+    :param ppc_list: List of pypower case files.
+    :param table: PPCTables object specifying which table to describe.
+    :param node_numbers: The bus number in the bus table of the node to describe.
+    :param columns: List of table id enums specifying which columns to describe.
+    be one supported by this function.
+    :param bins: How many bins to work with.
+    :param axes: Ndarray of Axes
     :return:
     """
-    ppc_list = autodetect_load_ppc(cfg.data_path)
-
-    table, columns = table_and_columns_from_config(cfg)
-
-    pd.options.display.max_columns = None
-
-    description = describe_nodes(ppc_list, table=table, node_numbers=cfg.node_numbers, columns=columns)
-    pd.set_option('display.max_columns', None)
-    pd.set_option('display.width', None)
-
-    print()
-    print(f"Node # {cfg.node_numbers}")
-    print(description)
 
+    dataset = ppc_list_extract_nodes(ppc_list, table, node_numbers=node_numbers)
+    data_frame = generate_data_frame(dataset, table, columns)
 
-if __name__ == "__main__":
-    main()
+    visualize_histogram_data_frame(data_frame, bins, axes)
```

### Comparing `mlpf-0.0.5.2/mlpf/data/analysis/utils.py` & `mlpf-0.0.5.3/mlpf/data/analysis/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import numpy as np
+from typing import Dict, List, Union, Tuple, Any
 
+import numpy as np
+from matplotlib import pyplot as plt
 from numpy import ndarray
 from pandas import DataFrame
-from typing import Dict, List, Union, Tuple, Type
-
-from matplotlib import pyplot as plt
 
 from mlpf.enumerations.branch_table import BranchTableIds
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.bus_type import BusTypeIds
 from mlpf.enumerations.gencost_table import GeneratorCostTableIds
 from mlpf.enumerations.generator_table import GeneratorTableIds
 from mlpf.enumerations.ppc_tables import PPCTables, get_table_ids
@@ -133,15 +132,15 @@
         column_names = [column_names[i] for i in column_ids]
     else:
         column_ids = [i for i in range(dataset.shape[1])]
 
     return DataFrame(data=dataset[:, column_ids], columns=column_names)
 
 
-def table_and_columns_from_config(cfg) -> Tuple[PPCTables, Union[List[Type[BusTableIds | BranchTableIds | GeneratorTableIds | GeneratorCostTableIds]], None]]:
+def table_and_columns_from_config(cfg) -> Tuple[PPCTables, Union[List[Any], None]]:
     """
     Extract the table and column objects using the given config.
 
     :param cfg: Hydra config.
     :return: PPCTables
     """
     table = PPCTables(cfg.table)
```

### Comparing `mlpf-0.0.5.2/mlpf/data/analysis/visualization/grid_pdf_estimates.py` & `mlpf-0.0.5.3/mlpf/data/analysis/visualization/grid_pdf_estimates.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-import hydra
-
 from typing import Dict, List, Union
-from matplotlib import pyplot as plt
+
 from matplotlib.axes import Axes
 from numpy import ndarray
 
-from mlpf.data.analysis.utils import generate_data_frame, ppc_list_extract_bus_type, table_and_columns_from_config, create_subplots_grid
+from mlpf.data.analysis.utils import generate_data_frame, ppc_list_extract_bus_type
 from mlpf.data.analysis.visualization.visualize import visualize_pdf_data_frame, visualize_histogram_data_frame
-from mlpf.data.loading.load_data import load_data, autodetect_load_ppc
 from mlpf.enumerations.branch_table import BranchTableIds
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.bus_type import BusTypeIds
 from mlpf.enumerations.gencost_table import GeneratorCostTableIds
 from mlpf.enumerations.generator_table import GeneratorTableIds
 from mlpf.enumerations.ppc_tables import PPCTables
 
@@ -66,36 +63,7 @@
     :return:
     """
 
     dataset = ppc_list_extract_bus_type(ppc_list, table, bus_type)
     data_frame = generate_data_frame(dataset, table, columns)
 
     visualize_histogram_data_frame(data_frame, bins, axes)
-
-
-@hydra.main(version_base=None, config_path="../configs", config_name="default")
-def main(cfg):
-    ppc_list = autodetect_load_ppc(cfg.data_path)
-
-    bus_type = BusTypeIds(cfg.bus_type) if cfg.bus_type is not None else None
-
-    table, columns = table_and_columns_from_config(cfg)
-
-    num_columns = len(columns) if columns is not None else ppc_list[0][table.value].shape[1]
-    fig, axes = create_subplots_grid(num_columns)
-
-    fig.tight_layout()
-    visualize_grid_pdfs(ppc_list, table, bus_type=bus_type, columns=columns, kernel=cfg.visualization.kernel, bandwidth_coeff=cfg.visualization.bandwidth_coeff, axes=axes)
-
-    for ax in axes.flatten():
-        ax.set_ylim(bottom=0)
-
-    fig, axes = create_subplots_grid(num_columns)
-    fig.tight_layout()
-
-    visualize_grid_histograms(ppc_list, table, bus_type=bus_type, columns=columns, bins=cfg.visualization.bins, axes=axes)
-
-    plt.show()
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `mlpf-0.0.5.2/mlpf/data/analysis/visualization/visualize.py` & `mlpf-0.0.5.3/mlpf/data/analysis/visualization/visualize.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/conversion/numpy/power_flow.py` & `mlpf-0.0.5.3/mlpf/data/conversion/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/conversion/torch/power_flow.py` & `mlpf-0.0.5.3/mlpf/data/conversion/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/data/numpy/power_flow.py` & `mlpf-0.0.5.3/mlpf/data/data/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/data/torch/power_flow.py` & `mlpf-0.0.5.3/mlpf/data/data/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/loading/load_data.py` & `mlpf-0.0.5.3/mlpf/data/loading/load_data.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/utils/masks.py` & `mlpf-0.0.5.3/mlpf/data/utils/masks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/utils/pandapower_networks.py` & `mlpf-0.0.5.3/mlpf/data/utils/pandapower_networks.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/data/utils/saving.py` & `mlpf-0.0.5.3/mlpf/data/utils/saving.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/enumerations/generator_table.py` & `mlpf-0.0.5.3/mlpf/enumerations/generator_table.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/enumerations/ppc_tables.py` & `mlpf-0.0.5.3/mlpf/enumerations/ppc_tables.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from enum import Enum, IntEnum
-from typing import Type
+from enum import Enum
+from typing import Type, Any
 
 from mlpf.enumerations.branch_table import BranchTableIds
 from mlpf.enumerations.bus_table import BusTableIds
 from mlpf.enumerations.gencost_table import GeneratorCostTableIds
 from mlpf.enumerations.generator_table import GeneratorTableIds
 
 
@@ -14,15 +14,15 @@
     BaseMVA = "baseMVA"
     Branch = "branch"
     Bus = "bus"
     Generator = "gen"
     GeneratorCost = "gencost"
 
 
-def get_table_ids(table: PPCTables) -> Type[BusTableIds | BranchTableIds | GeneratorTableIds | GeneratorCostTableIds]:
+def get_table_ids(table: PPCTables) -> Type[Any]:
     """
     Get the table ids enum corresponding to the given table.
 
     :param table: PPCTables object representing a table in the pypower case format.
     :return: Table ids enum
     """
     # get the corresponding table ids
```

### Comparing `mlpf-0.0.5.2/mlpf/loss/numpy/bound_errors.py` & `mlpf-0.0.5.3/mlpf/loss/numpy/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/numpy/power_flow.py` & `mlpf-0.0.5.3/mlpf/loss/numpy/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/numpy/utils.py` & `mlpf-0.0.5.3/mlpf/loss/numpy/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/relative_values.py` & `mlpf-0.0.5.3/mlpf/loss/relative_values.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/torch/bound_errors.py` & `mlpf-0.0.5.3/mlpf/loss/torch/bound_errors.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/torch/metrics/power_flow.py` & `mlpf-0.0.5.3/mlpf/loss/torch/metrics/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/torch/power_flow.py` & `mlpf-0.0.5.3/mlpf/loss/torch/power_flow.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/loss/torch/utils.py` & `mlpf-0.0.5.3/mlpf/loss/torch/utils.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf/utils/standard_scaler.py` & `mlpf-0.0.5.3/mlpf/utils/standard_scaler.py`

 * *Files identical despite different names*

### Comparing `mlpf-0.0.5.2/mlpf.egg-info/PKG-INFO` & `mlpf-0.0.5.3/mlpf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlpf
-Version: 0.0.5.2
+Version: 0.0.5.3
 Summary: Machine learning for power flow
 Home-page: 
 Author: Viktor Todosijevic
 Author-email: todosijevicviktor998@gmail.com
 License: MIT
 Keywords: machine learning,power
 Classifier: Development Status :: 3 - Alpha
@@ -74,15 +74,15 @@
 
 active_power_losses_pu, reactive_power_losses_pu = power_flow_errors(
   edge_index,
   active_powers_pu,
   reactive_powers_pu,
   voltages_pu, angles_rad,
   conductances_pu,
-    susceptances_pu
+  susceptances_pu
 )
 ```
 
 #### torch
 
 ```python
```

### Comparing `mlpf-0.0.5.2/mlpf.egg-info/SOURCES.txt` & `mlpf-0.0.5.3/mlpf.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 CHANGELOG.md
 LICENCE.txt
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
+examples/data/analysis/describe_grid.py
+examples/data/analysis/describe_node.py
+examples/data/analysis/grid_pdf_estimates.py
+examples/data/analysis/node_pdf_estimates.py
+examples/data/generate/uniform.py
 examples/sklearn/loss/from_arrays.py
 examples/sklearn/supervised_power_flow/linear_regression.py
 examples/torch/loss/from_arrays.py
 examples/torch/supervised_power_flow/gcn.py
 examples/torch/supervised_power_flow/mlp.py
 mlpf/__init__.py
 mlpf.egg-info/PKG-INFO
```

### Comparing `mlpf-0.0.5.2/setup.py` & `mlpf-0.0.5.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ]
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='mlpf',
-    version='0.0.5.2',
+    version='0.0.5.3',
     description='Machine learning for power flow',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='',
     author='Viktor Todosijevic',
     author_email='todosijevicviktor998@gmail.com',
     license='MIT',
```

### Comparing `mlpf-0.0.5.2/test/test_power_flow_loss.py` & `mlpf-0.0.5.3/test/test_power_flow_loss.py`

 * *Files identical despite different names*

