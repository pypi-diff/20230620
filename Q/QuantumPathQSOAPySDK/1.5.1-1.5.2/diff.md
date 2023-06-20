# Comparing `tmp/QuantumPathQSOAPySDK-1.5.1.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.1.tar", last modified: Mon Jun 19 11:12:21 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.2.tar", last modified: Tue Jun 20 08:32:17 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.1.tar` & `QuantumPathQSOAPySDK-1.5.2.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.662078 QuantumPathQSOAPySDK-1.5.1/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0      928 2023-06-19 11:12:21.660064 QuantumPathQSOAPySDK-1.5.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.547377 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    41637 2023-06-14 10:34:16.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.566316 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.573301 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     8778 2023-06-19 11:09:52.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    27335 2023-06-19 11:02:12.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.577287 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4884 2023-06-12 08:01:23.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.582272 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53259 2023-06-12 08:01:11.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.607205 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.618175 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.631152 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      144 2023-06-13 07:52:54.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     1734 2023-06-09 11:25:34.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.564321 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      928 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-19 11:12:21.664652 QuantumPathQSOAPySDK-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      973 2023-06-19 10:58:38.000000 QuantumPathQSOAPySDK-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.634390 QuantumPathQSOAPySDK-1.5.1/test/
--rw-rw-rw-   0        0        0       83 2023-06-14 15:03:15.000000 QuantumPathQSOAPySDK-1.5.1/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.647465 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.657084 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   100345 2023-06-19 11:07:44.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     7478 2023-05-22 11:55:54.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0   183366 2023-06-01 14:20:56.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitGates.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.380949 QuantumPathQSOAPySDK-1.5.2/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-06-20 08:32:17.378940 QuantumPathQSOAPySDK-1.5.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.223635 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    41637 2023-06-14 10:34:16.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.267497 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.274525 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     8778 2023-06-19 11:09:52.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    27335 2023-06-19 11:02:12.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.280743 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4884 2023-06-12 08:01:23.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.287583 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53331 2023-06-20 08:30:05.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.319704 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.330845 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.347819 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      144 2023-06-13 07:52:54.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     1734 2023-06-09 11:25:34.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.264515 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-06-20 08:32:17.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-06-20 08:32:17.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:32:17.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 08:32:17.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-20 08:32:17.000000 QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:32:17.380949 QuantumPathQSOAPySDK-1.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-06-20 08:30:47.000000 QuantumPathQSOAPySDK-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.351832 QuantumPathQSOAPySDK-1.5.2/test/
+-rw-rw-rw-   0        0        0       83 2023-06-14 15:03:15.000000 QuantumPathQSOAPySDK-1.5.2/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.364883 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:32:17.375054 QuantumPathQSOAPySDK-1.5.2/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.2/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   100345 2023-06-19 11:07:44.000000 QuantumPathQSOAPySDK-1.5.2/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     7478 2023-05-22 11:55:54.000000 QuantumPathQSOAPySDK-1.5.2/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0   184849 2023-06-20 07:35:19.000000 QuantumPathQSOAPySDK-1.5.2/test/test_circuit/test_CircuitGates.py
```

### Comparing `QuantumPathQSOAPySDK-1.5.1/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.1
+Version: 1.5.2
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files 1% similar despite different names*

