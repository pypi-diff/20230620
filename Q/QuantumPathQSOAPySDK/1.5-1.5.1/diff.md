# Comparing `tmp/QuantumPathQSOAPySDK-1.5.tar.gz` & `tmp/QuantumPathQSOAPySDK-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantumPathQSOAPySDK-1.5.tar", last modified: Wed Jun 14 15:03:56 2023, max compression
+gzip compressed data, was "QuantumPathQSOAPySDK-1.5.1.tar", last modified: Mon Jun 19 11:12:21 2023, max compression
```

## Comparing `QuantumPathQSOAPySDK-1.5.tar` & `QuantumPathQSOAPySDK-1.5.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.335047 QuantumPathQSOAPySDK-1.5/
--rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5/MANIFEST.in
--rw-rw-rw-   0        0        0      926 2023-06-14 15:03:56.334456 QuantumPathQSOAPySDK-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.211335 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/
--rw-rw-rw-   0        0        0    41637 2023-06-14 10:34:16.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/QSOAPlatform.py
--rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.251229 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/
--rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.256214 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/annealing/
--rw-rw-rw-   0        0        0     8778 2023-06-12 07:47:27.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
--rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
--rw-rw-rw-   0        0        0    27335 2023-06-12 07:45:18.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/annealing/components.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.259205 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/flow/
--rw-rw-rw-   0        0        0     4884 2023-06-12 08:01:23.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
--rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/flow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.264196 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/gates/
--rw-rw-rw-   0        0        0    53259 2023-06-12 08:01:11.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
--rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/gates/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.285138 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/
--rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/Application.py
--rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/Asset.py
--rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/AssetManagementData.py
--rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
--rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/DeviceItem.py
--rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/Execution.py
--rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/FlowItem.py
--rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
--rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/SolutionItem.py
--rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.293221 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/
--rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/__init__.py
--rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
--rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
--rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.303091 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/
--rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/Context.py
--rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/Exception.py
--rw-rw-rw-   0        0        0      144 2023-06-13 07:52:54.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/__init__.py
--rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/apiConnection.py
--rw-rw-rw-   0        0        0     1734 2023-06-09 11:25:34.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/checker.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.249265 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/
--rw-rw-rw-   0        0        0      926 2023-06-14 15:03:56.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1993 2023-06-14 15:03:56.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-14 15:03:56.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-14 15:03:56.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-06-14 15:03:56.000000 QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5/README.md
--rw-rw-rw-   0        0        0       42 2023-06-14 15:03:56.335047 QuantumPathQSOAPySDK-1.5/setup.cfg
--rw-rw-rw-   0        0        0      971 2023-06-14 15:03:47.000000 QuantumPathQSOAPySDK-1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.312065 QuantumPathQSOAPySDK-1.5/test/
--rw-rw-rw-   0        0        0       83 2023-06-14 15:03:15.000000 QuantumPathQSOAPySDK-1.5/test/test.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.324077 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/__init__.py
--rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_ContextMethods.py
--rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_DynamicMethods.py
--rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_QSOAPlatform.py
--rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_SecurityMethods.py
--rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_StaticMethods.py
-drwxrwxrwx   0        0        0        0 2023-06-14 15:03:56.332061 QuantumPathQSOAPySDK-1.5/test/test_circuit/
--rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5/test/test_circuit/__init__.py
--rw-rw-rw-   0        0        0   100345 2023-06-01 10:30:21.000000 QuantumPathQSOAPySDK-1.5/test/test_circuit/test_CircuitAnnealing.py
--rw-rw-rw-   0        0        0     7478 2023-05-22 11:55:54.000000 QuantumPathQSOAPySDK-1.5/test/test_circuit/test_CircuitFlow.py
--rw-rw-rw-   0        0        0   183366 2023-06-01 14:20:56.000000 QuantumPathQSOAPySDK-1.5/test/test_circuit/test_CircuitGates.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.662078 QuantumPathQSOAPySDK-1.5.1/
+-rw-rw-rw-   0        0        0       25 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      928 2023-06-19 11:12:21.660064 QuantumPathQSOAPySDK-1.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.547377 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/
+-rw-rw-rw-   0        0        0    41637 2023-06-14 10:34:16.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/QSOAPlatform.py
+-rw-rw-rw-   0        0        0       38 2023-06-09 10:56:58.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.566316 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/
+-rw-rw-rw-   0        0        0      145 2023-06-12 08:01:03.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.573301 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/
+-rw-rw-rw-   0        0        0     8778 2023-06-19 11:09:52.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py
+-rw-rw-rw-   0        0        0       46 2023-06-12 08:43:39.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/__init__.py
+-rw-rw-rw-   0        0        0    27335 2023-06-19 11:02:12.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/components.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.577287 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/
+-rw-rw-rw-   0        0        0     4884 2023-06-12 08:01:23.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py
+-rw-rw-rw-   0        0        0       36 2023-06-12 08:44:11.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.582272 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/
+-rw-rw-rw-   0        0        0    53259 2023-06-12 08:01:11.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py
+-rw-rw-rw-   0        0        0       38 2023-06-12 08:44:43.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.607205 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/
+-rw-rw-rw-   0        0        0      746 2022-11-24 16:14:18.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Application.py
+-rw-rw-rw-   0        0        0     1542 2022-12-13 10:45:36.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Asset.py
+-rw-rw-rw-   0        0        0     1448 2022-11-24 16:17:42.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementData.py
+-rw-rw-rw-   0        0        0     1861 2022-11-24 16:18:41.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementResult.py
+-rw-rw-rw-   0        0        0     1088 2023-06-06 09:11:13.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/DeviceItem.py
+-rw-rw-rw-   0        0        0     1289 2022-11-24 16:21:25.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Execution.py
+-rw-rw-rw-   0        0        0      276 2022-11-24 16:21:43.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/FlowItem.py
+-rw-rw-rw-   0        0        0     2615 2022-11-24 16:24:27.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py
+-rw-rw-rw-   0        0        0      280 2022-11-24 16:24:49.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/SolutionItem.py
+-rw-rw-rw-   0        0        0      280 2023-06-09 10:57:16.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.618175 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/
+-rw-rw-rw-   0        0        0      968 2023-06-13 07:53:10.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/__init__.py
+-rw-rw-rw-   0        0        0     9076 2023-06-09 09:56:38.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/connectionPoints.py
+-rw-rw-rw-   0        0        0    10099 2023-06-12 08:01:27.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py
+-rw-rw-rw-   0        0        0     4077 2023-06-13 11:39:31.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.631152 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/
+-rw-rw-rw-   0        0        0     3764 2023-06-09 09:40:06.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Context.py
+-rw-rw-rw-   0        0        0     1047 2022-11-30 08:30:03.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Exception.py
+-rw-rw-rw-   0        0        0      144 2023-06-13 07:52:54.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/__init__.py
+-rw-rw-rw-   0        0        0     1514 2023-06-06 09:42:42.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/apiConnection.py
+-rw-rw-rw-   0        0        0     1734 2023-06-09 11:25:34.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/checker.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.564321 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/
+-rw-rw-rw-   0        0        0      928 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1993 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-06-19 11:12:21.000000 QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      115 2022-07-20 09:04:50.000000 QuantumPathQSOAPySDK-1.5.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 11:12:21.664652 QuantumPathQSOAPySDK-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      973 2023-06-19 10:58:38.000000 QuantumPathQSOAPySDK-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.634390 QuantumPathQSOAPySDK-1.5.1/test/
+-rw-rw-rw-   0        0        0       83 2023-06-14 15:03:15.000000 QuantumPathQSOAPySDK-1.5.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.647465 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:50:59.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/__init__.py
+-rw-rw-rw-   0        0        0     2692 2023-06-14 10:56:41.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_ContextMethods.py
+-rw-rw-rw-   0        0        0    65272 2023-06-14 11:26:03.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_DynamicMethods.py
+-rw-rw-rw-   0        0        0     3244 2023-06-14 11:14:52.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_QSOAPlatform.py
+-rw-rw-rw-   0        0        0     8740 2023-06-14 11:02:20.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_SecurityMethods.py
+-rw-rw-rw-   0        0        0    28777 2023-06-14 11:23:11.000000 QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_StaticMethods.py
+drwxrwxrwx   0        0        0        0 2023-06-19 11:12:21.657084 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/
+-rw-rw-rw-   0        0        0        0 2023-06-14 10:31:46.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/__init__.py
+-rw-rw-rw-   0        0        0   100345 2023-06-19 11:07:44.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitAnnealing.py
+-rw-rw-rw-   0        0        0     7478 2023-05-22 11:55:54.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitFlow.py
+-rw-rw-rw-   0        0        0   183366 2023-06-01 14:20:56.000000 QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitGates.py
```

### Comparing `QuantumPathQSOAPySDK-1.5/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5
+Version: 1.5.1
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/CircuitAnnealing.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         Class,
         Variable,
         Rule,
         OffsetExp,
         LinearExp,
         QuadraticExp,
         SquaredExp,