```diff
@@ -952,15 +952,15 @@
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int | list
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        argument: string
+        argument: str | int | float
             Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
@@ -970,15 +970,15 @@
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
                 for p in position:
                     checkInputTypes(('position', p, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
-            ('argument', argument, (str, int)),
+            ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
 
         gateSymbol = {'id': 'P', 'arg': str(argument)}
 
@@ -1000,15 +1000,15 @@
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int | list
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        argument: string
+        argument: str | int | float
             Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
@@ -1018,15 +1018,15 @@
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
                 for p in position:
                     checkInputTypes(('position', p, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
-            ('argument', argument, (str, int)),
+            ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
 
         gateSymbol = {'id': 'RX', 'arg': str(argument)}
 
@@ -1048,15 +1048,15 @@
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int | list
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        argument: string
+        argument: str | int | float
             Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
@@ -1066,15 +1066,15 @@
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
                 for p in position:
                     checkInputTypes(('position', p, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
-            ('argument', argument, (str, int)),
+            ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
 
         gateSymbol = {'id': 'RY', 'arg': str(argument)}
 
@@ -1096,15 +1096,15 @@
         ----------
         - Created circuit.
 
         Parameters
         ----------
         position : int | list
             Optional argument. Qubit position to add the gate. If no position are indicated, gate will be added in all qubits. Argument can also be a list of positions.
-        argument: string
+        argument: str | int | float
             Optional argument. Gate angle value. In the case that it is not indicated, it will be pi by default.
         add : bool
             Optional argument. True by default. Indicates whether the gate should be added to the circuit or not. In the case of wanting to add it, it is not necessary to introduce that argument. If you want to create a new gate, you must enter False.
         
         Output
         ----------
         list
@@ -1114,15 +1114,15 @@
                 ('position', position, (int, list))
             )
             if isinstance(position, list):
                 for p in position:
                     checkInputTypes(('position', p, (int,)))
                 checkDifferentPosition(position)
         checkInputTypes(
-            ('argument', argument, (str, int)),
+            ('argument', argument, (str, int, float)),
             ('add', add, (bool,))
         )
         if isinstance(argument, str):
             checkMathExpression('argument', argument)
 
         gateSymbol = {'id': 'RZ', 'arg': str(argument)}
```

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5.1
+Version: 1.5.2
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.2/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/setup.py` & `QuantumPathQSOAPySDK-1.5.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5.1',
+  version='1.5.2',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_circuit/test_CircuitAnnealing.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.2/test/test_circuit/test_CircuitGates.py`

 * *Files 0% similar despite different names*

```diff
@@ -3342,14 +3342,25 @@
 
         gate = circuit.p(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'P', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': '2'}]])
 
+    # P argument FLOAT
+    def test_p_argument_float(self):
+        qsoa = QSOAPlatform()
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.p(1, 1.5)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, {'id': 'P', 'arg': '1.5'})])
+        self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'P', 'arg': '1.5'}]])
+
     # P argument STRING NUMBER
     def test_p_argument_string_number(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitGates()
 
         gate = circuit.p(1, '2')
 
@@ -3592,14 +3603,25 @@
 
         gate = circuit.rx(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RX', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': '2'}]])
 
+    # RX argument FLOAT
+    def test_rx_argument_float(self):
+        qsoa = QSOAPlatform()
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.rx(1, 1.5)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, {'id': 'RX', 'arg': '1.5'})])
+        self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RX', 'arg': '1.5'}]])
+
     # RX argument STRING NUMBER
     def test_rx_argument_string_number(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rx(1, '2')
 
@@ -3842,14 +3864,25 @@
 
         gate = circuit.ry(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RY', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': '2'}]])
 
+    # RY argument FLOAT
+    def test_ry_argument_float(self):
+        qsoa = QSOAPlatform()
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.ry(1, 1.5)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, {'id': 'RY', 'arg': '1.5'})])
+        self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RY', 'arg': '1.5'}]])
+
     # RY argument STRING NUMBER
     def test_ry_argument_string_number(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitGates()
 
         gate = circuit.ry(1, '2')
 
@@ -4092,14 +4125,25 @@
 
         gate = circuit.rz(1, 2)
 
         self.assertIsInstance(gate, list)
         self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': '2'})])
         self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': '2'}]])
 
+    # RZ argument FLOAT
+    def test_rz_argument_float(self):
+        qsoa = QSOAPlatform()
+        circuit = qsoa.CircuitGates()
+
+        gate = circuit.rz(1, 1.5)
+
+        self.assertIsInstance(gate, list)
+        self.assertEqual(gate, [(1, {'id': 'RZ', 'arg': '1.5'})])
+        self.assertEqual(circuit.getCircuitBody(), [[1, {'id': 'RZ', 'arg': '1.5'}]])
+
     # RZ argument STRING NUMBER
     def test_rz_argument_string_number(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitGates()
 
         gate = circuit.rz(1, '2')
```