-        SummatoryExp
+        SummationExp
     )
     
     # CONSTRUCTOR
     def __init__(self):
         """
         CircuitAnnealing object constructor.
```

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/annealing/components.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/annealing/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -712,16 +712,16 @@
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
-        expression : SummatoryExp obj | SquaredExp obj | LinearExp obj | QuadraticExp obj | OffsetExp obj | list
-            Expression to add. It could be an object or a list of following objects: SummatoryExp, SquaredExp, LinearExp, QuadraticExp or OffsetExp.
+        expression : SummationExp obj | SquaredExp obj | LinearExp obj | QuadraticExp obj | OffsetExp obj | list
+            Expression to add. It could be an object or a list of following objects: SummationExp, SquaredExp, LinearExp, QuadraticExp or OffsetExp.
         
         Output
         ----------
         Rule obj
         """
         def appendExpression(expression):
             self.__expressions.append({
@@ -734,23 +734,23 @@
                 'Iterator': expression.getIterator(),
                 'Term1': expression.getTerm1(),
                 'Term2': expression.getTerm2(),
                 'Childs': expression.getChilds()
             })
 
         checkInputTypes(
-            ('expression', expression, (SummatoryExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
+            ('expression', expression, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
         )
         if isinstance(expression, list):
             if not expression:
                 raise ValueError('List of expressions should not be empty')
             
             for e in expression:
                 checkInputTypes(
-                    ('expression', e, (SummatoryExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
+                    ('expression', e, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
                 )
 
             for e in expression:
                 appendExpression(e)
         
         else:
             appendExpression(expression)
@@ -954,16 +954,16 @@
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
-        expression: SummatoryExp obj | LinearExp obj | OffsetExp obj | list
-            Expression or list of expressions to be squared. It could be a Summatory, Linear, or Offset expression.
+        expression: SummationExp obj | LinearExp obj | OffsetExp obj | list
+            Expression or list of expressions to be squared. It could be a Summation, Linear, or Offset expression.
         """
         childs = []
         def appendChild(expression):
             childs.append({
                 'uiID': expression.getUiID(),
                 'Type': expression.getExpType(),
                 'Coefficient': expression.getCoefficient(),
@@ -973,51 +973,51 @@
                 'Iterator': expression.getIterator(),
                 'Term1': expression.getTerm1(),
                 'Term2': expression.getTerm2(),
                 'Childs': expression.getChilds()
             })
 
         checkInputTypes(
-            ('expression', expression, (SummatoryExp, LinearExp, OffsetExp, list))
+            ('expression', expression, (SummationExp, LinearExp, OffsetExp, list))
         )
         if isinstance(expression, list):
             if not expression:
                 raise ValueError('List of expressions should not be empty')
             for e in expression:
-                checkInputTypes(('expression', e, (SummatoryExp, LinearExp, OffsetExp, list)))
+                checkInputTypes(('expression', e, (SummationExp, LinearExp, OffsetExp, list)))
             if isinstance(expression, list):
                 for exp in expression:
                     appendChild(exp)
         
         else:
             appendChild(expression)
 
         super().__init__(expType='SQUARED', childs=childs)
 
 
-# SUMMATORY EXPRESSION
-class SummatoryExp(__Expression):
+# SUMMATION EXPRESSION
+class SummationExp(__Expression):
     
     # CONSTRUCTOR
     def __init__(self, fromValue: int, toValue: int, expression, iterator: str = 'i'): 
         """
-        Create Summatory expression.
+        Create Summation expression.
 
         Prerequisites
         ----------
         - Created rule.
 
         Parameters
         ----------
         fromValue: int | str
-            Start value of the summatory iteration.
+            Start value of the summation iteration.
         toValue: int | str
-            End value of the summatory iteration.
-        expression: SummatoryExp obj | SquaredExp obj | LinearExp obj | QuadraticExp obj | OffsetExp obj | list
-            Expression or list of expressions to be inside of the summatory. It could be a Summatory, Squared, Linear, Quadratic or Offset expression.
+            End value of the summation iteration.
+        expression: SummationExp obj | SquaredExp obj | LinearExp obj | QuadraticExp obj | OffsetExp obj | list
+            Expression or list of expressions to be inside of the summation. It could be a Summation, Squared, Linear, Quadratic or Offset expression.
         iterator: str
             Iterator name.
         """
         childs = []
         def appendChild(expression):
             childs.append({
                 'uiID': expression.getUiID(),
@@ -1031,23 +1031,23 @@
                 'Term2': expression.getTerm2(),
                 'Childs': expression.getChilds()
             })
 
         checkInputTypes(
             ('fromValue', fromValue, (int, str)),
             ('toValue', toValue, (int, str)),
-            ('expression', expression, (SummatoryExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list)),
+            ('expression', expression, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list)),
             ('iterator', iterator, (str,)),
         )
         if isinstance(expression, list):
             if not expression:
                 raise ValueError('List of expressions should not be empty')
             for e in expression:
                 checkInputTypes(
-                    ('expression', e, (SummatoryExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
+                    ('expression', e, (SummationExp, SquaredExp, LinearExp, QuadraticExp, OffsetExp, list))
                 )
             if isinstance(expression, list):
                 for exp in expression:
                     appendChild(exp)
         
         else:
             appendChild(expression)
```

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/flow/CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/circuit/gates/CircuitGates.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/Application.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Application.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/Asset.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Asset.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/AssetManagementData.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementData.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/AssetManagementResult.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/AssetManagementResult.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/DeviceItem.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/DeviceItem.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/Execution.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/Execution.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/objects/QuantumExecutionHistoryEntry.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/__init__.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/__init__.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/connectionPoints.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/connectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/dynamicConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/qsoa/securityConnectionPoints.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/Context.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Context.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/Exception.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/Exception.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/apiConnection.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/apiConnection.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK/utils/checker.py` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK/utils/checker.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/PKG-INFO` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QuantumPathQSOAPySDK
-Version: 1.5
+Version: 1.5.1
 Summary: QuantumPath qSOA Python SDK
 Home-page: https://core.quantumpath.app/
 Author: QuantumPath
 License: UNKNOWN
 Keywords: quantum,quantumpath,qSOA,sdk,quantum applications,quantum software
 Platform: UNKNOWN
 Classifier: Topic :: Scientific/Engineering
```

### Comparing `QuantumPathQSOAPySDK-1.5/QuantumPathQSOAPySDK.egg-info/SOURCES.txt` & `QuantumPathQSOAPySDK-1.5.1/QuantumPathQSOAPySDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/setup.py` & `QuantumPathQSOAPySDK-1.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   'Intended Audience :: Developers',
   'Intended Audience :: Education',
   'Intended Audience :: Information Technology'
 ]
 
 setup(
   name='QuantumPathQSOAPySDK',
-  version='1.5',
+  version='1.5.1',
   description='QuantumPath qSOA Python SDK',
   long_description=open('README.md').read(),
   long_description_content_type = 'text/markdown',
   url='https://core.quantumpath.app/',
   author='QuantumPath',
   classifiers=classifiers,
   keywords='quantum, quantumpath, qSOA, sdk, quantum applications, quantum software',
```

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_ContextMethods.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_ContextMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_DynamicMethods.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_DynamicMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_QSOAPlatform.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_QSOAPlatform.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_SecurityMethods.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_SecurityMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_QSOAPlatform/test_StaticMethods.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_QSOAPlatform/test_StaticMethods.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_circuit/test_CircuitAnnealing.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitAnnealing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1407,53 +1407,53 @@
             'To': linearExp.getTo(),
             'Iterator': linearExp.getIterator(),
             'Term1': linearExp.getTerm1(),
             'Term2': linearExp.getTerm2(),
             'Childs': linearExp.getChilds()
         }])
 
-    # SQUARED EXPRESSION expression SUMMATORYEXP
-    def test_SquaredExp_expression_SummatoryExp(self):
+    # SQUARED EXPRESSION expression SUMMATIONEXP
+    def test_SquaredExp_expression_SummationExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
-        summatory = circuit.SummatoryExp(1, 2, circuit.OffsetExp(1))
+        summation = circuit.SummationExp(1, 2, circuit.OffsetExp(1))
 
-        squaredExp = circuit.SquaredExp(summatory)
+        squaredExp = circuit.SquaredExp(summation)
         
         self.assertIsInstance(squaredExp, circuit.SquaredExp)
         self.assertEqual(squaredExp.getExpType(), 'SQUARED')
         self.assertEqual(squaredExp.getCoefficient(), '')
         self.assertEqual(squaredExp.getOffset(), '')
         self.assertEqual(squaredExp.getFrom(), '')
         self.assertEqual(squaredExp.getTo(), '')
         self.assertEqual(squaredExp.getIterator(), '')
         self.assertEqual(squaredExp.getTerm1(), {})
         self.assertEqual(squaredExp.getTerm2(), {})
         self.assertEqual(squaredExp.getChilds(), [{
-            'uiID': summatory.getUiID(),
-            'Type': summatory.getExpType(),
-            'Coefficient': summatory.getCoefficient(),
-            'Offset': summatory.getOffset(),
-            'From': summatory.getFrom(),
-            'To': summatory.getTo(),
-            'Iterator': summatory.getIterator(),
-            'Term1': summatory.getTerm1(),
-            'Term2': summatory.getTerm2(),
-            'Childs': summatory.getChilds()
+            'uiID': summation.getUiID(),
+            'Type': summation.getExpType(),
+            'Coefficient': summation.getCoefficient(),
+            'Offset': summation.getOffset(),
+            'From': summation.getFrom(),
+            'To': summation.getTo(),
+            'Iterator': summation.getIterator(),
+            'Term1': summation.getTerm1(),
+            'Term2': summation.getTerm2(),
+            'Childs': summation.getChilds()
         }])
 
-    # SQUARED EXPRESSION expression LIST OFFSETEXP, LINEAREXP, SUMMATORYEXP
-    def test_SquaredExp_expression_list_OffsetExp_LinearExp_SummatoryExp(self):
+    # SQUARED EXPRESSION expression LIST OFFSETEXP, LINEAREXP, SUMMATIONEXP
+    def test_SquaredExp_expression_list_OffsetExp_LinearExp_SummationExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
         linearExp = circuit.LinearExp((circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
-        summatory = circuit.SummatoryExp(1, 2, offsetExp)
+        summation = circuit.SummationExp(1, 2, offsetExp)
 
-        squaredExp = circuit.SquaredExp([offsetExp, linearExp, summatory])
+        squaredExp = circuit.SquaredExp([offsetExp, linearExp, summation])
         
         self.assertIsInstance(squaredExp, circuit.SquaredExp)
         self.assertEqual(squaredExp.getExpType(), 'SQUARED')
         self.assertEqual(squaredExp.getCoefficient(), '')
         self.assertEqual(squaredExp.getOffset(), '')
         self.assertEqual(squaredExp.getFrom(), '')
         self.assertEqual(squaredExp.getTo(), '')
@@ -1481,24 +1481,24 @@
             'To': linearExp.getTo(),
             'Iterator': linearExp.getIterator(),
             'Term1': linearExp.getTerm1(),
             'Term2': linearExp.getTerm2(),
             'Childs': linearExp.getChilds()
         },
         {
-            'uiID': summatory.getUiID(),
-            'Type': summatory.getExpType(),
-            'Coefficient': summatory.getCoefficient(),
-            'Offset': summatory.getOffset(),
-            'From': summatory.getFrom(),
-            'To': summatory.getTo(),
-            'Iterator': summatory.getIterator(),
-            'Term1': summatory.getTerm1(),
-            'Term2': summatory.getTerm2(),
-            'Childs': summatory.getChilds()
+            'uiID': summation.getUiID(),
+            'Type': summation.getExpType(),
+            'Coefficient': summation.getCoefficient(),
+            'Offset': summation.getOffset(),
+            'From': summation.getFrom(),
+            'To': summation.getTo(),
+            'Iterator': summation.getIterator(),
+            'Term1': summation.getTerm1(),
+            'Term2': summation.getTerm2(),
+            'Childs': summation.getChilds()
         }])
 
     # BAD ARGUMENT expression LIST
     def test_SquaredExp_badArgument_expression_list(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
 
@@ -1531,309 +1531,309 @@
             circuit.SquaredExp([offsetExp, 'expression'])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
-##################_____SUMMATORYEXP_____##################
-class Test_SummatoryExp(unittest.TestCase):
+##################_____SummationExp_____##################
+class Test_SummationExp(unittest.TestCase):
 
-    # SUMMATORY EXPRESSION fromValue INT
-    def test_SummatoryExp_fromValue_int(self):
+    # SUMMATION EXPRESSION fromValue INT
+    def test_SummationExp_fromValue_int(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
-        summatory = circuit.SummatoryExp(1, 2, offsetExp)
+        summation = circuit.SummationExp(1, 2, offsetExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION fromValue STRING
-    def test_SummatoryExp_fromValue_string(self):
+    # SUMMATION EXPRESSION fromValue STRING
+    def test_SummationExp_fromValue_string(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
-        summatory = circuit.SummatoryExp('fromValue', 2, offsetExp)
+        summation = circuit.SummationExp('fromValue', 2, offsetExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), 'fromValue')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), 'fromValue')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION toValue INT
-    def test_SummatoryExp_toValue_int(self):
+    # SUMMATION EXPRESSION toValue INT
+    def test_SummationExp_toValue_int(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
-        summatory = circuit.SummatoryExp(1, 2, offsetExp)
+        summation = circuit.SummationExp(1, 2, offsetExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION toValue STRING
-    def test_SummatoryExp_toValue_string(self):
+    # SUMMATION EXPRESSION toValue STRING
+    def test_SummationExp_toValue_string(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
-        summatory = circuit.SummatoryExp(1, 'toValue', offsetExp)
+        summation = circuit.SummationExp(1, 'toValue', offsetExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), 'toValue')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), 'toValue')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION expression OFFSETEXP
-    def test_SummatoryExp_expression_OffsetExp(self):
+    # SUMMATION EXPRESSION expression OFFSETEXP
+    def test_SummationExp_expression_OffsetExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
-        summatory = circuit.SummatoryExp(1, 2, offsetExp)
+        summation = circuit.SummationExp(1, 2, offsetExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION expression LINEAREXP
-    def test_SummatoryExp_expression_LinearExp(self):
+    # SUMMATION EXPRESSION expression LINEAREXP
+    def test_SummationExp_expression_LinearExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         linearExp = circuit.LinearExp((circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
 
-        summatory = circuit.SummatoryExp(1, 2, linearExp)
+        summation = circuit.SummationExp(1, 2, linearExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': linearExp.getUiID(),
             'Type': linearExp.getExpType(),
             'Coefficient': linearExp.getCoefficient(),
             'Offset': linearExp.getOffset(),
             'From': linearExp.getFrom(),
             'To': linearExp.getTo(),
             'Iterator': linearExp.getIterator(),
             'Term1': linearExp.getTerm1(),
             'Term2': linearExp.getTerm2(),
             'Childs': linearExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION expression QUADRATICEXP
-    def test_SummatoryExp_expression_QuadraticExp(self):
+    # SUMMATION EXPRESSION expression QUADRATICEXP
+    def test_SummationExp_expression_QuadraticExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         quadraticExp = circuit.QuadraticExp((variable:=circuit.Variable('Variable', circuit.Class('Class', 1)), 1), (variable, 2))
 
-        summatory = circuit.SummatoryExp(1, 2, quadraticExp)
+        summation = circuit.SummationExp(1, 2, quadraticExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': quadraticExp.getUiID(),
             'Type': quadraticExp.getExpType(),
             'Coefficient': quadraticExp.getCoefficient(),
             'Offset': quadraticExp.getOffset(),
             'From': quadraticExp.getFrom(),
             'To': quadraticExp.getTo(),
             'Iterator': quadraticExp.getIterator(),
             'Term1': quadraticExp.getTerm1(),
             'Term2': quadraticExp.getTerm2(),
             'Childs': quadraticExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION expression SQUAREDEXP
-    def test_SummatoryExp_expression_SquaredExp(self):
+    # SUMMATION EXPRESSION expression SQUAREDEXP
+    def test_SummationExp_expression_SquaredExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         squaredExp = circuit.SquaredExp(circuit.OffsetExp(1))
 
-        summatory = circuit.SummatoryExp(1, 2, squaredExp)
+        summation = circuit.SummationExp(1, 2, squaredExp)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': squaredExp.getUiID(),
             'Type': squaredExp.getExpType(),
             'Coefficient': squaredExp.getCoefficient(),
             'Offset': squaredExp.getOffset(),
             'From': squaredExp.getFrom(),
             'To': squaredExp.getTo(),
             'Iterator': squaredExp.getIterator(),
             'Term1': squaredExp.getTerm1(),
             'Term2': squaredExp.getTerm2(),
             'Childs': squaredExp.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION expression SUMMATORYEXP
-    def test_SummatoryExp_expression_SummatoryExp(self):
+    # SUMMATION EXPRESSION expression SUMMATIONEXP
+    def test_SummationExp_expression_SummationExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
-        summatory1 = circuit.SummatoryExp(1, 2, circuit.OffsetExp(1))
+        summation1 = circuit.SummationExp(1, 2, circuit.OffsetExp(1))
 
-        summatory = circuit.SummatoryExp(1, 2, summatory1)
+        summation = circuit.SummationExp(1, 2, summation1)
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
-            'uiID': summatory1.getUiID(),
-            'Type': summatory1.getExpType(),
-            'Coefficient': summatory1.getCoefficient(),
-            'Offset': summatory1.getOffset(),
-            'From': summatory1.getFrom(),
-            'To': summatory1.getTo(),
-            'Iterator': summatory1.getIterator(),
-            'Term1': summatory1.getTerm1(),
-            'Term2': summatory1.getTerm2(),
-            'Childs': summatory1.getChilds()
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
+            'uiID': summation1.getUiID(),
+            'Type': summation1.getExpType(),
+            'Coefficient': summation1.getCoefficient(),
+            'Offset': summation1.getOffset(),
+            'From': summation1.getFrom(),
+            'To': summation1.getTo(),
+            'Iterator': summation1.getIterator(),
+            'Term1': summation1.getTerm1(),
+            'Term2': summation1.getTerm2(),
+            'Childs': summation1.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION expression LIST OFFSETEXP, LINEAREXP, QUADRATICEXP, SQUAREDEXP, SUMMATORYEXP
-    def test_SummatoryExp_expression_list_OffsetExp_LinearExp_QuadraticExp_SquaredExp_SummatoryExp(self):
+    # SUMMATION EXPRESSION expression LIST OFFSETEXP, LINEAREXP, QUADRATICEXP, SQUAREDEXP, SUMMATIONEXP
+    def test_SummationExp_expression_list_OffsetExp_LinearExp_QuadraticExp_SquaredExp_SummationExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
         linearExp = circuit.LinearExp((variable:=circuit.Variable('Variable', circuit.Class('Class', 1)), 1))
         quadraticExp = circuit.QuadraticExp((variable, 1), (variable, 2))
         squaredExp = circuit.SquaredExp(offsetExp)
-        summatory1 = circuit.SummatoryExp(1, 2, offsetExp)
+        summation1 = circuit.SummationExp(1, 2, offsetExp)
 
-        summatory = circuit.SummatoryExp(1, 2, [offsetExp, linearExp, quadraticExp, squaredExp, summatory1])
+        summation = circuit.SummationExp(1, 2, [offsetExp, linearExp, quadraticExp, squaredExp, summation1])
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'i')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'i')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
@@ -1874,127 +1874,127 @@
             'To': squaredExp.getTo(),
             'Iterator': squaredExp.getIterator(),
             'Term1': squaredExp.getTerm1(),
             'Term2': squaredExp.getTerm2(),
             'Childs': squaredExp.getChilds()
         },
         {
-            'uiID': summatory1.getUiID(),
-            'Type': summatory1.getExpType(),
-            'Coefficient': summatory1.getCoefficient(),
-            'Offset': summatory1.getOffset(),
-            'From': summatory1.getFrom(),
-            'To': summatory1.getTo(),
-            'Iterator': summatory1.getIterator(),
-            'Term1': summatory1.getTerm1(),
-            'Term2': summatory1.getTerm2(),
-            'Childs': summatory1.getChilds()
+            'uiID': summation1.getUiID(),
+            'Type': summation1.getExpType(),
+            'Coefficient': summation1.getCoefficient(),
+            'Offset': summation1.getOffset(),
+            'From': summation1.getFrom(),
+            'To': summation1.getTo(),
+            'Iterator': summation1.getIterator(),
+            'Term1': summation1.getTerm1(),
+            'Term2': summation1.getTerm2(),
+            'Childs': summation1.getChilds()
         }])
 
-    # SUMMATORY EXPRESSION iterator
-    def test_SummatoryExp_iterator(self):
+    # SUMMATION EXPRESSION iterator
+    def test_SummationExp_iterator(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
-        summatory = circuit.SummatoryExp(1, 2, offsetExp, iterator='x')
+        summation = circuit.SummationExp(1, 2, offsetExp, iterator='x')
         
-        self.assertIsInstance(summatory, circuit.SummatoryExp)
-        self.assertEqual(summatory.getExpType(), 'SUMMATORY')
-        self.assertEqual(summatory.getCoefficient(), '')
-        self.assertEqual(summatory.getOffset(), '')
-        self.assertEqual(summatory.getFrom(), '1')
-        self.assertEqual(summatory.getTo(), '2')
-        self.assertEqual(summatory.getIterator(), 'x')
-        self.assertEqual(summatory.getTerm1(), {})
-        self.assertEqual(summatory.getTerm2(), {})
-        self.assertEqual(summatory.getChilds(), [{
+        self.assertIsInstance(summation, circuit.SummationExp)
+        self.assertEqual(summation.getExpType(), 'SUMMATORY')
+        self.assertEqual(summation.getCoefficient(), '')
+        self.assertEqual(summation.getOffset(), '')
+        self.assertEqual(summation.getFrom(), '1')
+        self.assertEqual(summation.getTo(), '2')
+        self.assertEqual(summation.getIterator(), 'x')
+        self.assertEqual(summation.getTerm1(), {})
+        self.assertEqual(summation.getTerm2(), {})
+        self.assertEqual(summation.getChilds(), [{
             'uiID': offsetExp.getUiID(),
             'Type': offsetExp.getExpType(),
             'Coefficient': offsetExp.getCoefficient(),
             'Offset': offsetExp.getOffset(),
             'From': offsetExp.getFrom(),
             'To': offsetExp.getTo(),
             'Iterator': offsetExp.getIterator(),
             'Term1': offsetExp.getTerm1(),
             'Term2': offsetExp.getTerm2(),
             'Childs': offsetExp.getChilds()
         }])
 
     # BAD ARGUMENT expression LIST
-    def test_SummatoryExp_badArgument_expression_list(self):
+    def test_SummationExp_badArgument_expression_list(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
 
         try:
-            circuit.SummatoryExp(1, 2, [])
+            circuit.SummationExp(1, 2, [])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, ValueError)
 
     # BAD ARGUMENT TYPE fromValue
-    def test_SummatoryExp_badArgumentType_fromValue(self):
+    def test_SummationExp_badArgumentType_fromValue(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
-            circuit.SummatoryExp(True, 2, offsetExp)
+            circuit.SummationExp(True, 2, offsetExp)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE toValue
-    def test_SummatoryExp_badArgumentType_toValue(self):
+    def test_SummationExp_badArgumentType_toValue(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
-            circuit.SummatoryExp(1, True, offsetExp)
+            circuit.SummationExp(1, True, offsetExp)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE expression STRING
-    def test_SummatoryExp_badArgumentType_expression_string(self):
+    def test_SummationExp_badArgumentType_expression_string(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
 
         try:
-            circuit.SummatoryExp(1, 2, 'expression')
+            circuit.SummationExp(1, 2, 'expression')
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE expression LIST
-    def test_SummatoryExp_badArgumentType_expression_list(self):
+    def test_SummationExp_badArgumentType_expression_list(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
-            circuit.SummatoryExp(1, 2, [offsetExp, 1])
+            circuit.SummationExp(1, 2, [offsetExp, 1])
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
     # BAD ARGUMENT TYPE iterator
-    def test_SummatoryExp_badArgumentType_iterator(self):
+    def test_SummationExp_badArgumentType_iterator(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         offsetExp = circuit.OffsetExp(1)
 
         try:
-            circuit.SummatoryExp(1, 2, offsetExp, iterator=99)
+            circuit.SummationExp(1, 2, offsetExp, iterator=99)
             raise Exception
 
         except Exception as e:
             self.assertIsInstance(e, TypeError)
 
 
 ##################_____ADD PARAMETER_____##################
@@ -2442,38 +2442,38 @@
                                         'Childs': [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}]}])
 
     # ADD EXPRESSION expression SQUAREDEXP
     def test_addExpression_expression_SquaredExp(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
-        summatory = circuit.SummatoryExp(1, 2, circuit.OffsetExp(1))
+        summation = circuit.SummationExp(1, 2, circuit.OffsetExp(1))
         
-        ruleAdded = rule.addExpression(summatory)
+        ruleAdded = rule.addExpression(summation)
 
         expressions = rule.getExpressions()
 
         self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'SUMMATORY', 'Coefficient': '', 'Offset': '', 'From': '1', 'To': '2', 'Iterator': 'i', 'Term1': {}, 'Term2': {},
                                         'Childs': [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []}]}])
 
-    # ADD EXPRESSION LIST OFFSETEXP, LINEAREXP, QUADRATICEXP, SQUAREDEXP, SUMMATORYEXP
+    # ADD EXPRESSION LIST OFFSETEXP, LINEAREXP, QUADRATICEXP, SQUAREDEXP, SUMMATIONEXP
     def test_addExpression_list(self):
         qsoa = QSOAPlatform()
         circuit = qsoa.CircuitAnnealing()
         rule = circuit.Rule('Rule', 1)
         offsetExp = circuit.OffsetExp(1)
         linearExp = circuit.LinearExp((variable:=circuit.Variable('Variable', cls:=circuit.Class('Class', 1)), 1))
         quadraticExp = circuit.QuadraticExp((variable, 1), (variable, 2))
         squaredExp = circuit.SquaredExp(offsetExp)
-        summatory = circuit.SummatoryExp(1, 2, offsetExp)
+        summation = circuit.SummationExp(1, 2, offsetExp)
 
-        ruleAdded = rule.addExpression([offsetExp, linearExp, quadraticExp, squaredExp, summatory])
+        ruleAdded = rule.addExpression([offsetExp, linearExp, quadraticExp, squaredExp, summation])
 
         expressions = rule.getExpressions()
         self.assertIsInstance(ruleAdded, qsoa.CircuitAnnealing.Rule)
         self.assertIsInstance(expressions, list)
         removeUiID(expressions) # remove random uiID to validate behaviour
         self.assertEqual(expressions, [{'Type': 'OFFSET', 'Coefficient': '', 'Offset': '1', 'From': '', 'To': '', 'Iterator': '', 'Term1': {}, 'Term2': {}, 'Childs': []},
                                        {'Type': 'LINEAR', 'Coefficient': '', 'Offset': '', 'From': '', 'To': '', 'Iterator': '',
```

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_circuit/test_CircuitFlow.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitFlow.py`

 * *Files identical despite different names*

### Comparing `QuantumPathQSOAPySDK-1.5/test/test_circuit/test_CircuitGates.py` & `QuantumPathQSOAPySDK-1.5.1/test/test_circuit/test_CircuitGates.py`

 * *Files identical despite different names*

