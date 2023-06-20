# Comparing `tmp/DIRAC-8.1.0a8.tar.gz` & `tmp/DIRAC-8.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DIRAC-8.1.0a8.tar", last modified: Tue Feb 21 07:56:23 2023, max compression
+gzip compressed data, was "DIRAC-8.1.0a9.tar", last modified: Tue Feb 28 16:16:58 2023, max compression
```

## Comparing `DIRAC-8.1.0a8.tar` & `DIRAC-8.1.0a9.tar`

### file list

```diff
@@ -1,1519 +1,1518 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.802815 DIRAC-8.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-02-21 07:56:23.802815 DIRAC-8.1.0a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (123)    41418 2023-02-21 07:55:50.000000 DIRAC-8.1.0a8/dirac.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (123)    24539 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/integration_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)   403475 2023-02-21 07:56:14.000000 DIRAC-8.1.0a8/release.notes
--rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/releases.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    18988 2023-02-21 07:56:23.802815 DIRAC-8.1.0a8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.614813 DIRAC-8.1.0a8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.638814 DIRAC-8.1.0a8/src/DIRAC/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.638814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.638814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/NetworkAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.638814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/test/Test_NetworkAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.638814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/AccountingCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/DataStoreClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/ReportCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/ReportsClient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/BaseAccountingType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/DataOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/Job.py
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/Pilot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/PilotSubmission.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/StorageOccupancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/WMSHistory.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    68727 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/AccountingDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/AccountingDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/MultiAccountingDB.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/test/Test_AccountingDB.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Service/DataStoreHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Service/ReportGeneratorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/
--rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/DBUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/MainReporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/
--rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/BaseReporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/DataOperationPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/JobPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/NetworkPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/PilotPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/PilotSubmissionPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/StorageOccupancyPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/WMSHistoryPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Policies/
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Policies/FilterExecutor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Policies/JobPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/scripts/dirac_accounting_decode_fileid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/scripts/dirac_admin_accounting_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.642814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/Bdii2CSAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/GOCDB2CSAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    30084 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/RucioSynchronizerAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/VOMS2CSAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/test/
--rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/test/Test_Bdii2CS.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)    37024 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/CSAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/CSCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/CSShellCLI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      524 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/ConfigurationClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/ConfigurationData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/CSGlobals.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Local.py
--rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Operations.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Path.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    15785 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/ResourcesDefaults.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31015 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/LocalConfiguration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10795 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/PathFinder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/CERNLDAPSyncPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/DummySyncPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    26750 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/VOMS2CSSynchronizer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.646814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/test/Test_LocalConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/test/Test_PathFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.650814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Service/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4036 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Service/ConfigurationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Service/TornadoConfigurationHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Service/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.650814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/
--rwxr-xr-x   0 runner    (1001) docker     (123)    10905 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ConfigurationClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14919 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ConfigurationData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10537 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/Modificator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3922 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/Refresher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/RefresherBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1895 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ServiceInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceTornado.py
--rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/TornadoRefresher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.650814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10705 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1455 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_shifter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3710 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_site.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7578 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_check_config_options.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4185 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_sort_cs_sites.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3051 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_voms_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_dump_local_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.650814 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/test/Test_agentOptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.650814 DIRAC-8.1.0a8/src/DIRAC/Core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.654814 DIRAC-8.1.0a8/src/DIRAC/Core/Base/
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/API.py
--rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/AgentModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/AgentReactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/CLI.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/Client.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/DB.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/DIRACDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/ElasticDB.py
--rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/ExecutorMindHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/ExecutorModule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/ExecutorReactor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/SQLAlchemyDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8143 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/Script.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.654814 DIRAC-8.1.0a8/src/DIRAC/Core/Base/private/
--rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/private/ModuleLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Base/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.654814 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13459 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/AuthManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6007 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/MessageClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3816 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/RPCClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24051 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/RequestHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/ServiceReactor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/ThreadConfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7620 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/TransferClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.654814 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/
--rwxr-xr-x   0 runner    (1001) docker     (123)    28524 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/BaseClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14383 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/FileHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/GatewayService.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/InnerRPCClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/LockManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/MessageBroker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/MessageFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      448 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    27235 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3824 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/ServiceConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/TransportPool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13373 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/BaseTransport.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    23469 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/M2SSLTransport.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4712 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/PlainTransport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSL/
--rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSL/FakeSocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSL/M2Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSL/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4135 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSLTransport.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/test/Test_SSLTransport.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/test/proxy.pem
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/DISET/test/Test_AuthManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/LCG/
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/LCG/GGUSTicketsClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/LCG/GOCDBClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/LCG/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/LCG/test/
--rw-r--r--   0 runner    (1001) docker     (123)    32871 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/LCG/test/Test_LCG.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/Locations.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/Properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/ProxyFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/ProxyInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/VOMS.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/VOMSService.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.658814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509CRL.py
--rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509Certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    38098 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509Request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/asn1_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/Test_X509Certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/Test_X509Chain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/Test_X509Request.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.618813 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/b236481c.0
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/ca.cert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/ca.key.pem
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/crlnumber
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/index.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/index.txt.attr
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/index.txt.attr.old
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/index.txt.old
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/1000.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/1001.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/1002.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/openssl_config_ca.cnf
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/serial
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/serial.old
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/hostcert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/hostkey.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/hostkey.pem.bak
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/openssl_config_host.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/request.csr.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/key/
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/key/encrypted_key_pass_0000.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/openssl_config_user.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/request.csr.pem
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/usercert.pem
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/userkey.pem
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/voms/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/voms/README
--rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/voms/proxy.pem
--rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/x509TestUtilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.662814 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.666814 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/ClientSelector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/TornadoClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.666814 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/private/
--rw-r--r--   0 runner    (1001) docker     (123)    28384 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/private/TornadoBaseClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.666814 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/
--rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/HandlerManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/TornadoREST.py
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/TornadoServer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/TornadoService.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.666814 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/private/
--rw-r--r--   0 runner    (1001) docker     (123)    42720 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/private/BaseRequestHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/private/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.666814 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/scripts/tornado_start_CS.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/scripts/tornado_start_all.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.674814 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3321 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Adler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.674814 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ClassAd/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9584 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ClassAd/ClassAdLight.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ClassAd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/CountryMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DAG.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15565 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DEncode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DErrno.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DIRACSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Devloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DictCache.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DirectoryExplorer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21207 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ElasticSearchDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/EventDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    28893 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ExecutorDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Extensions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7551 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/File.py
--rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Glue2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.674814 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/BarGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/CurveGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Dwatermark.png
--rw-r--r--   0 runner    (1001) docker     (123)    13486 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    19352 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/GraphData.py
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/GraphUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Legend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/LineGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Palette.py
--rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/PieGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/PlotBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/QualityMapGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/JDL.py
--rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/JEncode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3684 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/List.py
--rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/LockRing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/MJF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Mail.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/MixedEncode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62483 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/MySQL.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Network.py
--rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ObjectLoader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3958 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Os.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7765 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Pfn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Platform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.674814 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/DataCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/FileCoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/Plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/TypeLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/PrettyPrint.py
--rw-r--r--   0 runner    (1001) docker     (123)    35966 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ProcessPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/PromptUser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8683 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ReturnValues.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ServerUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Shifter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/SiteSEMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11484 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ThreadPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ThreadSafe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ThreadScheduler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9001 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/TimeUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.678814 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/ProcessesCreator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Adler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_DAG.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Dictionaries.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ExecutorDispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_File.py
--rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_List.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Network.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ObjectLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Pfn.py
--rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ProcessPool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ReturnValues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Subprocess.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Time.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_entrypoints.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.678814 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/
--rwxr-xr-x   0 runner    (1001) docker     (123)    12631 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Module.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    26903 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Parameter.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    20689 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Step.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Utility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.678814 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/WFEditor/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/WFEditor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18115 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5245 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/WorkflowReader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.678814 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    18060 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/JobSamples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/ModulesSamples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/WFSamples.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/step_g.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.682814 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1740 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_cert_convert.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28789 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_configure.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1818 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_generate_cas.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_generate_crls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3736 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1241 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_install_db.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_install_web_portal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5594 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_platform.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1689 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_setup_site.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5457 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/scripts/install_full.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.682814 DIRAC-8.1.0a8/src/DIRAC/Core/test/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Core/test/Test_API.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.682814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.682814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)    24139 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/FTS3Agent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.682814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ArchiveFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/CheckMigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/DMSRequestOperationsBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/MoveReplica.py
--rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PhysicalRemoval.py
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PutAndRegister.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReTransfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterReplica.py
--rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveReplica.py
--rw-r--r--   0 runner    (1001) docker     (123)    26999 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReplicateAndRegister.py
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/StagingCallback.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.682814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ArchiveFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_CheckMigration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_RequestOperations.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.686814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.686814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/AbstractFileSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/DirectoryCompletion.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/ConsistencyInspector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/DataIntegrityClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    81684 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/DataManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/DirectoryListing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3Client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3File.py
--rw-r--r--   0 runner    (1001) docker     (123)    33837 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3Job.py
--rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FailoverTransfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    80127 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FileCatalogClientCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/MetaQuery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/S3GatewayClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.686814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/Test_FTS3Objects.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/mock_DM.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/new_dir_completion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/DataIntegrityDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/DataIntegrityDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FTS3DB.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FTS3DB.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/
--rw-r--r--   0 runner    (1001) docker     (123)    31121 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/DatasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/
--rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryClosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryFlatTree.py
--rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryLevelTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryNodeTree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectorySimpleTree.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49195 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryTreeBase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    37600 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/DirectoryMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/MultiVODirectoryMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/
--rwxr-xr-x   0 runner    (1001) docker     (123)    35622 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManager.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54588 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15554 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerFlat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    33910 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerPs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/
--rw-r--r--   0 runner    (1001) docker     (123)    27746 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/FileMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/MultiVOFileMetadata.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.690814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerDB.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManagerWithDelete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/FullSecurityManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/NoSecurityManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/SecurityManagerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/VOMSSecurityManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/test/
--rw-r--r--   0 runner    (1001) docker     (123)    55701 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/test/Test_VOMSSecurityManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerCS.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerDB.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/test/Test_DataManagement_FileCatalogComponents.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43086 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9007 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)    61258 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogWithFkAndPsDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/test/Test_FTS3DB.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/DataIntegrityHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/FTS3ManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    25949 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/FileCatalogHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/S3GatewayHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18963 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/StorageElementHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/TornadoDataIntegrityHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/TornadoFTS3ManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/TornadoFileCatalogHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/TornadoS3GatewayHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/test/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/test/Test_Service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/DMSHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/ResolveSE.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/test/Test_resolveSE.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.694814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.698814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/DefaultFTS3Plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.698814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/test/Test_DefaultFTS3Plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/HttpStorageAccessHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.698814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/test/Test_FTS3Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7413 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_admin_allow_se.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9938 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_admin_ban_se.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_admin_user_quota.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3442 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2368 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_catalog_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_change_replica_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_clean_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_archive_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_moving_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_removal_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_data_size.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18000 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_directory_sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2005 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_filecatalog_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_find_lfns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3948 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_move_replica_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9097 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_protocol_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2700 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_put_and_register_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2236 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_replicas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1883 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replica_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4524 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replicate_and_register_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_resolve_guid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2344 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_set_replica_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_show_se_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5779 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_lfns.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_quota.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/API/
--rw-r--r--   0 runner    (1001) docker     (123)    21867 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/API/AuthHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/API/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/ComponentSupervisionAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/ProxyRenewalAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/test/
--rw-r--r--   0 runner    (1001) docker     (123)    33839 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/test/Test_ComponentSupervisionAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/BundleDeliveryClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    99348 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ComponentInstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ComponentMonitoringClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/NotificationClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ProxyGeneration.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27110 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ProxyManagerClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ProxyUpload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SecurityLogClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    52784 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClientCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SystemAdministratorIntegrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/TokenManagerClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/UserProfileClient.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.702814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/test/Test_ComponentInstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6387 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.706814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/AuthDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/AuthDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)    43144 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/InstalledComponentsDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/InstalledComponentsDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)    35430 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/NotificationDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/NotificationDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)    54769 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/ProxyDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/ProxyDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/TokenDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/TokenDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)    21493 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/UserProfileDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/UserProfileDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.706814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/BundleDeliveryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/ComponentMonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/NotificationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/ProxyManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/SecurityLoggingHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/SystemAdministratorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13158 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TokenManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoBundleDeliveryHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoComponentMonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoNotificationHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoProxyManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoUserProfileManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/UserProfileManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.706814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Utilities/MonitoringUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.706814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/SecurityFileLog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.706814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)    23061 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/AuthServer.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.710814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/AuthorizationCode.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/DeviceFlow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/RefreshToken.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/RevokeToken.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.710814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.710814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.710814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/BaseFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/ColoredBaseFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/MicrosecondJsonFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.710814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/MessageQueueHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/LogLevels.py
--rw-r--r--   0 runner    (1001) docker     (123)    21874 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/LoggingRoot.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.710814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/TestLogUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LogLevels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LoggingRoot_ConfigForExternalLibs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_CreationLogRecord.py
--rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_FormatOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_GetSubLogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Levels.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.714814 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_CAs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5344 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_proxy_upload.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_sysadmin_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9454 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_instance.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_pilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2681 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_users_with_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4424 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_install_component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_install_tornado_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_logout.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7966 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_populate_component_db.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5010 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_destroy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_get_uploaded_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5864 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10373 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_init.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_restart_component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1289 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_start_component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1658 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_status_component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_stop_component.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_sys_sendmail.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_uninstall_component.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.714814 DIRAC-8.1.0a8/src/DIRAC/Interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.714814 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/
--rwxr-xr-x   0 runner    (1001) docker     (123)    93582 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/Dirac.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31377 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/DiracAdmin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50504 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/Job.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.714814 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/Test_DIRAC.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/Test_JobAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/testWF.jdl
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/testWF.xml
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/testWFSIO.jdl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.718814 DIRAC-8.1.0a8/src/DIRAC/Interfaces/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    21688 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/Utilities/DCommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/Utilities/DConfigCache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.726814 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1323 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dcd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1732 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dchgrp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1735 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dchmod.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1707 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dchown.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2652 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dconfig.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dfind.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3437 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dget.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1247 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dgetenv.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2126 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dinit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3305 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_add_host.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_add_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_allow_site.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_ban_site.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_ce_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_delete_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_banned_sites.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilot_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3037 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4525 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2191 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_logging_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_site_mask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_list_hosts.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_list_users.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2271 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_modify_user.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_pilot_summary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_reset_job.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_service_ports.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_set_site_protocols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_site_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_site_mask_logging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1825 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_sync_users_from_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_get_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_accessURL.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2247 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_replicas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_accessURL.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_metadata.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1971 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_replicate_lfn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_framework_ping_service.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_framework_self_ping.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_utils_file_adler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_utils_file_md5.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_get_normalized_queue_length.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_get_queue_normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2107 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_attributes.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_delete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_input.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1937 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_jdl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3708 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2838 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_logging_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_peek.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_reschedule.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2273 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_jobs_select_output_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4153 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_select_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2507 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dkill.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1483 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dlogging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dls.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5107 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dmeta.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1298 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dmkdir.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5834 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/doutput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4465 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dput.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      445 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dpwd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3007 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/drepl.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1258 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dreplicas.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3806 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/drm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/drmdir.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7211 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dstat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15436 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dsub.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.726814 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.726814 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/DataOperationSender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/MonitoringClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/MonitoringReporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/ServerUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.726814 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/AgentMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/BaseType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/DataOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/FailedDataOperation.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/PilotSubmissionMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/PilotsHistory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/RMSMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/ServiceMonitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/WMSHistory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.726814 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/MonitoringDB.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/test/Test_monitoringdb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Service/MonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Service/TornadoMonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/DBUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/MainReporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/
--rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/BasePlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/RMSMonitoringPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/WMSHistoryPlotter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Client/ProductionClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Client/ProductionStep.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/DB/ProductionDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/DB/ProductionDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Service/ProductionManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Service/TornadoProductionManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.730815 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/ProdTransManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/ProdValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_add_trans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      721 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_clean.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_complete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_delete.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1259 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_all.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_description.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3060 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_trans.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_start.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_stop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/CleanReqDBAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestExecutingAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/
--rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/ForwardDISET.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/test/ForwardDISETTests.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/File.py
--rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/Operation.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27746 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/ReqClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/Request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/Test_File.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/Test_Operation.py
--rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/Test_Request.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/
--rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/ReqDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)    35114 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/RequestDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/test/RMSTestScenari.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/test/Test_RequestDB.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.734815 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/
--rwxr-xr-x   0 runner    (1001) docker     (123)    13798 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/ReqManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9220 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/ReqProxyHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/TornadoReqManagerHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/test/OperationHandlerBaseTests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/JSONUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/OperationHandlerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/RequestTask.py
--rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/RequestValidator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/Test_OperationHandlerBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/Test_RequestTask.py
--rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/Test_RequestValidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_list_req_cache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1246 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_reqdb_summary.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11656 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/CacheFeederAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/ElementInspectorAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/EmailAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/RucioRSSAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/SiteInspectorAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/SummarizeLogsAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/TokenAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.738814 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ElementInspectorAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ResourceStatusSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_SiteInspectorAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.742815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/PublisherClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    33305 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/ResourceManagementClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/ResourceStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/ResourceStatusClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/SiteStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.742815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/Command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/CommandCaller.py
--rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/DowntimeCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/FreeDiskSpaceCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/GGUSTicketsCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/GOCDBSyncCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/JobCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/MacroCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/PilotCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/PropagationCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/TransferCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.742815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/test/
--rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBStatusCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBSyncCommand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.742815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    19205 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/ResourceManagementDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/ResourceManagementDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/ResourceStatusDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/ResourceStatusDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.746815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysActivePolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysBannedPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysDegradedPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysProbingPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/CEAvailabilityPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/Configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/DowntimePolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/FreeDiskSpacePolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/GGUSTicketsPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobDoneRatioPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobEfficiencyPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobRunningMatchedRatioPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobRunningWaitingRatioPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/PilotEfficiencyPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/PropagationPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.746815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_AlwaysActivePolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_CEAvailabilityPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_DTPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_FreeDiskSpacePolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_GGUSTicketsPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobDoneRatioPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobEfficiencyPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningMatchedRatioPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningWaitingRatioPolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_PilotEfficiencyPolicy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.746815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.746815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/BaseAction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogPolicyResultAction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogStatusAction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/SlackAction.py
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PDP.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PEP.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyCaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.746815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/test/Test_PolicySystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.750815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/PublisherHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/ResourceManagementHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/ResourceStatusHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/TornadoPublisherHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/TornadoResourceManagementHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/TornadoResourceStatusHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.750815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/CSHelpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/InfoGetter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/RSSCache.py
--rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/RSSCacheNoThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/RssConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/Synchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.750815 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4572 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_list_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13824 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_db.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9929 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_dtcache.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7942 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_status.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6167 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_token.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7616 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.750815 DIRAC-8.1.0a8/src/DIRAC/Resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.750815 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.754815 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/DummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/FCConditionBasePlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/FilenamePlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/ProxyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.754815 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_FilenamePlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_ProxyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FCConditionParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    25899 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalogClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalogClientBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalogFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11778 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/PoolXMLCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/PoolXMLFile.py
--rw-r--r--   0 runner    (1001) docker     (123)    30541 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/RucioFileCatalogClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/TSCatalogClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/Utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.754815 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/Test_FCConditionParser.py
--rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/Test_FileCatalog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/mock_FC.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.754815 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/
--rwxr-xr-x   0 runner    (1001) docker     (123)     9619 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ARC6ComputingElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29149 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ARCComputingElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30812 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/AREXComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BOINCComputingElement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.758815 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/
--rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/Condor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/GE.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/Host.py
--rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/LSF.py
--rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/OAR.py
--rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/SLURM.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.758815 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/HTCondorResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/LSFResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/MJFResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/PBSResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/ResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SGEResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SLURMResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/TimeLeft.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.758815 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_LSFResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_PBSResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_SGEResourceUsage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_TimeLeft.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/Torque.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/executeBatch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.758815 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/test/Test_SLURM.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/CREAMComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/CloudComputingElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21965 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ComputingElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ComputingElementFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    23530 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/HTCondorCEComputingElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4750 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/InProcessComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/LocalComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/PilotBundle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/PoolComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SSHBatchComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)    32135 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SSHComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SingularityComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SudoComputingElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/cloudinit.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.758815 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6811 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_HTCondorCEComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_InProcessComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_PoolComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_SSHComputingElement.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.762815 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/CheckInIdProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/IAMIdProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/IdProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/IdProviderFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/OAuth2IdProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.762815 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/AbstractBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/ElasticSearchBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/FileBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/MessageQueueBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/StderrBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/StdoutBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/StdoutJsonBackend.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.762815 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/ModuleFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/PatternFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/SensitiveDataFilter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.762815 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/test/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/test/Test_LogFilter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.762815 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQCommunication.py
--rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQConnectionManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQConnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQConsumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQProducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.762815 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/Simple/
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/Simple/StompInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/Simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/StompMQConnector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.766815 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/
--rw-r--r--   0 runner    (1001) docker     (123)    32690 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQConnectionManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQConsumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQProducer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQ_Utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.766815 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/
--rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/DIRACCAProxyProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/PUSPProxyProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/ProxyProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/ProxyProviderFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.766815 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/test/Test_DIRACCAProxyProvider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/test/Test_ProxyProviderFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.766815 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/CTAStorage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19817 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/DIPStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/EchoStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/FCOnlyStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    22075 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/FileStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_GSIFTPStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_HTTPSStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_SRM2Storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    58784 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_StorageBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_XROOTStorage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.766815 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/BDIIOccupancy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingHTTPJson.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingJson.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42741 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/RFIOStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    28080 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/S3Storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16350 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/StorageBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61603 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/StorageElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19435 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/StorageFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/Utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)    32777 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/FIXME_Test_RFIOPlugIn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    39829 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/FIXME_Test_StorageElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    36441 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/FIXME_Test_StoragePlugIn.py
--rw-r--r--   0 runner    (1001) docker     (123)    18987 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_FilePlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_GFAL2_XROOTStorage.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_StorageElement.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22448 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_StorageFactory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/test_utilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/Resources/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/scripts/dirac_resource_get_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Resources/scripts/dirac_resource_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7862 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/RequestFinalizationAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11601 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/RequestPreparationAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9727 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/StageMonitorAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/StageRequestAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/StorageManagerClient.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/test/Test_Client_StorageManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    63907 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.770815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Service/
--rwxr-xr-x   0 runner    (1001) docker     (123)    15033 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Service/StorageManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Service/TornadoStorageManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.774815 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4379 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5626 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_jobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_request.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7357 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_requests.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3131 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_show_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_stage_files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.774815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.774815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/
--rw-r--r--   0 runner    (1001) docker     (123)    26982 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/DataRecoveryAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/InputDataAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5266 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/MCExtensionAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.774815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/RequestOperations/
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/RequestOperations/SetFileStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/RequestOperations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/RequestTaskAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TaskManagerAgentBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationAgentsUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    31929 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10108 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1770 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.774815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/test/
--rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/test/Test_Agent_TransformationSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/test/Test_Plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.778815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.778815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/BodyPlugin/
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/BodyPlugin/BaseBody.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/BodyPlugin/DummyBody.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/BodyPlugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/FileReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/PluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/RequestTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TaskManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TaskManagerPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    28485 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/Transformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationCLI.py
--rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationFilesStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    28710 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/WorkflowTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.778815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_RequestTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_TaskManagerPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationClient.py
--rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_WorkflowTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.778815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/DB/
--rwxr-xr-x   0 runner    (1001) docker     (123)    78503 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/DB/TransformationDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6835 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/DB/TransformationDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.778815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Service/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    30589 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Service/TransformationManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.778815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/JobInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/ReplicationCLIParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/ReplicationTransformation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/ScriptUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/TransformationInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4793 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1553 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_clean.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_cli.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_get_files.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_information.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1854 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_recover_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_remove_output.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_replication.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_update_derived.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_verify_outputdata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/
--rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_DRA.py
--rw-r--r--   0 runner    (1001) docker     (123)    26685 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_JobInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_TransformationInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_replicationTransformation.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/Workflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/FailoverRequest.py
--rw-r--r--   0 runner    (1001) docker     (123)    23090 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/ModuleBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/Script.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/UploadOutputs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/test/
--rw-r--r--   0 runner    (1001) docker     (123)    32354 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/test/Test_Modules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/test/Test_Utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/Workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.782815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.786815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/
--rwxr-xr-x   0 runner    (1001) docker     (123)    37109 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/JobAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/JobCleaningAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13572 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/OptimizerModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/PilotStatusAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/PilotSyncAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/PushJobAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)    60374 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25262 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/StalledJobAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/StatesAccountingAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/TaskQueuesAgent.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.786815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobCleaningAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PilotStatusAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PushJobAgent.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_SiteDirector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_StalledJobAgent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/CPUNormalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
--rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/InputDataByProtocol.py
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/InputDataResolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobManagerClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobMinorStatus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2205 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobMonitoringClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobReport.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/
--rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/CachedJobState.py
--rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobManifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobState.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobStateUpdateClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/Limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/Matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/MatcherClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/PilotManagerClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/PilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/PoolXMLSlice.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11811 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/SandboxStoreClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/ServerUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/WMSAdministratorClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9256 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/WMSClient.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_DownloadInputData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_WorkloadManagementSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/Test_JobReport.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/
--rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/ElasticJobParametersDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    76374 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6817 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1869 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)    49685 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.sql
--rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/SandboxMetadataDB.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/SandboxMetadataDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)    57007 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.sql
--rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/tests/Test_JobDB.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/Base/
--rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/Base/OptimizerExecutor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/Base/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18049 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/InputData.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2511 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/JobPath.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6301 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/JobSanity.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27868 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/JobScheduling.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.790815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/test/
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/test/Test_Executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.794815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/
--rwxr-xr-x   0 runner    (1001) docker     (123)    70468 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapperTemplate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    42540 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/Watchdog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.794815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_JobWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_Watchdog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/jobDescription.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)        7 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/script-OK.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       10 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/script-RESC.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)        9 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/script.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.794815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/
--rwxr-xr-x   0 runner    (1001) docker     (123)    25264 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobManagerHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22130 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobMonitoringHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8237 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobPolicy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11062 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobStateUpdateHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/MatcherHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/OptimizationMindHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/PilotManagerHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    21484 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/SandboxStoreHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobManagerHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobMonitoringHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobStateUpdateHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/TornadoWMSAdministratorHandler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9073 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/WMSAdministratorHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/WMSUtilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.798815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/JobParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/JobStatusUtility.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/ParametricJob.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/PilotCStoJSONSynchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/PilotWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/QueueUtilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/RemoteRunner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.798815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_JobStatusUtility.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_ParametricJob.py
--rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotCStoJSONSynchronizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotWrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_QueueUtilities.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.798815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/ConfigHelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/SharesCorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.798815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseCorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseHistoryCorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/MonitoringHistoryCorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/WMSHistoryCorrector.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.798815 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_kill_pilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3248 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_show_task_queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_sync_pilot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_jobexec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3106 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_cpu_normalization.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_queue_cpu_time.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7506 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1476 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_match.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3233 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_pilot_job_info.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11458 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.798815 DIRAC-8.1.0a8/src/DIRAC/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.802815 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/Accounting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/IntegrationTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/ProcessesCreator_withChildren.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/WMS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/assertingUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/mpTest-flexible.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/mpTest.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/testJobDefinitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.634814 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.802815 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Integration/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Integration/exe-script.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Integration/helloWorld.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.802815 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Regression/
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Regression/helloWorld.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5310 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Regression/helloWorld.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 07:55:51.000000 DIRAC-8.1.0a8/src/DIRAC/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 07:56:23.638814 DIRAC-8.1.0a8/src/DIRAC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-02-21 07:56:23.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    72053 2023-02-21 07:56:23.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 07:56:23.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-02-21 07:56:23.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 07:56:22.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-21 07:56:23.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-21 07:56:23.000000 DIRAC-8.1.0a8/src/DIRAC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.325814 DIRAC-8.1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    32452 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-02-28 16:16:58.325814 DIRAC-8.1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7255 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    41425 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/dirac.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24539 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/integration_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)   405136 2023-02-28 16:16:47.000000 DIRAC-8.1.0a9/release.notes
+-rw-r--r--   0 runner    (1001) docker     (123)    37079 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/releases.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    18988 2023-02-28 16:16:58.325814 DIRAC-8.1.0a9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      142 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.917793 DIRAC-8.1.0a9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.953795 DIRAC-8.1.0a9/src/DIRAC/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.957795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.957795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/NetworkAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.957795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/test/Test_NetworkAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.957795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/AccountingCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/DataStoreClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/ReportCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/ReportsClient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.957795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     6388 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/BaseAccountingType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/DataOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/Pilot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/PilotSubmission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/StorageOccupancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/WMSHistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.961795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    68727 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/AccountingDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/AccountingDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3755 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/MultiAccountingDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.961795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15849 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/test/Test_AccountingDB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.961795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Service/DataStoreHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8485 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Service/ReportGeneratorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.961795 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/
+-rw-r--r--   0 runner    (1001) docker     (123)    12869 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/DBUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/MainReporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.965796 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)    16007 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/BaseReporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10237 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/DataOperationPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34563 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/JobPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/NetworkPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/PilotPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/PilotSubmissionPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4925 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/StorageOccupancyPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4853 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/WMSHistoryPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.965796 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Policies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Policies/FilterExecutor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3500 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Policies/JobPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.965796 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1251 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/scripts/dirac_accounting_decode_fileid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      627 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/scripts/dirac_admin_accounting_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.965796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.965796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)    13176 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/Bdii2CSAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11384 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/GOCDB2CSAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30084 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/RucioSynchronizerAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10072 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/VOMS2CSAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.965796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/test/Test_Bdii2CS.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.969796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)    37024 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/CSAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18679 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/CSCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/CSShellCLI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      524 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/ConfigurationClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      124 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/ConfigurationData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.969796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/CSGlobals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8707 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19637 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16555 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/ResourcesDefaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      206 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.969796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31015 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/LocalConfiguration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10795 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/PathFinder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.969796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/CERNLDAPSyncPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/DummySyncPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26758 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/VOMS2CSSynchronizer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.973796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/test/Test_LocalConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/test/Test_PathFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.973796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Service/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4036 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Service/ConfigurationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Service/TornadoConfigurationHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Service/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.973796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10905 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ConfigurationClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14919 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ConfigurationData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10537 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/Modificator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3922 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/Refresher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/RefresherBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1895 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ServiceInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceTornado.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3798 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/TornadoRefresher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.977796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10705 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1455 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_shifter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3710 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_site.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7578 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_check_config_options.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4185 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_sort_cs_sites.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3051 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_voms_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      560 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1170 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_dump_local_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      438 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.977796 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/test/Test_agentOptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.977796 DIRAC-8.1.0a9/src/DIRAC/Core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.981797 DIRAC-8.1.0a9/src/DIRAC/Core/Base/
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19681 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/AgentModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7572 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/AgentReactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/CLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/Client.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1765 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/DIRACDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/ElasticDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11021 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/ExecutorMindHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/ExecutorModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9396 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/ExecutorReactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10165 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/SQLAlchemyDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8143 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/Script.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.981797 DIRAC-8.1.0a9/src/DIRAC/Core/Base/private/
+-rw-r--r--   0 runner    (1001) docker     (123)     8894 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/private/ModuleLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Base/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.981797 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13459 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/AuthManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6007 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/MessageClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3816 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/RPCClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24051 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/RequestHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11041 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/ServiceReactor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/ThreadConfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7620 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/TransferClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1085 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.985797 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28524 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/BaseClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14383 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/FileHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20839 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/GatewayService.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2922 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/InnerRPCClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1045 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/LockManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16556 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/MessageBroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/MessageFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      448 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27235 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3824 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/ServiceConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/TransportPool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.985797 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13373 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/BaseTransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23469 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/M2SSLTransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4712 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/PlainTransport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.985797 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSL/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      707 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSL/FakeSocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8489 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSL/M2Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSL/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4135 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSLTransport.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.985797 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/test/Test_SSLTransport.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/test/proxy.pem
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.985797 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11961 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/DISET/test/Test_AuthManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.985797 DIRAC-8.1.0a9/src/DIRAC/Core/LCG/
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/LCG/GGUSTicketsClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15377 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/LCG/GOCDBClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/LCG/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.989797 DIRAC-8.1.0a9/src/DIRAC/Core/LCG/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    32871 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/LCG/test/Test_LCG.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.989797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/Locations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/Properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/ProxyFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/ProxyInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13598 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/VOMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/VOMSService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.989797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509CRL.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16292 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509Certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38098 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6591 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509Request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13329 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/asn1_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.993797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11585 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/Test_X509Certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19020 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/Test_X509Chain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/Test_X509Request.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.925794 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.993797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/b236481c.0
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/ca.cert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/ca.key.pem
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/crlnumber
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/index.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/index.txt.attr
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/index.txt.attr.old
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/index.txt.old
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.993797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/1000.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/1001.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/1002.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/openssl_config_ca.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/serial
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/serial.old
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.993797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/hostcert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/hostkey.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/hostkey.pem.bak
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/openssl_config_host.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/request.csr.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/key/
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/key/encrypted_key_pass_0000.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/openssl_config_user.cnf
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/request.csr.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/usercert.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/userkey.pem
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/voms/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/voms/README
+-rw-r--r--   0 runner    (1001) docker     (123)     7784 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/voms/proxy.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    17181 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/x509TestUtilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     3447 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/ClientSelector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/TornadoClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/private/
+-rw-r--r--   0 runner    (1001) docker     (123)    28384 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/private/TornadoBaseClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/HandlerManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15769 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/TornadoREST.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/TornadoServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9037 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/TornadoService.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.997797 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/private/
+-rw-r--r--   0 runner    (1001) docker     (123)    42705 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/private/BaseRequestHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/private/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.005798 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/scripts/tornado_start_CS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/scripts/tornado_start_all.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.013798 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3321 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Adler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.013798 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ClassAd/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9584 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ClassAd/ClassAdLight.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ClassAd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/CountryMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DAG.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15565 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DEncode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10480 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DErrno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DIRACSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Devloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8396 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DictCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DirectoryExplorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21207 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ElasticSearchDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/EventDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28893 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ExecutorDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7196 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Extensions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7551 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Glue2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.017798 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/BarGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/CurveGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Dwatermark.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13486 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19352 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/GraphData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/GraphUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8750 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/LineGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Palette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5838 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/PieGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9684 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/PlotBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7880 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/QualityMapGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/JDL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7459 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/JEncode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3684 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/List.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/LockRing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/MJF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/MixedEncode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62483 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/MySQL.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1597 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8883 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ObjectLoader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3958 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Os.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7765 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Pfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Platform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.017798 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/DataCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/FileCoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5285 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/Plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/TypeLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/PrettyPrint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35966 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ProcessPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7531 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/PromptUser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10033 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8683 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ReturnValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ServerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Shifter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5683 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/SiteSEMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6691 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21989 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11484 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ThreadPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1117 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ThreadSafe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6212 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ThreadScheduler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9001 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/TimeUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.021798 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/ProcessesCreator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Adler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_DAG.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Dictionaries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ExecutorDispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4393 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4848 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_List.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ObjectLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7398 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Pfn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10890 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ProcessPool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4143 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ReturnValues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Subprocess.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2225 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Time.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_entrypoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.025799 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12631 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Module.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    26903 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Parameter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20689 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.025799 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/WFEditor/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/WFEditor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18115 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5245 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/WorkflowReader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.025799 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18060 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/JobSamples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1671 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/ModulesSamples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8537 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/WFSamples.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21830 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/step_g.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.029799 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1740 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_cert_convert.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28789 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_configure.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1818 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_generate_cas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_generate_crls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3736 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1241 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_install_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      618 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_install_web_portal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5594 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_platform.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1689 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1790 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_setup_site.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      662 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5457 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/scripts/install_full.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.029799 DIRAC-8.1.0a9/src/DIRAC/Core/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Core/test/Test_API.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.029799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.029799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)    25103 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/FTS3Agent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.033799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ArchiveFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/CheckMigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/DMSRequestOperationsBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/MoveReplica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7322 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PhysicalRemoval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PutAndRegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReTransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4858 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterReplica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10330 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7972 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveReplica.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28019 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReplicateAndRegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/StagingCallback.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.033799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ArchiveFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_CheckMigration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23364 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ReplicateAndRegister.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8292 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_RequestOperations.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.037799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.037799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/AbstractFileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/DirectoryCompletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31227 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/ConsistencyInspector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9130 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/DataIntegrityClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81684 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/DataManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/DirectoryListing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3File.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33837 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3Job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24570 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13164 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FailoverTransfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80127 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FileCatalogClientCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9634 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/MetaQuery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/S3GatewayClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.037799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3956 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15333 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/Test_FTS3Objects.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/mock_DM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/new_dir_completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.037799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/DataIntegrityDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/DataIntegrityDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    27895 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FTS3DB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FTS3DB.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.041799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.041799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/
+-rw-r--r--   0 runner    (1001) docker     (123)    31121 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/DatasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.041799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/
+-rw-r--r--   0 runner    (1001) docker     (123)    23739 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryClosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryFlatTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20157 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryLevelTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryNodeTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectorySimpleTree.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49195 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryTreeBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.041799 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    37600 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/DirectoryMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/MultiVODirectoryMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.045800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35622 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManager.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54588 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15554 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerFlat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    33910 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerPs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.045800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    27746 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/FileMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/MultiVOFileMetadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.045800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.045800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManagerWithDelete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/FullSecurityManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/NoSecurityManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/SecurityManagerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23975 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/VOMSSecurityManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.045800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    55701 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/test/Test_VOMSSecurityManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.045800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerCS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.049800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/test/Test_DataManagement_FileCatalogComponents.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43086 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9007 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61258 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogWithFkAndPsDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.049800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/test/Test_FTS3DB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.049800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/DataIntegrityHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/FTS3ManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25949 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/FileCatalogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6299 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/S3GatewayHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18963 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/StorageElementHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/TornadoDataIntegrityHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/TornadoFTS3ManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/TornadoFileCatalogHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/TornadoS3GatewayHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       54 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.049800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/test/Test_Service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.049800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    19049 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/DMSHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/ResolveSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.049800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10846 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/test/Test_resolveSE.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       46 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.053800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.053800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/DefaultFTS3Plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.053800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12778 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/test/Test_DefaultFTS3Plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/HttpStorageAccessHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.053800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7360 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/test/Test_FTS3Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.057800 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7413 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_admin_allow_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9938 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_admin_ban_se.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_admin_user_quota.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3442 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2368 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_catalog_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1778 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_change_replica_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1782 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_clean_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22462 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_archive_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_moving_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3535 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_removal_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2478 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_data_size.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18000 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_directory_sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3339 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_filecatalog_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2423 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_find_lfns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3948 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_move_replica_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9097 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_protocol_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2700 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_put_and_register_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2241 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2236 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_replicas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1883 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1908 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replica_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4524 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replicate_and_register_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1230 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_resolve_guid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2344 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_set_replica_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3150 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_show_se_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5779 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_lfns.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1058 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_quota.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.061801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.061801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/API/
+-rw-r--r--   0 runner    (1001) docker     (123)    21970 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/API/AuthHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/API/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.061801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)    26043 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/ComponentSupervisionAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/ProxyRenewalAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.061801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    33839 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/test/Test_ComponentSupervisionAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.065801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/BundleDeliveryClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99348 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ComponentInstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ComponentMonitoringClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      145 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/NotificationClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10396 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ProxyGeneration.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27110 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ProxyManagerClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ProxyUpload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SecurityLogClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52784 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClientCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SystemAdministratorIntegrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/TokenManagerClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/UserProfileClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.065801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/test/Test_ComponentInstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6207 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.069801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    11929 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/AuthDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/AuthDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    43144 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/InstalledComponentsDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/InstalledComponentsDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    35430 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/NotificationDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/NotificationDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54769 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/ProxyDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/ProxyDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8649 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/TokenDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/TokenDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21493 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/UserProfileDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/UserProfileDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.069801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/BundleDeliveryHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13527 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/ComponentMonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/NotificationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17387 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/ProxyManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/SecurityLoggingHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26488 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/SystemAdministratorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TokenManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoComponentMonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoNotificationHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoProxyManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoUserProfileManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5707 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/UserProfileManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.069801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Utilities/MonitoringUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.069801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/SecurityFileLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.073801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)    23068 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/AuthServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.073801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/AuthorizationCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/DeviceFlow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/RefreshToken.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/RevokeToken.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.073801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6351 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.073801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.073801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/BaseFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/ColoredBaseFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/MicrosecondJsonFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.077801 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/MessageQueueHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/LogLevels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21874 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10440 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/LoggingRoot.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.081802 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/TestLogUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LogLevels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LoggingRoot_ConfigForExternalLibs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5114 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_CreationLogRecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12614 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_FormatOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_GetSubLogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.089802 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      961 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_CAs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5344 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      716 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_proxy_upload.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_sysadmin_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9454 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_instance.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2237 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_pilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2681 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_users_with_proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4424 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_install_component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3547 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_install_tornado_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15816 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_logout.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7966 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_populate_component_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5010 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_destroy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3692 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_get_uploaded_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5864 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10373 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1275 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_restart_component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1289 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_start_component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1658 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_status_component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1272 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_stop_component.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2453 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_sys_sendmail.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2797 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_uninstall_component.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.089802 DIRAC-8.1.0a9/src/DIRAC/Interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.093802 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    93582 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/Dirac.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31377 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/DiracAdmin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    51360 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/Job.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      566 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.093802 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/Test_DIRAC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/Test_JobAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/testWF.jdl
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/testWF.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/testWFSIO.jdl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.093802 DIRAC-8.1.0a9/src/DIRAC/Interfaces/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    21666 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/Utilities/DCommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/Utilities/DConfigCache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.117803 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1317 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dcd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1692 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dchgrp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1695 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dchmod.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1667 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dchown.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2693 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dconfig.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1204 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dfind.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3459 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dget.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dgetenv.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2148 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dinit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2795 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3305 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_add_host.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3036 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_add_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3274 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_allow_site.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3341 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_ban_site.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1310 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_ce_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1542 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_delete_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1059 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_banned_sites.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1388 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilot_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3037 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4525 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2191 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_logging_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1225 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      930 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_site_mask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1208 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_list_hosts.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2183 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_list_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2271 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_modify_user.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1466 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_pilot_summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1279 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_reset_job.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1318 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_service_ports.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1283 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_set_site_protocols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1305 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_site_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1174 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_site_mask_logging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1825 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_sync_users_from_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1359 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_get_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1703 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_accessURL.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2247 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1557 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_replicas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_accessURL.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1257 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_metadata.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1971 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_replicate_lfn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2978 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_framework_ping_service.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_framework_self_ping.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_utils_file_adler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1137 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_utils_file_md5.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1337 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_get_normalized_queue_length.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_get_queue_normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2107 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_attributes.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2152 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_delete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1444 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1937 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_jdl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3708 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1287 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1493 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2838 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_logging_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1914 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1042 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_peek.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1155 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_reschedule.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2249 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2273 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3477 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_jobs_select_output_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4153 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_select_jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2544 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dkill.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1516 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dlogging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14827 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dls.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5170 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dmeta.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1322 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dmkdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5866 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/doutput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4506 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dput.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      479 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dpwd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3017 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/drepl.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1309 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dreplicas.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3769 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/drm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1138 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/drmdir.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2033 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7250 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dstat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15504 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dsub.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.117803 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.117803 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     7911 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/DataOperationSender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/MonitoringClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8046 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/MonitoringReporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/ServerUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.121803 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/AgentMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/BaseType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/DataOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/FailedDataOperation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/PilotSubmissionMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/PilotsHistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/RMSMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/ServiceMonitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/WMSHistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.121803 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    21402 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/MonitoringDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.121803 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/test/Test_monitoringdb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.121803 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Service/MonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Service/TornadoMonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.125804 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/DBUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/MainReporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.125804 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/
+-rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/BasePlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/RMSMonitoringPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/WMSHistoryPlotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.125804 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.125804 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Client/ProductionClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2270 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Client/ProductionStep.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.125804 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    25437 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/DB/ProductionDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3130 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/DB/ProductionDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.125804 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)     5587 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Service/ProductionManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Service/TornadoProductionManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.129804 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     3758 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/ProdTransManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5568 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/ProdValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.129804 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2332 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_add_trans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      721 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_clean.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_complete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_delete.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1488 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1259 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      846 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_description.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3060 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_trans.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      795 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_start.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      794 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_stop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.129804 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.133804 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/CleanReqDBAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20038 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestExecutingAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.133804 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2934 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/ForwardDISET.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.133804 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/test/ForwardDISETTests.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.137804 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/File.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11101 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/Operation.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27746 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/ReqClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/Request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.137804 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/Test_File.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/Test_Operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14706 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/Test_Request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.141805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       94 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/ReqDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    35114 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/RequestDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       52 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.141805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/test/RMSTestScenari.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/test/Test_RequestDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.141805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13798 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/ReqManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8793 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/ReqProxyHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/TornadoReqManagerHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.145805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/test/OperationHandlerBaseTests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       49 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.145805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/JSONUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10557 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/OperationHandlerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/RequestTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11362 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/RequestValidator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.149805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/Test_OperationHandlerBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/Test_RequestTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3905 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/Test_RequestValidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.149805 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1201 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_list_req_cache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1246 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_reqdb_summary.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11656 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.149805 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.153805 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/CacheFeederAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7045 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/ElementInspectorAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6034 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/EmailAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6531 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/RucioRSSAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/SiteInspectorAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9152 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/SummarizeLogsAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/TokenAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.157805 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ElementInspectorAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4987 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ResourceStatusSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_SiteInspectorAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.157805 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/PublisherClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33305 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/ResourceManagementClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/ResourceStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18329 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/ResourceStatusClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10928 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/SiteStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.165806 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/Command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/CommandCaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15358 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/DowntimeCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/FreeDiskSpaceCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/GGUSTicketsCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/GOCDBSyncCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6371 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/JobCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/MacroCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/PilotCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/PropagationCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/TransferCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.165806 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    12289 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBStatusCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBSyncCommand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.169806 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    19205 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/ResourceManagementDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/ResourceManagementDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    15990 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/ResourceStatusDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/ResourceStatusDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.177806 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysActivePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysBannedPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysDegradedPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysProbingPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/CEAvailabilityPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/Configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/DowntimePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/FreeDiskSpacePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/GGUSTicketsPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobDoneRatioPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobEfficiencyPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobRunningMatchedRatioPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobRunningWaitingRatioPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/PilotEfficiencyPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/PropagationPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.181806 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_AlwaysActivePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_CEAvailabilityPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_DTPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3698 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_FreeDiskSpacePolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2693 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_GGUSTicketsPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobDoneRatioPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobEfficiencyPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3991 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningMatchedRatioPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningWaitingRatioPolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_PilotEfficiencyPolicy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.185807 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.189807 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/BaseAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogPolicyResultAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogStatusAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/SlackAction.py
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16416 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PDP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PEP.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyCaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.189807 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/test/Test_PolicySystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.193807 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/PublisherHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/ResourceManagementHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/ResourceStatusHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/TornadoPublisherHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/TornadoResourceManagementHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/TornadoResourceStatusHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.197807 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     4438 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/CSHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/InfoGetter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/RSSCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15514 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/RSSCacheNoThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3337 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/RssConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20184 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/Synchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2436 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.201807 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4572 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_list_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13824 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_db.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9929 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_dtcache.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7942 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_status.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6167 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_token.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7616 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.201807 DIRAC-8.1.0a9/src/DIRAC/Resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.205808 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.209808 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/DummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/FCConditionBasePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/FilenamePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4273 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/ProxyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.209808 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_FilenamePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_ProxyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11002 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FCConditionParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25900 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalogClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalogClientBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalogFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11778 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/PoolXMLCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/PoolXMLFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30541 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/RucioFileCatalogClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/TSCatalogClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/Utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.209808 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/Test_FCConditionParser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/Test_FileCatalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/mock_FC.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.221809 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9187 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ARC6ComputingElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28706 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ARCComputingElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31726 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/AREXComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13904 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BOINCComputingElement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.225809 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/
+-rw-r--r--   0 runner    (1001) docker     (123)    10273 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/Condor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9170 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/GE.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/Host.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/LSF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8846 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/OAR.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13795 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/SLURM.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.229809 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/HTCondorResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/LSFResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/MJFResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/PBSResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/ResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SGEResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SLURMResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/TimeLeft.py
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.233809 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_LSFResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_PBSResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_SGEResourceUsage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_TimeLeft.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/Torque.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/executeBatch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.233809 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/test/Test_SLURM.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17901 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/CREAMComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24156 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/CloudComputingElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22102 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ComputingElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2525 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ComputingElementFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27177 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/HTCondorCEComputingElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4750 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/InProcessComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13399 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/LocalComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/PilotBundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10290 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/PoolComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6693 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SSHBatchComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32135 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SSHComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19374 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SingularityComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9265 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SudoComputingElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       43 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6224 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/cloudinit.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.237809 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_HTCondorCEComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_InProcessComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8098 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_PoolComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_SSHComputingElement.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.241809 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/CheckInIdProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/IAMIdProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/IdProviderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21798 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/OAuth2IdProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.241809 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/AbstractBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/ElasticSearchBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/FileBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/MessageQueueBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/StderrBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/StdoutBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/StdoutJsonBackend.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.241809 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/ModuleFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/PatternFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/SensitiveDataFilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.241809 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/test/Test_LogFilter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.245810 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQCommunication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16807 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQConnectionManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQConnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQConsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQProducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.245810 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/Simple/
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/Simple/StompInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/Simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13023 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/StompMQConnector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.245810 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    32690 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQConnectionManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQConsumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQProducer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQ_Utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.249810 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/
+-rw-r--r--   0 runner    (1001) docker     (123)    18699 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/DIRACCAProxyProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/PUSPProxyProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/ProxyProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/ProxyProviderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.249810 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7538 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/test/Test_DIRACCAProxyProvider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/test/Test_ProxyProviderFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.253810 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/CTAStorage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19817 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/DIPStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/EchoStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/FCOnlyStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22075 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/FileStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_GSIFTPStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_HTTPSStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8844 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_SRM2Storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58784 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_StorageBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_XROOTStorage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.253810 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/BDIIOccupancy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingHTTPJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingJson.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42741 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/RFIOStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28080 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/S3Storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16350 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/StorageBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61603 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/StorageElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19435 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/StorageFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/Utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.257810 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    32777 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/FIXME_Test_RFIOPlugIn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    39829 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/FIXME_Test_StorageElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36441 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/FIXME_Test_StoragePlugIn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18987 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_FilePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_GFAL2_XROOTStorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_StorageElement.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22448 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_StorageFactory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       45 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/test_utilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       33 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.257810 DIRAC-8.1.0a9/src/DIRAC/Resources/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1116 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/scripts/dirac_resource_get_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4934 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Resources/scripts/dirac_resource_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.257810 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.261810 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7862 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/RequestFinalizationAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11601 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/RequestPreparationAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9727 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/StageMonitorAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24891 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/StageRequestAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.261810 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)     9763 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/StorageManagerClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.261810 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8185 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/test/Test_Client_StorageManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.261810 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    63907 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.261810 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Service/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15033 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Service/StorageManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Service/TornadoStorageManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.265811 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4379 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5626 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_jobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2324 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_request.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7357 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_requests.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3131 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_show_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2673 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_stage_files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.265811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.269811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/
+-rw-r--r--   0 runner    (1001) docker     (123)    26982 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/DataRecoveryAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7642 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/InputDataAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5266 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/MCExtensionAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.269811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/RequestOperations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/RequestOperations/SetFileStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/RequestOperations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/RequestTaskAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31606 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TaskManagerAgentBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32734 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationAgentsUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31929 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11322 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10108 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1770 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.269811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     9698 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/test/Test_Agent_TransformationSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/test/Test_Plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.273811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.273811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/BodyPlugin/
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/BodyPlugin/BaseBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/BodyPlugin/DummyBody.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/BodyPlugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/FileReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/PluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15929 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/RequestTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TaskManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TaskManagerPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28485 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/Transformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25401 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationCLI.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26048 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationFilesStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28710 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/WorkflowTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.273811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_RequestTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10760 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_TaskManagerPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13760 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_WorkflowTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.277811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/DB/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78503 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/DB/TransformationDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6835 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/DB/TransformationDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.277811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Service/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Service/TornadoTransformationManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30589 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Service/TransformationManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.277811 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)    10706 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/JobInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/ReplicationCLIParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/ReplicationTransformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/ScriptUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/TransformationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.281812 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4793 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1553 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      790 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      783 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      363 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_cli.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      802 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_get_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1961 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_information.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1854 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_recover_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_remove_output.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1404 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_replication.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1941 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_update_derived.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      851 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_verify_outputdata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.281812 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    27128 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_DRA.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26685 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_JobInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15430 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_TransformationInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_replicationTransformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.285812 DIRAC-8.1.0a9/src/DIRAC/Workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.285812 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/FailoverRequest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23090 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/ModuleBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/Script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/UploadOutputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.285812 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    32354 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/test/Test_Modules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.285812 DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.285812 DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/test/Test_Utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/Workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.285812 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.289812 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37109 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/JobAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14791 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/JobCleaningAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13572 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/OptimizerModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10615 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/PilotStatusAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4728 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/PilotSyncAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17075 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/PushJobAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61576 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/SiteDirector.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25262 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/StalledJobAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6643 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/StatesAccountingAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/TaskQueuesAgent.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.289812 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15913 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobCleaningAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PilotStatusAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PushJobAgent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_SiteDirector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_StalledJobAgent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.297812 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/CPUNormalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16387 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/DownloadInputData.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13084 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/InputDataByProtocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/InputDataResolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobManagerClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobMinorStatus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2205 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobMonitoringClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobReport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.297812 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/
+-rw-r--r--   0 runner    (1001) docker     (123)    12787 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/CachedJobState.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8963 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobManifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13004 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobState.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobStateUpdateClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10070 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/Limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/Matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/MatcherClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/PilotManagerClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/PilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/PoolXMLSlice.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11811 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/SandboxStoreClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/ServerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/WMSAdministratorClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9256 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/WMSClient.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.297812 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_DownloadInputData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_WorkloadManagementSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/Test_JobReport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9384 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/ConfigTemplate.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.301813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/
+-rw-r--r--   0 runner    (1001) docker     (123)    14130 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/ElasticJobParametersDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    76374 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6817 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5615 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1869 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49685 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3023 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    16964 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/SandboxMetadataDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/SandboxMetadataDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57007 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.sql
+-rwxr-xr-x   0 runner    (1001) docker     (123)       53 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.301813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/tests/Test_JobDB.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.301813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.301813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/Base/
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/Base/OptimizerExecutor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       56 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/Base/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18049 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/InputData.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2511 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/JobPath.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6301 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/JobSanity.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27868 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/JobScheduling.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.305813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/test/Test_Executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.305813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70468 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11164 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapperTemplate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    42540 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/Watchdog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.305813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_JobWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_Watchdog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/jobDescription.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)        7 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/script-OK.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       10 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/script-RESC.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)        9 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/script.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.309813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25264 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobManagerHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22130 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobMonitoringHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8237 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobPolicy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11062 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobStateUpdateHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/MatcherHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/OptimizationMindHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18743 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/PilotManagerHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    21484 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/SandboxStoreHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobManagerHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobMonitoringHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobStateUpdateHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/TornadoWMSAdministratorHandler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9073 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/WMSAdministratorHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/WMSUtilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       58 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.313813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/JobParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10881 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/JobStatusUtility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/ParametricJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/PilotCStoJSONSynchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11088 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/PilotWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/QueueUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/RemoteRunner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5076 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.313813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_JobStatusUtility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_ParametricJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4352 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotCStoJSONSynchronizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotWrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_QueueUtilities.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       50 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.313813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/ConfigHelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/SharesCorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.317813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseCorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseHistoryCorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/MonitoringHistoryCorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/WMSHistoryCorrector.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.317813 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      931 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_kill_pilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3248 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_show_task_queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_sync_pilot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4273 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_jobexec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3106 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_cpu_normalization.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1107 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_queue_cpu_time.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7506 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1476 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_match.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3233 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_pilot_job_info.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11458 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.321813 DIRAC-8.1.0a9/src/DIRAC/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.321813 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/Accounting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/IntegrationTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/ProcessesCreator_withChildren.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/WMS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/assertingUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/mpTest-flexible.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/mpTest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/testJobDefinitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.949795 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.321813 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Integration/exe-script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Integration/helloWorld.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:58.325814 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Regression/
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Regression/helloWorld.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5310 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Regression/helloWorld.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:15.000000 DIRAC-8.1.0a9/src/DIRAC/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 16:16:57.953795 DIRAC-8.1.0a9/src/DIRAC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7985 2023-02-28 16:16:57.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    72031 2023-02-28 16:16:57.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 16:16:57.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17133 2023-02-28 16:16:57.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 16:16:56.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-28 16:16:57.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-28 16:16:57.000000 DIRAC-8.1.0a9/src/DIRAC.egg-info/top_level.txt
```

### Comparing `DIRAC-8.1.0a8/AUTHORS.rst` & `DIRAC-8.1.0a9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/LICENSE` & `DIRAC-8.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/PKG-INFO` & `DIRAC-8.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DIRAC
-Version: 8.1.0a8
+Version: 8.1.0a9
 Summary: DIRAC is an interware, meaning a software framework for distributed computing.
 Home-page: https://github.com/DIRACGrid/DIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DIRAC-8.1.0a8/README.rst` & `DIRAC-8.1.0a9/README.rst`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/dirac.cfg` & `DIRAC-8.1.0a9/dirac.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
       # If not specified, the VO "DefaultGroup" will be used
       VOAdminGroup = lhcb_admin
 
       # Real VOMS VO name, if this VO is associated with VOMS VO
       VOMSName = lhcb
 
       # Registered identity provider associated with VO
-      IdP = CheckIn
+      IdProvider = CheckIn
 
       # Section to describe all the VOMS servers that can be used with the given VOMS VO
       VOMSServers
       {
 
         # The host name of the VOMS server
         cclcgvomsli01.in2p3.fr
```

### Comparing `DIRAC-8.1.0a8/environment.yml` & `DIRAC-8.1.0a9/environment.yml`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/integration_tests.py` & `DIRAC-8.1.0a9/integration_tests.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/pyproject.toml` & `DIRAC-8.1.0a9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -24,14 +24,39 @@
     'src/DIRAC/Core/Utilities/ReturnValues.py',
     'src/DIRAC/Core/Security/Properties.py'
 ]
 exclude = [
     '/tests/'
 ]
 
+[tool.pylint.basic]
+
+# We mostly have CamelCase, with a few differences.
+# In tests we have quite some snake_case, mostly due to pytest
+# We can instruct pylint to understand both, but the problem is that it
+# will stick to one style per file (i.e if the first variable is snake,
+# all the following must be snake)
+# It's not quite the case yet...
+# For the time being, I wrote the regex that matches best our code.
+# (except for the services with their export_ and types_ ...)
+# We will see about tests later...
+# See https://pylint.readthedocs.io/en/latest/user_guide/messages/convention/invalid-name.html#multiple-naming-styles-for-custom-regular-expressions
+
+# Camel case with capital letter first
+class-rgx = '([A-Z][a-z]*)+$'
+module-rgx = '([A-Z][a-z]*)+$'
+
+# Attributes, variables, functions and methods
+# are camelCase, but can start with one or two understcore
+attr-rgx = '(?:_*[a-z]+([A-Z][a-z]*)*)$'
+variable-rgx = '(?:_*[a-z]+([A-Z][a-z]*)*)$'
+function-rgx = '(?:_*[a-z]+([A-Z][a-z]*)*)$'
+method-rgx = '(?:_*[a-z]+([A-Z][a-z]*)*)$'
+
+argument-naming-style = "camelCase"
 
 [tool.pylint.main]
 # Files or directories to be skipped. They should be base names, not paths.
 ignore = [".svn", ".git", "integration_tests.py"]
 
 # List of module names for which member attributes should not be checked (useful
 # for modules/projects where namespaces are manipulated during runtime and thus
```

### Comparing `DIRAC-8.1.0a8/release.notes` & `DIRAC-8.1.0a9/release.notes`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,62 @@
+[v8.1.0a9]
+
+*ConfigurationSystem
+
+FIX: (#6868) VOMS2CSAgent: strip whitespaces from DN entried and nickname
+NEW: (#6865) Resources helper - getQueues() - can select queues by Tag values also
+
+*FrameworkSystem
+
+FIX: (#6865) TokenManager - use refreshToken flow to generate access tokens from the stored refresh tokens
+
+*WorkloadManagement
+
+NEW: (#6865) SiteDirector enabled to select queues by tags
+NEW: (#6865) SiteDirector sets up tokens for ComputingElements configured with the Token tag
+
+*Resources
+
+NEW: (#6865) HTCondorComputingElement, ARC(6)ComputingElement and AREXComputingElement enabled to for job operations with tokens
+FIX: (#6842) Complete AREX renewal
+
+*DataManagementSystem
+
+NEW: (#6863) ReplicateAndRegister FTS mode also checks the SE status
+NEW: (#6863) add a delay in monitoring in the FTS3Agent
+NEW: (#6860) dirac-dms-filecatalog-cli - use the default VO FileCatalog if not explicitly specified
+CHANGE: (#6835) Speed up ReplicateAndRegister operation
+
+*dashboards/PilotSubmissions
+
+FIX: (#6858) efficiency plots now use heatmaps
+FIX: (#6858) index patterns are now environment agnostic
+
+*dashboards/ServiceMonitoring
+
+FIX: (#6858) index patterns are now environment agnostic
+
+*dashboards/AgentMonitoring
+
+FIX: (#6858) index patterns are now environment agnostic
+
+*dashboards/PilotsHistory
+
+FIX: (#6858) style of plots
+FIX: (#6858) index patterns are now environment agnostic
+
+*Interfaces
+
+NEW: (#6853) Add setPriority to Job API
+FIX: (#6849) removed print statements and replaced with gLogger as appropriate as requested in #6746
+
+*RequestManagementSystem
+
+CHANGE: (#6848) ReqProxy does not attempt a direct forward to central ReqManager
+
 [v8.1.0a8]
 
 *Resources
 
 FIX: (#6832) Update AREX delegation renewal
 FIX: (#6830) Fix AREX ARCRESTTimeout
 FIX: (#6817) fix account parameter in SSHBatchCE
```

### Comparing `DIRAC-8.1.0a8/releases.cfg` & `DIRAC-8.1.0a9/releases.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/setup.cfg` & `DIRAC-8.1.0a9/setup.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/NetworkAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/NetworkAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Agent/test/Test_NetworkAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Agent/test/Test_NetworkAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/AccountingCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/AccountingCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/DataStoreClient.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/DataStoreClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/ReportCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/ReportCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/ReportsClient.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/ReportsClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/BaseAccountingType.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/BaseAccountingType.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/DataOperation.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/DataOperation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/Job.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/Job.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/Network.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/Network.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/Pilot.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/Pilot.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/PilotSubmission.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/PilotSubmission.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/StorageOccupancy.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/StorageOccupancy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Client/Types/WMSHistory.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Client/Types/WMSHistory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/AccountingDB.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/AccountingDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/MultiAccountingDB.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/MultiAccountingDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/DB/test/Test_AccountingDB.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/DB/test/Test_AccountingDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Service/DataStoreHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Service/DataStoreHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/Service/ReportGeneratorHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/Service/ReportGeneratorHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/DBUtils.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/DBUtils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/MainReporter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/MainReporter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/BaseReporter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/BaseReporter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/DataOperationPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/DataOperationPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/JobPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/JobPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/NetworkPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/NetworkPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/PilotPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/PilotPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/PilotSubmissionPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/PilotSubmissionPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/StorageOccupancyPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/StorageOccupancyPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Plotters/WMSHistoryPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Plotters/WMSHistoryPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Policies/FilterExecutor.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Policies/FilterExecutor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/private/Policies/JobPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/private/Policies/JobPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/scripts/dirac_accounting_decode_fileid.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/scripts/dirac_accounting_decode_fileid.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/AccountingSystem/scripts/dirac_admin_accounting_cli.py` & `DIRAC-8.1.0a9/src/DIRAC/AccountingSystem/scripts/dirac_admin_accounting_cli.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/Bdii2CSAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/Bdii2CSAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/GOCDB2CSAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/GOCDB2CSAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/RucioSynchronizerAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/RucioSynchronizerAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/VOMS2CSAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/VOMS2CSAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Agent/test/Test_Bdii2CS.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Agent/test/Test_Bdii2CS.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/CSAPI.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/CSAPI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/CSCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/CSCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/CSShellCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/CSShellCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Config.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Config.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/ConfigurationClient.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/ConfigurationClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/CSGlobals.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/CSGlobals.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Operations.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Operations.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Path.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Path.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Registry.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,31 +159,31 @@
     dn = dn.strip()
     result = getUsernameForDN(dn)
     if not result["OK"]:
         return result
     return findDefaultGroupForUser(result["Value"])
 
 
-def findDefaultGroupForUser(userName):
+def findDefaultGroupForUser(username):
     """Get default group for user
 
-    :param str userName: user name
+    :param str username: user name
 
     :return: S_OK(str)/S_ERROR()
     """
-    defGroups = getUserOption(userName, "DefaultGroup", [])
+    defGroups = getUserOption(username, "DefaultGroup", [])
     defGroups += gConfig.getValue(f"{gBaseRegistrySection}/DefaultGroup", ["user"])
-    result = getGroupsForUser(userName)
+    result = getGroupsForUser(username)
     if not result["OK"]:
         return result
     userGroups = result["Value"]
     for group in defGroups:
         if group in userGroups:
             return S_OK(group)
-    return S_OK(userGroups[0]) if userGroups else S_ERROR(f"User {userName} has no groups")
+    return S_OK(userGroups[0]) if userGroups else S_ERROR(f"User {username} has no groups")
 
 
 def getAllUsers():
     """Get all users
 
     :return: list
     """
@@ -345,24 +345,24 @@
     :return: list -- contain matched properties
     """
     if isinstance(propList, str):
         propList = [propList]
     return __matchProps(propList, getPropertiesForHost(hostName))
 
 
-def getUserOption(userName, optName, defaultValue=""):
+def getUserOption(username, optName, defaultValue=""):
     """Get user option
 
-    :param str userName: user name
+    :param str username: user name
     :param str optName: option name
     :param defaultValue: default value
 
     :return: defaultValue or str
     """
-    return gConfig.getValue(f"{gBaseRegistrySection}/Users/{userName}/{optName}", defaultValue)
+    return gConfig.getValue(f"{gBaseRegistrySection}/Users/{username}/{optName}", defaultValue)
 
 
 def getGroupOption(groupName, optName, defaultValue=""):
     """Get group option
 
     :param str groupName: group name
     :param str optName: option name
@@ -426,15 +426,15 @@
 def getIdPForGroup(group):
     """Get identity provider for group VO
 
     :param str group: group name
 
     :return: str
     """
-    return getVOOption(getVOForGroup(group), "IdP")
+    return getVOOption(getVOForGroup(group), "IdProvider")
 
 
 def getDefaultVOMSAttribute():
     """Get default VOMS attribute
 
     :return: str
     """
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/Resources.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/Resources.py`

 * *Files 3% similar despite different names*

```diff
@@ -224,16 +224,25 @@
         if tags:
             resultDict[tagFieldName] = tags
 
     resultDict["Queue"] = queue
     return S_OK(resultDict)
 
 
-def getQueues(siteList=None, ceList=None, ceTypeList=None, community=None):
-    """Get CE/queue options according to the specified selection"""
+def getQueues(siteList=None, ceList=None, ceTypeList=None, community=None, tags=None):
+    """Get CE/queue options according to the specified selection
+
+    :param str list siteList: sites to be selected
+    :param str list ceList: CEs to be selected
+    :param str list ceTypeList: CE types to be selected
+    :param str community: selected VO
+    :param str list tags: tags required for selection
+
+    :return: S_OK/S_ERROR with Value - dictionary of selected Site/CE/Queue parameters
+    """
 
     result = gConfig.getSections("/Resources/Sites")
     if not result["OK"]:
         return result
 
     resultDict = {}
 
@@ -255,14 +264,15 @@
             if result["OK"]:
                 siteCEParameters = result["Value"]
             result = gConfig.getSections(f"/Resources/Sites/{grid}/{site}/CEs")
             if not result["OK"]:
                 continue
             ces = result["Value"]
             for ce in ces:
+                ceTags = gConfig.getValue(f"/Resources/Sites/{grid}/{site}/CEs/{ce}/Tag", [])
                 if ceTypeList:
                     ceType = gConfig.getValue(f"/Resources/Sites/{grid}/{site}/CEs/{ce}/CEType", "")
                     if not ceType or ceType not in ceTypeList:
                         continue
                 if ceList and ce not in ceList:
                     continue
                 if community:
@@ -279,14 +289,19 @@
                     continue
                 queues = result["Value"]
                 for queue in queues:
                     if community:
                         comList = gConfig.getValue(f"/Resources/Sites/{grid}/{site}/CEs/{ce}/Queues/{queue}/VO", [])
                         if comList and community.lower() not in [cl.lower() for cl in comList]:
                             continue
+                    if tags:
+                        queueTags = gConfig.getValue(f"/Resources/Sites/{grid}/{site}/CEs/{ce}/Queues/{queue}/Tag", [])
+                        queueTags = set(ceTags + queueTags)
+                        if not queueTags or not set(tags).issubset(queueTags):
+                            continue
                     resultDict.setdefault(site, {})
                     resultDict[site].setdefault(ce, ceOptionsDict)
                     resultDict[site][ce].setdefault("Queues", {})
                     result = gConfig.getOptionsDict(f"/Resources/Sites/{grid}/{site}/CEs/{ce}/Queues/{queue}")
                     if not result["OK"]:
                         continue
                     queueOptionsDict = result["Value"]
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/ResourcesDefaults.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/ResourcesDefaults.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Helpers/test/Test_Helpers.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/LocalConfiguration.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/LocalConfiguration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/PathFinder.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/PathFinder.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/CERNLDAPSyncPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/CERNLDAPSyncPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/DummySyncPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/SyncPlugins/DummySyncPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/VOMS2CSSynchronizer.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/VOMS2CSSynchronizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,15 +269,15 @@
                     diracName = nickName
                     # This is a flag for adding the new DN to an already existing user
                     newDNForExistingUser = dn
 
                 # We have a real new user
                 if not diracName:
                     if nickName:
-                        newDiracName = nickName
+                        newDiracName = nickName.strip()
                     else:
                         newDiracName = self.getUserName(dn)
 
                     # Do not consider users with Suspended status in VOMS
                     if self.vomsUserDict[dn]["suspended"] or self.vomsUserDict[dn]["certSuspended"]:
                         resultDict["SuspendedUsers"].append(newDiracName)
                         continue
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/test/Test_LocalConfiguration.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/test/Test_LocalConfiguration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Client/test/Test_PathFinder.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Client/test/Test_PathFinder.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Service/ConfigurationHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Service/ConfigurationHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/Service/TornadoConfigurationHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/Service/TornadoConfigurationHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ConfigurationClient.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ConfigurationClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ConfigurationData.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ConfigurationData.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/Modificator.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/Modificator.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/Refresher.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/Refresher.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/RefresherBase.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/RefresherBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ServiceInterface.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ServiceInterface.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceBase.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceTornado.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/ServiceInterfaceTornado.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/private/TornadoRefresher.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/private/TornadoRefresher.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_resources.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_resources.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_shifter.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_shifter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_site.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_add_site.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_check_config_options.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_check_config_options.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_sort_cs_sites.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_sort_cs_sites.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_voms_sync.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_admin_voms_sync.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_cli.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_cli.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_dump_local_cache.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/scripts/dirac_configuration_dump_local_cache.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ConfigurationSystem/test/Test_agentOptions.py` & `DIRAC-8.1.0a9/src/DIRAC/ConfigurationSystem/test/Test_agentOptions.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/API.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/API.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/AgentModule.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/AgentModule.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/AgentReactor.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/AgentReactor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/CLI.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/CLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/Client.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/Client.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/DB.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/DB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/DIRACDB.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/DIRACDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/ElasticDB.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/ElasticDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/ExecutorMindHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/ExecutorMindHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/ExecutorModule.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/ExecutorModule.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/ExecutorReactor.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/ExecutorReactor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/SQLAlchemyDB.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/SQLAlchemyDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/Script.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/Script.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Base/private/ModuleLoader.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Base/private/ModuleLoader.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/AuthManager.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/AuthManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/MessageClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/MessageClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/RPCClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/RPCClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/RequestHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/ServiceReactor.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/ServiceReactor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/ThreadConfig.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/ThreadConfig.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/TransferClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/TransferClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/BaseClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/BaseClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/FileHelper.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/FileHelper.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/GatewayService.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/GatewayService.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/InnerRPCClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/InnerRPCClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/LockManager.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/LockManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/MessageBroker.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/MessageBroker.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/MessageFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/MessageFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Service.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Service.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/ServiceConfiguration.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/ServiceConfiguration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/TransportPool.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/TransportPool.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/BaseTransport.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/BaseTransport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/M2SSLTransport.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/M2SSLTransport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/PlainTransport.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/PlainTransport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSL/FakeSocket.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSL/FakeSocket.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSL/M2Utils.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSL/M2Utils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/SSLTransport.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/SSLTransport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/test/Test_SSLTransport.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/test/Test_SSLTransport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/private/Transports/test/proxy.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/private/Transports/test/proxy.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/DISET/test/Test_AuthManager.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/DISET/test/Test_AuthManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/LCG/GGUSTicketsClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/LCG/GGUSTicketsClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/LCG/GOCDBClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/LCG/GOCDBClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/LCG/test/Test_LCG.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/LCG/test/Test_LCG.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/Locations.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/Locations.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/Properties.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/Properties.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/ProxyFile.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/ProxyFile.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/ProxyInfo.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/ProxyInfo.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/VOMS.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/VOMS.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/VOMSService.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/VOMSService.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509CRL.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509CRL.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509Certificate.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509Certificate.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509Chain.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509Chain.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/X509Request.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/X509Request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/m2crypto/asn1_utils.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/m2crypto/asn1_utils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/Test_X509Certificate.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/Test_X509Certificate.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/Test_X509Chain.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/Test_X509Chain.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/Test_X509Request.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/Test_X509Request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/b236481c.0` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/b236481c.0`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/ca.cert.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/ca.cert.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/ca.key.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/ca.key.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/1000.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/1000.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/1001.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/1001.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/newcerts/1002.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/newcerts/1002.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/ca/openssl_config_ca.cnf` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/ca/openssl_config_ca.cnf`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/hostcert.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/hostcert.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/hostkey.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/hostkey.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/hostkey.pem.bak` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/hostkey.pem.bak`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/openssl_config_host.cnf` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/openssl_config_host.cnf`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/host/request.csr.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/host/request.csr.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/key/encrypted_key_pass_0000.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/key/encrypted_key_pass_0000.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/openssl_config_user.cnf` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/openssl_config_user.cnf`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/request.csr.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/request.csr.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/usercert.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/usercert.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/user/userkey.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/user/userkey.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/certs/voms/proxy.pem` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/certs/voms/proxy.pem`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Security/test/x509TestUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Security/test/x509TestUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/ClientSelector.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/ClientSelector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/TornadoClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/TornadoClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Client/private/TornadoBaseClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Client/private/TornadoBaseClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/HandlerManager.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/HandlerManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/TornadoREST.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/TornadoREST.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/TornadoServer.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/TornadoServer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/TornadoService.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/TornadoService.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/Server/private/BaseRequestHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/Server/private/BaseRequestHandler.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from datetime import datetime
 
 from http import HTTPStatus
 from urllib.parse import unquote
 from functools import partial
 
 import jwt
-import tornado
 from tornado.web import RequestHandler, HTTPError
 from tornado.ioloop import IOLoop
 
 import DIRAC
 
 from DIRAC import gConfig, gLogger, S_OK, S_ERROR
 from DIRAC.Core.Utilities import DErrno
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/scripts/tornado_start_CS.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/scripts/tornado_start_CS.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Tornado/scripts/tornado_start_all.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Tornado/scripts/tornado_start_all.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Adler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Adler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ClassAd/ClassAdLight.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ClassAd/ClassAdLight.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/CountryMapping.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/CountryMapping.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DAG.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DAG.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DEncode.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DEncode.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DErrno.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DErrno.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DIRACSingleton.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DIRACSingleton.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Decorators.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Decorators.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Devloader.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Devloader.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DictCache.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DictCache.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Dictionaries.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Dictionaries.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/DirectoryExplorer.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ElasticSearchDB.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ElasticSearchDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/EventDispatcher.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/EventDispatcher.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ExecutorDispatcher.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ExecutorDispatcher.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Extensions.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Extensions.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/File.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/File.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Glue2.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Glue2.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/BarGraph.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/BarGraph.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/CurveGraph.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/CurveGraph.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Dwatermark.png` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Dwatermark.png`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Graph.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Graph.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/GraphData.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/GraphData.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/GraphUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/GraphUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Legend.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Legend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/LineGraph.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/LineGraph.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/Palette.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/Palette.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/PieGraph.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/PieGraph.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/PlotBase.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/PlotBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/QualityMapGraph.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/QualityMapGraph.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Graphs/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Graphs/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Grid.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Grid.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from DIRAC.FrameworkSystem.Client.ProxyManagerClient import gProxyManager
 from DIRAC.Core.Security.ProxyInfo import getProxyInfo
 from DIRAC.ConfigurationSystem.Client.Helpers import Local
 from DIRAC.Core.Utilities.ReturnValues import S_OK, S_ERROR
 from DIRAC.Core.Utilities.Subprocess import systemCall, shellCall
 
 
-def executeGridCommand(proxy, cmd, gridEnvScript=None):
+def executeGridCommand(proxy, cmd, gridEnvScript=None, gridEnvDict=None):
     """
     Execute cmd tuple after sourcing GridEnv
     """
     currentEnv = dict(os.environ)
 
     if not gridEnvScript:
         # if not passed as argument, use default from CS Helpers
@@ -49,14 +49,17 @@
             return S_ERROR("Can not treat proxy passed as a string")
     else:
         ret = gProxyManager.dumpProxyToFile(proxy)
         if not ret["OK"]:
             return ret
         gridEnv["X509_USER_PROXY"] = ret["Value"]
 
+    if gridEnvDict:
+        gridEnv.update(gridEnvDict)
+
     result = systemCall(120, cmd, env=gridEnv)
     return result
 
 
 def ldapsearchBDII(filt=None, attr=None, host=None, base=None, selectionString="Glue"):
     """Python wrapper for ldapserch at bdii.
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/JDL.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/JDL.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/JEncode.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/JEncode.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/List.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/List.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/LockRing.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/LockRing.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/MJF.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/MJF.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Mail.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Mail.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/MixedEncode.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/MixedEncode.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/MySQL.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/MySQL.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Network.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Network.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ObjectLoader.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ObjectLoader.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Os.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Os.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Pfn.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Pfn.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Platform.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Platform.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/DataCache.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/DataCache.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/FileCoding.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/FileCoding.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/Plots.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/Plots.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Plotting/TypeLoader.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Plotting/TypeLoader.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/PrettyPrint.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/PrettyPrint.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ProcessPool.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ProcessPool.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Profiler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Profiler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/PromptUser.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/PromptUser.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Proxy.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Proxy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ReturnValues.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ReturnValues.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ServerUtils.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ServerUtils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Shifter.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Shifter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/SiteSEMapping.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/SiteSEMapping.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/StateMachine.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/StateMachine.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Subprocess.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Subprocess.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ThreadPool.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ThreadPool.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ThreadSafe.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ThreadSafe.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/ThreadScheduler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/ThreadScheduler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/TimeUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/TimeUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/Version.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/Version.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Adler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Adler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_DAG.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_DAG.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Decorator.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Decorator.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Dictionaries.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Dictionaries.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Encode.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Encode.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ExecutorDispatcher.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ExecutorDispatcher.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Extensions.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Extensions.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_File.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_File.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_List.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_List.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Mail.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Mail.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Network.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Network.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ObjectLoader.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ObjectLoader.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Pfn.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Pfn.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ProcessPool.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ProcessPool.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Profiler.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Profiler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_ReturnValues.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_ReturnValues.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Subprocess.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Subprocess.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Utilities/test/Test_Time.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Utilities/test/Test_Time.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Module.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Module.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Parameter.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Parameter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Step.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Step.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Utility.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Utility.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/Workflow.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/WorkflowReader.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/WorkflowReader.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/JobSamples.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/JobSamples.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/ModulesSamples.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/ModulesSamples.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/WFSamples.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/WFSamples.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/Workflow/test/step_g.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/Workflow/test/step_g.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_agent.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_agent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_cert_convert.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_cert_convert.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_configure.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_configure.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_executor.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_executor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_install_db.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_install_db.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_install_web_portal.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_install_web_portal.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_platform.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_platform.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_service.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_service.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_setup_site.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_setup_site.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/dirac_version.py` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/dirac_version.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Core/scripts/install_full.cfg` & `DIRAC-8.1.0a9/src/DIRAC/Core/scripts/install_full.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/FTS3Agent.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/FTS3Agent.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 .. literalinclude:: ../ConfigTemplate.cfg
   :start-after: ##BEGIN FTS3Agent
   :end-before: ##END FTS3Agent
   :dedent: 2
   :caption: FTS3Agent options
 
 """
+import datetime
 import errno
+import os
+from urllib import parse
 import time
 
 # from threading import current_thread
 from multiprocessing.pool import ThreadPool
 
 # We use the dummy module because we use the ThreadPool
 from multiprocessing.dummy import current_process
@@ -48,14 +51,18 @@
 PROXY_LIFETIME = 43200  # 12 hours
 
 # Instead of querying many jobs at once,
 # which maximizes the possibility of race condition
 # when running multiple agents, we rather do it in steps
 JOB_MONITORING_BATCH_SIZE = 20
 
+# We do not monitor a job more often
+# than MONITORING_DELAY in minutes
+MONITORING_DELAY = 10
+
 
 class FTS3Agent(AgentModule):
     """
     This Agent is responsible of interacting with the FTS3 services.
     Several of them can run in parallel.
     It first treats the Operations, by creating new FTS jobs and performing
     callback.
@@ -104,14 +111,16 @@
         :return: S_OK()/S_ERROR()
         """
         self._globalContextCache = {}
 
         # name that will be used in DB for assignment tag
         self.assignmentTag = gethostname().split(".")[0]
 
+        self.workDirectory = self.am_getWorkDirectory()
+
         res = self.__readConf()
 
         # We multiply by two because of the two threadPools
         self.fts3db = FTS3DB(pool_size=2 * self.maxNumberOfThreads)
 
         self.jobsThreadPool = ThreadPool(self.maxNumberOfThreads)
         self.opsThreadPool = ThreadPool(self.maxNumberOfThreads)
@@ -161,21 +170,27 @@
             if not res["OK"]:
                 return res
             # We take the first DN returned
             userDN = res["Value"][0]
 
             log.debug(f"UserDN {userDN}")
 
+            # Chose a meaningful proxy name for easier debugging
+            srvName = parse.urlparse(ftsServer).netloc.split(":")[0]
+            proxyFile = os.path.join(
+                self.workDirectory, f"{int(time.time())}_{username}_{group}_{srvName}_{threadID}.pem"
+            )
+
             # We dump the proxy to a file.
             # It has to have a lifetime of self.proxyLifetime
             # Because the FTS3 servers cache it for 2/3rd of the lifetime
             # we should make our cache a bit less than 2/3rd of the lifetime
             cacheTime = int(2 * self.proxyLifetime / 3) - 600
             res = gProxyManager.downloadVOMSProxyToFile(
-                userDN, group, requiredTimeLeft=self.proxyLifetime, cacheTime=cacheTime
+                userDN, group, requiredTimeLeft=self.proxyLifetime, cacheTime=cacheTime, filePath=proxyFile
             )
             if not res["OK"]:
                 return res
 
             proxyFile = res["Value"]
             log.debug(f"Proxy file {proxyFile}")
 
@@ -285,26 +300,37 @@
         log.debug(f"Size of the context cache {len(self._globalContextCache)}")
 
         # Find the number of loops
         nbOfLoops, mod = divmod(self.jobBulkSize, JOB_MONITORING_BATCH_SIZE)
         if mod:
             nbOfLoops += 1
 
+        # Not only is it pointless to monitor right after submission
+        # but also we would end up fetching multiple time the same job otherwise
+        # as we call getActiveJobs by batch
+        lastMonitor = datetime.datetime.utcnow() - datetime.timedelta(minutes=MONITORING_DELAY)
+
         log.debug("Getting active jobs")
 
         for loopId in range(nbOfLoops):
             log.info("Getting next batch of jobs to monitor", f"{loopId}/{nbOfLoops}")
             # get jobs from DB
-            res = self.fts3db.getActiveJobs(limit=JOB_MONITORING_BATCH_SIZE, jobAssignmentTag=self.assignmentTag)
+            res = self.fts3db.getActiveJobs(
+                limit=JOB_MONITORING_BATCH_SIZE, lastMonitor=lastMonitor, jobAssignmentTag=self.assignmentTag
+            )
 
             if not res["OK"]:
                 log.error("Could not retrieve ftsJobs from the DB", res)
                 return res
 
             activeJobs = res["Value"]
+            if not activeJobs:
+                log.info("No more jobs to monitor")
+                break
+
             log.info("Jobs queued for monitoring", len(activeJobs))
 
             # We store here the AsyncResult object on which we are going to wait
             applyAsyncResults = []
 
             # Starting the monitoring threads
             for ftsJob in activeJobs:
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ArchiveFiles.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ArchiveFiles.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/CheckMigration.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/CheckMigration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/DMSRequestOperationsBase.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/DMSRequestOperationsBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/MoveReplica.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/MoveReplica.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PhysicalRemoval.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PhysicalRemoval.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PutAndRegister.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/PutAndRegister.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReTransfer.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReTransfer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterFile.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterFile.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterReplica.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RegisterReplica.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,22 +51,25 @@
 
         if self.rmsMonitoring:
             self.rmsMonitoringReporter.addRecord(self.createRMSRecord("Attempted", len(waitingFiles)))
 
         # # loop over files
         registerOperations = {}
         successReplicas = 0
+
+        targetSE = self.operation.targetSEList[0]
+        replicaTuples = [(opFile.LFN, opFile.PFN, targetSE) for opFile in waitingFiles]
+
+        registerReplica = self.dm.registerReplica(replicaTuples, catalogs)
+
         for opFile in waitingFiles:
             # # get LFN
             lfn = opFile.LFN
             # # and others
-            targetSE = self.operation.targetSEList[0]
-            replicaTuple = (lfn, opFile.PFN, targetSE)
-            # # call ReplicaManager
-            registerReplica = self.dm.registerReplica(replicaTuple, catalogs)
+
             # # check results
             if not registerReplica["OK"] or lfn in registerReplica["Value"]["Failed"]:
                 # There have been some errors
 
                 if self.rmsMonitoring:
                     self.rmsMonitoringReporter.addRecord(self.createRMSRecord("Failed", 1))
                 #        self.dataLoggingClient().addFileRecord( lfn, "RegisterReplicaFail", ','.join( catalogs ) if catalogs else "all catalogs", "", "RegisterReplica" )
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveFile.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveFile.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveReplica.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveReplica.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReplicateAndRegister.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReplicateAndRegister.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,38 +42,47 @@
 from DIRAC.DataManagementSystem.private.FTS3Utilities import getFTS3Plugin
 
 from DIRAC.ConfigurationSystem.Client.Helpers import Registry
 
 from DIRAC.MonitoringSystem.Client.MonitoringReporter import MonitoringReporter
 
 
-def filterReplicas(opFile, logger=None, dataManager=None, opSources=None):
-    """filter out banned/invalid source SEs"""
+def filterReplicas(opFile, logger=None, dataManager=None, opSources=None, activeReplicas=None):
+    """filter out banned/invalid source SEs
+
+    :param list opSources: list of SE names to which limit the possible sources
+    :param dict activeReplicas: the result of dm.getActiveReplicas(*)["Value"]. Used as a cache
+
+    :returns: Valid list of SEs valid as source
+
+    """
 
     if logger is None:
         logger = gLogger
     if dataManager is None:
         dataManager = DataManager()
 
     log = logger.getSubLogger("filterReplicas")
     result = defaultdict(list)
 
-    replicas = dataManager.getActiveReplicas(opFile.LFN, getUrl=False, preferDisk=True)
-    if not replicas["OK"]:
-        log.error("Failed to get active replicas", replicas["Message"])
-        return replicas
+    if not activeReplicas:
+        res = dataManager.getActiveReplicas(opFile.LFN, getUrl=False, preferDisk=True)
+        if not res["OK"]:
+            log.error("Failed to get active replicas", res["Message"])
+            return res
+        activeReplicas = res["Value"]
+
     reNotExists = re.compile(r".*such file.*")
-    replicas = replicas["Value"]
-    failed = replicas["Failed"].get(opFile.LFN, "")
+    failed = activeReplicas["Failed"].get(opFile.LFN, "")
     if reNotExists.match(failed.lower()):
         opFile.Status = "Failed"
         opFile.Error = failed
         return S_ERROR(failed)
 
-    replicas = replicas["Successful"].get(opFile.LFN, {})
+    replicas = activeReplicas["Successful"].get(opFile.LFN, {})
 
     # If user set sourceSEs, only consider those replicas
     if opSources:
         replicas = {x: y for (x, y) in replicas.items() if x in opSources}
 
     noReplicas = False
     if not replicas:
@@ -171,14 +180,43 @@
         """call me maybe"""
 
         # The flag  'rmsMonitoring' is set by the RequestTask and is False by default.
         # Here we use 'createRMSRecord' to create the ES record which is defined inside OperationHandlerBase.
         if self.rmsMonitoring:
             self.rmsMonitoringReporter = MonitoringReporter(monitoringType="RMSMonitoring")
 
+        sourceSE = self.operation.SourceSE if self.operation.SourceSE else None
+        if sourceSE:
+            # check sourceSE for read
+            bannedSource = self.checkSEsRSS(sourceSE, "ReadAccess")
+            if not bannedSource["OK"]:
+                if self.rmsMonitoring:
+                    for status in ["Attempted", "Failed"]:
+                        self.rmsMonitoringReporter.addRecord(self.createRMSRecord(status, len(self.operation)))
+                    self.rmsMonitoringReporter.commit()
+                return bannedSource
+
+            if bannedSource["Value"]:
+                self.operation.Error = f"SourceSE {sourceSE} is banned for reading"
+                self.log.info(self.operation.Error)
+                return S_OK(self.operation.Error)
+
+        # check targetSEs for write
+        bannedTargets = self.checkSEsRSS()
+        if not bannedTargets["OK"]:
+            if self.rmsMonitoring:
+                for status in ["Attempted", "Failed"]:
+                    self.rmsMonitoringReporter.addRecord(self.createRMSRecord(status, len(self.operation)))
+                self.rmsMonitoringReporter.commit()
+            return bannedTargets
+
+        if bannedTargets["Value"]:
+            self.operation.Error = f"{','.join(bannedTargets['Value'])} targets are banned for writing"
+            return S_OK(self.operation.Error)
+
         # # check replicas first
         checkReplicas = self.__checkReplicas()
         if not checkReplicas["OK"]:
             self.log.error("Failed to check replicas", checkReplicas["Message"])
         if hasattr(self, "FTSMode") and getattr(self, "FTSMode"):
             bannedGroups = getattr(self, "FTSBannedGroups") if hasattr(self, "FTSBannedGroups") else ()
             if self.request.OwnerGroup in bannedGroups:
@@ -249,17 +287,23 @@
                 opFileToSchedule.ChecksumType = metadata[lfn]["ChecksumType"]
             opFileToSchedule.Size = metadata[lfn]["Size"]
 
             filesToSchedule[opFileToSchedule.LFN] = opFileToSchedule
 
         return S_OK(filesToSchedule)
 
-    def _filterReplicas(self, opFile):
+    def _filterReplicas(self, opFile, activeReplicas):
         """filter out banned/invalid source SEs"""
-        return filterReplicas(opFile, logger=self.log, dataManager=self.dm, opSources=self.operation.sourceSEList)
+        return filterReplicas(
+            opFile,
+            logger=self.log,
+            dataManager=self.dm,
+            opSources=self.operation.sourceSEList,
+            activeReplicas=activeReplicas,
+        )
 
     def _checkExistingFTS3Operations(self):
         """
         Check if there are ongoing FTS3Operation for the current RMS Operation
 
         Under some conditions, we can be trying to schedule files while
         there is still an FTS transfer going on. This typically happens
@@ -338,21 +382,30 @@
 
         # Dict which maps the FileID to the object
         rmsFilesIds = {}
 
         if self.rmsMonitoring:
             self.rmsMonitoringReporter.addRecord(self.createRMSRecord("Attempted", len(self.getWaitingFilesList())))
 
-        for opFile in self.getWaitingFilesList():
+        waitingFiles = self.getWaitingFilesList()
+
+        allLFNs = [opFile.LFN for opFile in waitingFiles]
+        res = self.dm.getActiveReplicas(allLFNs, getUrl=False, preferDisk=True)
+        if not res["OK"]:
+            self.log.error("Failed to get active replicas", res["Message"])
+            return res
+        allActiveReplicas = res["Value"]
+
+        for opFile in waitingFiles:
             rmsFilesIds[opFile.FileID] = opFile
 
             opFile.Error = ""
 
             # # check replicas
-            replicas = self._filterReplicas(opFile)
+            replicas = self._filterReplicas(opFile, allActiveReplicas)
             if not replicas["OK"]:
                 continue
             replicas = replicas["Value"]
 
             validReplicas = replicas["Valid"]
             noMetaReplicas = replicas["NoMetadata"]
             noReplicas = replicas["NoReplicas"]
@@ -452,44 +505,14 @@
             self.rmsMonitoringReporter.commit()
 
         # Just in case some transfers could not be scheduled, try them with RM
         return self.dmTransfer(fromFTS=True)
 
     def dmTransfer(self, fromFTS=False):
         """replicate and register using dataManager"""
-        # # get waiting files. If none just return
-        # # source SE
-        sourceSE = self.operation.SourceSE if self.operation.SourceSE else None
-        if sourceSE:
-            # # check source se for read
-            bannedSource = self.checkSEsRSS(sourceSE, "ReadAccess")
-            if not bannedSource["OK"]:
-                if self.rmsMonitoring:
-                    for status in ["Attempted", "Failed"]:
-                        self.rmsMonitoringReporter.addRecord(self.createRMSRecord(status, len(self.operation)))
-                    self.rmsMonitoringReporter.commit()
-                return bannedSource
-
-            if bannedSource["Value"]:
-                self.operation.Error = f"SourceSE {sourceSE} is banned for reading"
-                self.log.info(self.operation.Error)
-                return S_OK(self.operation.Error)
-
-        # # check targetSEs for write
-        bannedTargets = self.checkSEsRSS()
-        if not bannedTargets["OK"]:
-            if self.rmsMonitoring:
-                for status in ["Attempted", "Failed"]:
-                    self.rmsMonitoringReporter.addRecord(self.createRMSRecord(status, len(self.operation)))
-                self.rmsMonitoringReporter.commit()
-            return bannedTargets
-
-        if bannedTargets["Value"]:
-            self.operation.Error = f"{','.join(bannedTargets['Value'])} targets are banned for writing"
-            return S_OK(self.operation.Error)
 
         # Can continue now
         self.log.verbose("No targets banned for writing")
 
         waitingFiles = self.getWaitingFilesList()
         if not waitingFiles:
             return S_OK()
@@ -500,29 +523,36 @@
             self.log.info("Transferring files using Data manager...")
         errors = defaultdict(int)
         delayExecution = 0
 
         if self.rmsMonitoring:
             self.rmsMonitoringReporter.addRecord(self.createRMSRecord("Attempted", len(waitingFiles)))
 
+        allLFNs = [opFile.LFN for opFile in waitingFiles]
+        res = self.dm.getActiveReplicas(allLFNs, getUrl=False, preferDisk=True)
+        if not res["OK"]:
+            self.log.error("Failed to get active replicas", res["Message"])
+            return res
+        allActiveReplicas = res["Value"]
+
         for opFile in waitingFiles:
             if opFile.Error in (
                 "Couldn't get metadata",
                 "File doesn't exist",
                 "No active replica found",
                 "All replicas have a bad checksum",
             ):
                 err = "File already in error status"
                 errors[err] += 1
 
             opFile.Error = ""
             lfn = opFile.LFN
 
             # Check if replica is at the specified source
-            replicas = self._filterReplicas(opFile)
+            replicas = self._filterReplicas(opFile, allActiveReplicas)
             if not replicas["OK"]:
                 self.log.error("Failed to check replicas", replicas["Message"])
                 continue
             replicas = replicas["Value"]
             validReplicas = replicas.get("Valid")
             noMetaReplicas = replicas.get("NoMetadata")
             noReplicas = replicas.get("NoReplicas")
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/StagingCallback.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/StagingCallback.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ArchiveFiles.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ArchiveFiles.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_CheckMigration.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_CheckMigration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_RequestOperations.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_RequestOperations.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/AbstractFileSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/AbstractFileSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/DirectoryCompletion.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/CmdDirCompletion/DirectoryCompletion.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/ConsistencyInspector.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/ConsistencyInspector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/DataIntegrityClient.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/DataIntegrityClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/DataManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/DataManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/DirectoryListing.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/DirectoryListing.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3Client.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3Client.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3File.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3File.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3Job.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3Job.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FTS3Operation.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FTS3Operation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FailoverTransfer.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FailoverTransfer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/FileCatalogClientCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/FileCatalogClientCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/MetaQuery.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/MetaQuery.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/S3GatewayClient.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/S3GatewayClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/Test_Client_DataManagementSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/Test_FTS3Objects.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/Test_FTS3Objects.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/mock_DM.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/mock_DM.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Client/test/new_dir_completion.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Client/test/new_dir_completion.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/DataIntegrityDB.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/DataIntegrityDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FTS3DB.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FTS3DB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/DatasetManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DatasetManager/DatasetManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryClosure.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryClosure.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryFlatTree.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryFlatTree.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryLevelTree.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryLevelTree.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryNodeTree.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryNodeTree.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectorySimpleTree.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectorySimpleTree.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryTreeBase.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryManager/DirectoryTreeBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/DirectoryMetadata.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/DirectoryMetadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/MultiVODirectoryMetadata.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/DirectoryMetadata/MultiVODirectoryMetadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerBase.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerFlat.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerFlat.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerPs.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileManager/FileManagerPs.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/FileMetadata.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/FileMetadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/MultiVOFileMetadata.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/FileMetadata/MultiVOFileMetadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerBase.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerDB.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SEManager/SEManagerDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManagerWithDelete.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/DirectorySecurityManagerWithDelete.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/FullSecurityManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/FullSecurityManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/NoSecurityManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/NoSecurityManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/SecurityManagerBase.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/SecurityManagerBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/VOMSSecurityManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/VOMSSecurityManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/test/Test_VOMSSecurityManager.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/SecurityManager/test/Test_VOMSSecurityManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerBase.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerCS.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerCS.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerDB.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/UserGroupManager/UserAndGroupManagerDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/test/Test_DataManagement_FileCatalogComponents.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogComponents/test/Test_DataManagement_FileCatalogComponents.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/FileCatalogWithFkAndPsDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/FileCatalogWithFkAndPsDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/DB/test/Test_FTS3DB.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/DB/test/Test_FTS3DB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/DataIntegrityHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/DataIntegrityHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/FTS3ManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/FTS3ManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/FileCatalogHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/FileCatalogHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/S3GatewayHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/S3GatewayHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/StorageElementHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/StorageElementHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/TornadoDataIntegrityHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/TornadoDataIntegrityHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Service/TornadoFileCatalogHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Service/TornadoFileCatalogHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/DMSHelpers.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/DMSHelpers.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/ResolveSE.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/ResolveSE.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/Utilities/test/Test_resolveSE.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/Utilities/test/Test_resolveSE.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/DefaultFTS3Plugin.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/DefaultFTS3Plugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Plugins/test/Test_DefaultFTS3Plugin.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Plugins/test/Test_DefaultFTS3Plugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/FTS3Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/FTS3Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/HttpStorageAccessHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/HttpStorageAccessHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/private/test/Test_FTS3Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/private/test/Test_FTS3Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_admin_allow_se.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_admin_allow_se.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_admin_ban_se.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_admin_ban_se.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_admin_user_quota.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_admin_user_quota.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_add_file.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_catalog_metadata.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_catalog_metadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_change_replica_status.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_change_replica_status.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_clean_directory.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_clean_directory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_archive_request.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_archive_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_moving_request.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_moving_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_removal_request.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_create_removal_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_data_size.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_data_size.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_directory_sync.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_directory_sync.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_find_lfns.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_find_lfns.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_move_replica_request.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_move_replica_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_protocol_matrix.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_protocol_matrix.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_put_and_register_request.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_put_and_register_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_files.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_files.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_replicas.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_catalog_replicas.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_files.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_remove_replicas.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replica_metadata.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replica_metadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replicate_and_register_request.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_replicate_and_register_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_resolve_guid.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_resolve_guid.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_set_replica_status.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_set_replica_status.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_show_se_status.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_show_se_status.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_lfns.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_lfns.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_quota.py` & `DIRAC-8.1.0a9/src/DIRAC/DataManagementSystem/scripts/dirac_dms_user_quota.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/API/AuthHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/API/AuthHandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -413,32 +413,36 @@
           {
             "error": "authorization_pending"
           }
         """
         return self.server.create_token_response(self.request)
 
     def __researchDIRACGroup(self, extSession, chooseScope, state):
-        """Research DIRAC groups for authorized user
+        """Look for DIRAC groups of a user already authorized by an Identity Provider
 
         :param dict extSession: ended authorized external IdP session
 
         :return: -- will return (None, response) to provide error or group selector
-                    will return (grant_user, request) to contionue authorization with choosed group
+                    will return (grant_user, request) to continue authorization with chosen group
         """
         # Base DIRAC client auth session
         firstRequest = createOAuth2Request(extSession["firstRequest"])
         # Read requested groups by DIRAC client or user
         firstRequest.addScopes(chooseScope)
         # Read already authed user
         username = extSession["authed"]["username"]
         # Requested arguments in first request
         provider = firstRequest.provider
-        self.log.debug(f"Next groups has been found for {username}:", ", ".join(firstRequest.groups))
+        self.log.debug("The following groups found", f"for {username}: {', '.join(firstRequest.groups)}")
 
-        # Researche Group
+        # If group is already defined in the first request, just return it as it was already validated
+        if firstRequest.groups:
+            return extSession["authed"], firstRequest
+
+        # Look for DIRAC groups valid for the user
         result = getGroupsForUser(username)
         if not result["OK"]:
             return None, self.server.handle_response(
                 payload=getHTML("server error", theme="error", info=result["Message"]), delSession=True
             )
         groups = result["Value"]
 
@@ -453,24 +457,20 @@
                     info=f"No groups found for {username} and for {provider} Identity Provider.",
                 ),
                 delSession=True,
             )
 
         self.log.debug(f"The state of {username} user groups has been checked:", pprint.pformat(validGroups))
 
-        # If group already defined in first request, just return it
-        if firstRequest.groups:
-            return extSession["authed"], firstRequest
-
         # If not and we found only one valid group, apply this group
         if len(validGroups) == 1:
             firstRequest.addScopes([f"g:{validGroups[0]}"])
             return extSession["authed"], firstRequest
 
-        # Else give user chanse to choose group in browser
+        # Else give user a chance to choose a group in the browser
         with dom.div(cls="row mt-5 justify-content-md-center align-items-center") as tag:
             for group in sorted(validGroups):
                 vo, gr = group.split("_")
                 with dom.div(cls="col-auto p-2").add(dom.div(cls="card shadow-lg border-0 text-center p-2")):
                     dom.h4(vo.upper() + " " + gr, cls="p-2")
                     dom.a(href=f"{self.currentPath}?state={state}&chooseScope=g:{group}", cls="stretched-link")
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/ComponentSupervisionAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/ComponentSupervisionAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/ProxyRenewalAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/ProxyRenewalAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Agent/test/Test_ComponentSupervisionAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Agent/test/Test_ComponentSupervisionAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/BundleDeliveryClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/BundleDeliveryClient.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     """Get hash for bundle in directory
 
     :param str bundleID: bundle ID
     :param str dirToSyncTo: path to sync directory
 
     :return: str
     """
+    bundle_path = os.path.join(dirToSyncTo, f".dab.{bundleID}")
+    if not os.path.isfile(bundle_path):
+        return ""
     try:
         with open(os.path.join(dirToSyncTo, f".dab.{bundleID}"), "rb") as fd:
             bdHash = fd.read().strip()
             return bdHash.decode()
     except OSError as e:
         gLogger.exception("File can't be open/read, returning empty string", lException=e)
         return ""
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ComponentInstaller.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ComponentInstaller.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/NotificationClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/NotificationClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ProxyGeneration.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ProxyGeneration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ProxyManagerClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ProxyManagerClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/ProxyUpload.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/ProxyUpload.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SecurityLogClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SecurityLogClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClientCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SystemAdministratorClientCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/SystemAdministratorIntegrator.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/SystemAdministratorIntegrator.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/TokenManagerClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/TokenManagerClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 from DIRAC import S_OK, S_ERROR
 from DIRAC.Core.Utilities import ThreadSafe
 from DIRAC.Core.Utilities.DictCache import DictCache
 from DIRAC.Core.Base.Client import Client, createClient
 from DIRAC.ConfigurationSystem.Client.Helpers import Registry
 from DIRAC.Resources.IdProvider.IdProviderFactory import IdProviderFactory
+from DIRAC.FrameworkSystem.private.authorization.utils.Tokens import OAuth2Token
 
 gTokensSync = ThreadSafe.Synchronizer()
 
 
 @createClient("Framework/TokenManager")
 class TokenManagerClient(Client):
     """Client exposing the TokenManager Service."""
@@ -29,15 +30,15 @@
         username: str,
         userGroup: str = None,
         scope: str = None,
         audience: str = None,
         identityProvider: str = None,
         requiredTimeLeft: int = 0,
     ):
-        """Get an access token for a user/group.
+        """Get an access token for a user/group keeping the local cache
 
         :param username: user name
         :param userGroup: group name
         :param scope: scope
         :param audience: audience
         :param identityProvider: identity Provider
         :param requiredTimeLeft: required time
@@ -51,40 +52,39 @@
 
         # prepare the client instance of the appropriate IdP
         result = self.idps.getIdProvider(identityProvider)
         if not result["OK"]:
             return result
         idpObj = result["Value"]
 
-        if userGroup and (result := idpObj.getGroupScopes(userGroup))["OK"]:
+        if userGroup and (result := idpObj.getGroupScopes(userGroup)):
             # What scope correspond to the requested group?
-            scope = list(set((scope or []) + result["Value"]))
+            scope = list(set((scope or []) + result))
 
         # Set the scope
         idpObj.scope = " ".join(scope)
 
         # Let's check if there are corresponding tokens in the cache
         cacheKey = (username, idpObj.scope, audience, identityProvider)
         if self.__tokensCache.exists(cacheKey, requiredTimeLeft):
             # Well we have a fresh record containing a Token object
             token = self.__tokensCache.get(cacheKey)
             # Let's check if the access token is fresh
             if not token.is_expired(requiredTimeLeft):
                 return S_OK(token)
-            # It seems that it is no longer valid for us, but whether there is a refresh token?
-            if token.get("refresh_token"):
-                # Okay, so we can try to refresh tokens
-                if (result := idpObj.refreshToken(token["refresh_token"]))["OK"]:
-                    # caching new tokens
-                    self.__tokensCache.add(
-                        cacheKey,
-                        token.get_claim("exp", "refresh_token") or self.DEFAULT_RT_EXPIRATION_TIME,
-                        result["Value"],
-                    )
-                    return result
-                self.log.verbose(f"Failed to get token on client's side: {result['Message']}")
-                # Let's try to revoke broken token
-                idpObj.revokeToken(token["refresh_token"])
 
-        return self.executeRPC(
+        result = self.executeRPC(
             username, userGroup, scope, audience, identityProvider, requiredTimeLeft, call="getToken"
         )
+
+        if result["OK"]:
+            token = OAuth2Token(dict(result["Value"]))
+            self.__tokensCache.add(
+                cacheKey,
+                token.get_claim("exp", "refresh_token") or self.DEFAULT_RT_EXPIRATION_TIME,
+                token,
+            )
+
+        return result
+
+
+gTokenManager = TokenManagerClient()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Client/UserProfileClient.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Client/UserProfileClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/ConfigTemplate.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -135,26 +135,14 @@
       Default = authenticated
       FileTransfer
       {
         Default = authenticated
       }
     }
   }
-  TornadoBundleDelivery
-  {
-    Protocol = https
-    Authorization
-    {
-      Default = authenticated
-      FileTransfer
-      {
-        Default = authenticated
-      }
-    }
-  }
   Notification
   {
     Port = 9154
     SMSSwitch = sms.switch.ch
     Authorization
     {
       Default = AlarmsManagement
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/AuthDB.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/AuthDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/InstalledComponentsDB.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/InstalledComponentsDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/NotificationDB.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/NotificationDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/ProxyDB.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/ProxyDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/TokenDB.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/TokenDB.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 from DIRAC.FrameworkSystem.private.authorization.utils.Tokens import OAuth2Token
 
 
 Model = declarative_base()
 
 
 class Token(Model, OAuth2TokenMixin):
-    """This class describe token fields"""
+    """This class describes token fields"""
 
     __tablename__ = "Token"
     __table_args__ = {"mysql_engine": "InnoDB", "mysql_charset": "utf8"}
     # access_token too large for varchar(255)
     # 767 bytes is the stated prefix limitation for InnoDB tables in MySQL version 5.6
     # https://stackoverflow.com/questions/1827063/mysql-error-key-specification-without-a-key-length
     id = Column(Integer, autoincrement=True, primary_key=True)  # Unique token ID
     kid = Column(String(255))  # Unique secret key ID for token encryption
-    user_id = Column(String(255))  # User identificator that registred in an identity provider, token owner
-    provider = Column(String(255))  # Provider name registred in DIRAC
+    user_id = Column(String(255))  # User identifier registered in an identity provider, token owner
+    provider = Column(String(255))  # Provider name registered in DIRAC
     expires_at = Column(Integer, nullable=False, default=0)  # When the access token is expired
     access_token = Column(Text, nullable=False)
     refresh_token = Column(Text, nullable=False)
     rt_expires_at = Column(Integer, nullable=False, default=0)  # When the refresh token is expired
 
 
 class TokenDB(SQLAlchemyDB):
@@ -97,15 +97,15 @@
         :param userID: user ID (token owner)
         :param provider: provider name that issued the token
         :param rt_expired_in: refresh token expiration time, will be applied if the rt_expires_at value is missing
 
         :return: S_OK(list)/S_ERROR() -- return old tokens that should be revoked.
         """
         if not token["refresh_token"]:
-            return S_ERROR("Cannot store absent refresh token.")
+            return S_ERROR("Cannot store token without a refresh token.")
 
         # Let's collect the necessary attributes of the token
         token["user_id"] = userID
         token["provider"] = provider
         # If the expiration time of the token refresh is not specified, we will try to determine it
         if not token.get("rt_expires_at"):
             try:
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/DB/UserProfileDB.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/DB/UserProfileDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/BundleDeliveryHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/BundleDeliveryHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/ComponentMonitoringHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/ComponentMonitoringHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/NotificationHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/NotificationHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/ProxyManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/ProxyManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/SecurityLoggingHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/SecurityLoggingHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/SystemAdministratorHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/SystemAdministratorHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TokenManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TokenManagerHandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         """Get an access token for a user/group.
 
         * Properties:
             * FullDelegation <- permits full delegation of tokens
             * LimitedDelegation <- permits downloading only limited tokens
             * PrivateLimitedDelegation <- permits downloading only limited tokens for one self
 
-        :paarm username: user name
+        :param username: user name
         :param userGroup: user group
         :param scope: requested scope
         :param audience: requested audience
         :param identityProvider: Identity Provider name
         :param requiredTimeLeft: requested minimum life time
 
         :return: S_OK(dict)/S_ERROR()
@@ -206,72 +206,58 @@
 
         # prepare the client instance of the appropriate IdP
         result = self.idps.getIdProvider(identityProvider)
         if not result["OK"]:
             return result
         idpObj = result["Value"]
 
-        if userGroup and (result := idpObj.getGroupScopes(userGroup))["OK"]:
+        if userGroup and (result := idpObj.getGroupScopes(userGroup)):
             # What scope correspond to the requested group?
-            scope = list(set((scope or []) + result["Value"]))
+            scope = list(set((scope or []) + result))
 
         # Set the scope
         idpObj.scope = " ".join(scope)
 
-        # Let's check if there are corresponding tokens in the cache
+        # Let's check if there is a corresponding token in the cache
         cacheKey = (username, idpObj.scope, audience, identityProvider)
         if self.__tokensCache.exists(cacheKey, requiredTimeLeft):
             # Well we have a fresh record containing a Token object
             token = self.__tokensCache.get(cacheKey)
             # Let's check if the access token is fresh
             if not token.is_expired(requiredTimeLeft):
                 return S_OK(token)
-            # It seems that it is no longer valid for us, but whether there is a refresh token?
-            if token.get("refresh_token"):
-                # Okay, so we can try to refresh tokens
-                if (result := idpObj.refreshToken(token["refresh_token"]))["OK"]:
-                    # caching new tokens
-                    self.__tokensCache.add(
-                        cacheKey,
-                        result["Value"].get_claim("exp", "refresh_token") or self.DEFAULT_RT_EXPIRATION_TIME,
-                        result["Value"],
-                    )
-                    return result
-                self.log.verbose(f"Failed to get token with cached tokens: {result['Message']}")
-                # Let's try to revoke broken token
-                idpObj.revokeToken(token["refresh_token"])
 
         err = []
-        # The cache did not help, so let's make an exchange token
+        # No luck so far, let's refresh the token stored in the database
         result = Registry.getDNForUsername(username)
         if not result["OK"]:
             return result
         for dn in result["Value"]:
             # For backward compatibility, the user ID is written as DN. So let's check if this DN contains a user ID
             result = Registry.getIDFromDN(dn)
             if result["OK"]:
                 uid = result["Value"]
                 # To do this, first find the refresh token stored in the database with the maximum scope
                 result = self.__tokenDB.getTokenForUserProvider(uid, identityProvider)
                 if result["OK"] and result["Value"]:
                     idpObj.token = result["Value"]
                     result = self.__checkProperties(dn, userGroup)
                     if result["OK"]:
-                        # exchange token with requested scope
-                        result = idpObj.exchangeToken()
+                        # refresh token with requested scope
+                        result = idpObj.refreshToken()
                         if result["OK"]:
                             # caching new tokens
                             self.__tokensCache.add(
                                 cacheKey,
                                 result["Value"].get_claim("exp", "refresh_token") or self.DEFAULT_RT_EXPIRATION_TIME,
                                 result["Value"],
                             )
                             return result
-                # Not find any token associated with the found user ID
-                err.append(result.get("Message", f"No token found for {uid}."))
+                # Did not find any token associated with the found user ID
+                err.append(result.get("Message", f"No token found for {uid}"))
         # Collect all errors when trying to get a token, or if no user ID is registered
         return S_ERROR("; ".join(err or [f"No user ID found for {username}"]))
 
     def export_deleteToken(self, userDN: str):
         """Delete a token from the DB
 
         :param userDN: user DN
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoBundleDeliveryHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Service/TornadoMonitoringHandler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-""" Handler for CAs + CRLs bundles
+""" Tornado-based HTTPs Monitoring service.
+
+.. literalinclude:: ../ConfigTemplate.cfg
+  :start-after: ##BEGIN TornadoMonitoring
+  :end-before: ##END
+  :dedent: 2
+  :caption: Monitoring options
+
 """
-from base64 import b64encode
 
-from DIRAC import S_OK, S_ERROR
-from DIRAC.Core.Security import Utilities
+from DIRAC import S_ERROR
 from DIRAC.Core.Tornado.Server.TornadoService import TornadoService
-from DIRAC.FrameworkSystem.Service.BundleDeliveryHandler import BundleDeliveryHandlerMixin
+from DIRAC.Core.Utilities.Plotting import gDataCache
+from DIRAC.Core.Utilities.Plotting.Plots import generateErrorMessagePlot
+from DIRAC.MonitoringSystem.Service.MonitoringHandler import MonitoringHandlerMixin
 
 
-class TornadoBundleDeliveryHandler(BundleDeliveryHandlerMixin, TornadoService):
+class TornadoMonitoringHandler(MonitoringHandlerMixin, TornadoService):
     types_streamToClient = []
 
     def export_streamToClient(self, fileId):
-        version = ""
-        if isinstance(fileId, str):
-            if fileId in ["CAs", "CRLs"]:
-                retVal = Utilities.generateCAFile() if fileId == "CAs" else Utilities.generateRevokedCertsFile()
-                if not retVal["OK"]:
-                    return retVal
-                with open(retVal["Value"]) as fd:
-                    return S_OK(b64encode(fd.read()).decode())
-            bId = fileId
-
-        elif isinstance(fileId, (list, tuple)):
-            if len(fileId) == 0:
-                return S_ERROR("No bundle specified!")
-            bId = fileId[0]
-            if len(fileId) != 1:
-                version = fileId[1]
-
-        if not self.bundleManager.bundleExists(bId):
-            return S_ERROR(f"Unknown bundle {bId}")
-
-        bundleVersion = self.bundleManager.getBundleVersion(bId)
-        if bundleVersion is None:
-            return S_ERROR(f"Empty bundle {bId}")
+        """
+        Get graphs data
 
-        if version == bundleVersion:
-            return S_OK(bundleVersion)
+        :param str fileId: encoded plot attributes
+        """
 
-        return S_OK(b64encode(self.bundleManager.getBundleData(bId)).decode())
+        # First check if we've got to generate the plot
+        if len(fileId) > 5 and fileId[1] == ":":
+            self.log.info("Seems the file request is a plot generation request!")
+            try:
+                result = self._generatePlotFromFileId(fileId)
+            except Exception as e:  # pylint: disable=broad-except
+                self.log.exception("Exception while generating plot", str(e))
+                result = S_ERROR(f"Error while generating plot: {str(e)}")
+            if not result["OK"]:
+                return generateErrorMessagePlot(result["Message"])
+            fileId = result["Value"]
+
+        retVal = gDataCache.getPlotData(fileId)
+        if not retVal["OK"]:
+            return generateErrorMessagePlot(result["Message"])
+        return retVal["Value"]
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoComponentMonitoringHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoComponentMonitoringHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoProxyManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoProxyManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/TornadoUserProfileManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/TornadoUserProfileManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Service/UserProfileManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Service/UserProfileManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/Utilities/MonitoringUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/Utilities/MonitoringUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/SecurityFileLog.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/SecurityFileLog.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/AuthServer.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/AuthServer.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     def generateProxyOrToken(
         self, client, grant_type, user=None, scope=None, expires_in=None, include_refresh_token=True
     ):
         """Generate proxy or tokens after authorization
 
         :param client: instance of the IdP client
         :param grant_type: authorization grant type (unused)
-        :param str user: user identificator
+        :param str user: user identifier
         :param str scope: requested scope
         :param expires_in: when the token should expire (unused)
         :param bool include_refresh_token: to include refresh token (unused)
 
         :return: dict or str -- will return tokens as dict or proxy as string
         """
         # Read requested scopes
@@ -276,33 +276,33 @@
 
         :param dict response: authorization response
         :param str session: session
 
         :return: S_OK(dict)/S_ERROR()
         """
         providerName = session.pop("Provider")
-        sLog.debug(f"Try to parse authentification response from {providerName}:\n", pprint.pformat(response))
+        sLog.debug(f"Try to parse authentication response from {providerName}:\n", pprint.pformat(response))
         # Parse response
         result = self.idps.getIdProvider(providerName)
         if not result["OK"]:
             return result
         idpObj = result["Value"]
         result = idpObj.parseAuthResponse(response, session)
         if not result["OK"]:
             return result
 
         # FINISHING with IdP
         # As a result of authentication we will receive user credential dictionary
         credDict, payload = result["Value"]
 
         sLog.debug("Read profile:", pprint.pformat(credDict))
-        # Is ID registred?
+        # Is ID registered?
         result = getUsernameForDN(credDict["DN"])
         if not result["OK"]:
-            comment = f"ID {credDict['ID']} is not registred in DIRAC. "
+            comment = f"ID {credDict['ID']} is not registered in DIRAC. "
             payload.update(idpObj.getUserProfile().get("Value", {}))
             result = self.__registerNewUser(providerName, payload)
 
             if result["OK"]:
                 comment += "Administrators have been notified about you."
             else:
                 comment += "Please, contact the DIRAC administrators."
@@ -422,33 +422,33 @@
             self.db.removeSession(request.sessionID)
             sLog.exception(e)
             return self.handle_response(
                 payload=getHTML("server error", theme="error", body="traceback", info=repr(e)), delSession=True
             )
 
     def validateIdentityProvider(self, request, provider):
-        """Check if identity provider registred in DIRAC
+        """Check if identity provider registered in DIRAC
 
         :param object request: request
         :param str provider: provider name
 
         :return: OAuth2Request object or HTML -- new request with provider name or provider selector
         """
         if provider:
             request.provider = provider
 
         # Find identity provider for group
         groupProvider = getIdPForGroup(request.group) if request.groups else None
 
-        # If requested access token for group that is not registred in any identity provider
-        # or the requested provider does not match the group return error
+        # If access token is requested for a group that is not registered in any identity provider
+        # or the requested provider does not match the group, return error
         if request.group and not groupProvider and "proxy" not in request.scope:
             raise Exception(f"The {request.group} group belongs to the VO that is not tied to any Identity Provider.")
 
-        sLog.debug(f"Check if {request.provider} identity provider registred in DIRAC..")
+        sLog.debug(f"Check if {request.provider} identity provider registered in DIRAC...")
         # Research supported IdPs
         result = getProvidersForInstance("Id")
         if not result["OK"]:
             raise Exception(result["Message"])
 
         idPs = result["Value"]
         if not idPs:
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/AuthorizationCode.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/AuthorizationCode.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from authlib.jose import JsonWebSignature
 from authlib.oauth2.base import OAuth2Error
 from authlib.oauth2.rfc6749.grants import AuthorizationCodeGrant as _AuthorizationCodeGrant
 from authlib.common.encoding import json_b64encode, urlsafe_b64decode, json_loads
 
 
 class OAuth2Code(dict):
-    """This class describe Authorization Code object"""
+    """This class describes Authorization Code object"""
 
     def __init__(self, params):
         """C'or"""
         params["auth_time"] = params.get("auth_time", int(time()))
         super().__init__(params)
 
     @property
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/DeviceFlow.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/DeviceFlow.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/RefreshToken.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/RefreshToken.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/grants/RevokeToken.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/grants/RevokeToken.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Clients.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Clients.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Requests.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Requests.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Tokens.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Tokens.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/authorization/utils/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/authorization/utils/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/BaseFormatter.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/BaseFormatter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/ColoredBaseFormatter.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/ColoredBaseFormatter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/MicrosecondJsonFormatter.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Formatter/MicrosecondJsonFormatter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/MessageQueueHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Handler/MessageQueueHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/LogLevels.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/LogLevels.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/Logging.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/Logging.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/LoggingRoot.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/LoggingRoot.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/TestLogUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/TestLogUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LogLevels.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LogLevels.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LoggingRoot_ConfigForExternalLibs.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_LoggingRoot_ConfigForExternalLibs.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Backends.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Backends.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_CreationLogRecord.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_CreationLogRecord.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_FormatOptions.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_FormatOptions.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_GetSubLogger.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_GetSubLogger.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Levels.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/private/standardLogging/test/Test_Logging_Levels.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_CAs.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_CAs.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_proxy.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_get_proxy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_proxy_upload.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_proxy_upload.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_sysadmin_cli.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_sysadmin_cli.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_instance.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_instance.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_pilot.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_update_pilot.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_admin_users_with_proxy.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_admin_users_with_proxy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_install_component.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_install_component.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_install_tornado_service.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_install_tornado_service.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_login.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_login.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_logout.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_logout.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_populate_component_db.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_populate_component_db.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_destroy.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_destroy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_get_uploaded_info.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_get_uploaded_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_info.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_init.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_proxy_init.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_restart_component.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_restart_component.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_start_component.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_start_component.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_status_component.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_status_component.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_stop_component.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_stop_component.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_sys_sendmail.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_sys_sendmail.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/FrameworkSystem/scripts/dirac_uninstall_component.py` & `DIRAC-8.1.0a9/src/DIRAC/FrameworkSystem/scripts/dirac_uninstall_component.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/Dirac.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/Dirac.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/DiracAdmin.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/DiracAdmin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/Job.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/Job.py`

 * *Files 2% similar despite different names*

```diff
@@ -774,14 +774,38 @@
             return self._reportError("Expected string for job group name", **{"jobGroup": jobGroup})
 
         description = "User specified job group"
         self._addParameter(self.workflow, "JobGroup", "JDL", jobGroup, description)
         return S_OK()
 
     #############################################################################
+    def setPriority(self, priority):
+        """Helper function.
+
+        Sets the job priority in the range 1-10.
+        Priorities 1-9 are matched probabilistically with higher numbers being more likely.
+        Priority 10 jobs are always started before lower priority jobs from the same user.
+
+        Example usage:
+
+        >>> job = Job()
+        >>> job.setPriority(5)
+
+        :param priority: Job priority
+        :type priority: int
+        """
+        if not isinstance(priority, int):
+            return self._reportError("Expected int for priority", **{"priority": priority})
+
+        self.priority = priority
+        description = "User Job Priority"
+        self._addParameter(self.workflow, "Priority", "JDL", priority, description)
+        return S_OK()
+
+    #############################################################################
     def setLogLevel(self, logLevel):
         """Helper function.
 
         Optionally specify a DIRAC logging level for the job, e.g.
         ALWAYS, INFO, VERBOSE, WARN, DEBUG
         by default this is set to the info level.
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/Test_DIRAC.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/Test_DIRAC.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/Test_JobAPI.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/Test_JobAPI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/testWF.jdl` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/testWF.jdl`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/API/test/testWF.xml` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/API/test/testWF.xml`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/Utilities/DCommands.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/Utilities/DCommands.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,18 +153,18 @@
         self.__buildSectionsAliases()
 
     def bootstrapFile(self):
         if not os.path.exists(self.configDir):
             os.mkdir(self.configDir)
             os.chmod(self.configDir, stat.S_IRWXU)
         elif not os.path.isdir(self.configDir):
-            print(f'Error: "{self.configDir}" config dir is not a directory')
+            gLogger.error(f'"{self.configDir}" config dir is not a directory')
             DIRAC.exit(-1)
         elif not os.stat(self.configDir).st_mode != stat.S_IRWXU:
-            print(f'Error: "{self.configDir}" config dir doesn\'t have correct permissions')
+            gLogger.error(f'"{self.configDir}" config dir doesn\'t have correct permissions')
             DIRAC.exit(-1)
         if os.path.isfile(self.configPath):
             self.config.read(self.configPath)
 
     def __buildSectionsAliases(self):
         self.sectionsAliases = {}
         for section in self.config.sections():
@@ -315,15 +315,15 @@
 
         self.__cleanSessionDirectory()
 
         oldProfileName = self.getEnv("profile_name", "")["Value"]
         profileName = profileName or oldProfileName or self.origin.defaultProfile()
         retVal = self.origin.sectionAliasName(profileName)
         if not retVal["OK"]:
-            print("Error:", retVal["Message"])
+            gLogger.error(retVal["Message"])
             DIRAC.exit(-1)
         self.profileName = retVal["Value"]
 
         if not os.path.isfile(self.configPath) or self.profileName != oldProfileName:
             self.__clearEnv()
             # set default common options from section [global]
             self.copyProfile("global")
@@ -454,19 +454,17 @@
             gLogger.error("Your CRLs appear to be outdated, but you have no access to update them.")
             # Try to continue anyway...
             return S_OK()
         # Update the CAs & CRLs
         gLogger.notice("Your CRLs appear to be outdated; attempting to update them...")
         bdc = BundleDeliveryClient()
         res = bdc.syncCAs()
-        print(res)
         if not res["OK"]:
             gLogger.error("Failed to update CAs", res["Message"])
         res = bdc.syncCRLs()
-        print(res)
         if not res["OK"]:
             gLogger.error("Failed to update CRLs", res["Message"])
         # Continue even if the update failed...
         return S_OK()
 
     def proxyInit(self):
         params = ProxyGeneration.CLIParams()
@@ -576,15 +574,15 @@
                 # write to config
                 config.set(section, "default_se", defaultSESite)
 
 
 def sessionFromProxy(config=DConfig(), sessionDir=None):
     proxyPath = _getProxyLocation()
     if not proxyPath:
-        print("No proxy found")
+        gLogger.error("No proxy found")
         return None
 
     retVal = _getProxyInfo(proxyPath)
     if not retVal["OK"]:
         raise Exception(retVal["Message"])
 
     pi = retVal["Value"]
@@ -616,15 +614,15 @@
 
     return session
 
 
 def getDNFromProxy():
     proxyPath = _getProxyLocation()
     if not proxyPath:
-        print("No proxy found")
+        gLogger.error("No proxy found")
         return None
 
     retVal = _getProxyInfo(proxyPath)
     if not retVal["OK"]:
         return retVal
 
     pi = retVal["Value"]
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/Utilities/DConfigCache.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/Utilities/DConfigCache.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import re
 import stat
 import time
 import pickle
 import tempfile
 
+from DIRAC import gLogger
 from DIRAC.Core.Base.Script import Script
 from DIRAC.ConfigurationSystem.Client.ConfigurationData import gConfigurationData
 
 
 class ConfigCache:
     @classmethod
     def cacheFilePrefix(cls):
@@ -71,8 +72,8 @@
                 os.chmod(self.configCacheName, stat.S_IRUSR | stat.S_IWUSR)
                 pickle.dump(gConfigurationData.mergedCFG, fcache)
         else:
             try:
                 with open(self.configCacheName, "rb") as fh:
                     gConfigurationData.mergedCFG = pickle.load(fh)
             except:
-                print("Warning: Cache corrupt or unreadable")
+                gLogger.error("Cache corrupt or unreadable")
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dcd.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dcd.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,28 +27,28 @@
     configCache.cacheConfig()
 
     args = Script.getPositionalArgs()
 
     session = DSession()
 
     if len(args) > 1:
-        gLogger.notice(f"Error: too many arguments provided\n{Script.scriptName}:")
+        gLogger.notice(f"Too many arguments provided\n{Script.scriptName}:")
         Script.showHelp(exitCode=-1)
 
     if len(args):
         arg = pathFromArgument(session, args[0])
     else:
         arg = session.homeDir()
 
     catalog = DCatalog()
 
     if catalog.isDir(arg):
         if session.getCwd() != arg:
             session.setCwd(arg)
             session.write()
     else:
-        print(f'Error: "{arg}" not a valid directory')
+        gLogger.error(f'"{arg}" not a valid directory')
         DIRAC.exit(-1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dchgrp.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dchgrp.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 """
 Change file owner's group in file catalog.
 
 Examples:
     $ dchgrp atsareg ././some_lfn_file
     $ dchgrp -R pgay ./
 """
+from DIRAC import gLogger, S_OK
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
-from DIRAC import gLogger
 from DIRAC.Core.Base.Script import Script
-from DIRAC import S_OK
 
 
 class Params:
     def __init__(self):
         self.recursive = False
 
     def setRecursive(self, opt):
@@ -51,17 +50,17 @@
     fc = FileCatalog()
 
     for lfn in lfns:
         try:
             pathDict = {lfn: group}
             result = fc.changePathGroup(pathDict, params.recursive)
             if not result["OK"]:
-                gLogger.error("Error:", result["Message"])
+                gLogger.error(result["Message"])
                 break
             if lfn in result["Value"]["Failed"]:
-                gLogger.error("Error:", result["Value"]["Failed"][lfn])
-        except Exception as x:
-            print("Exception:", str(x))
+                gLogger.error(result["Value"]["Failed"][lfn])
+        except Exception as err:
+            gLogger.exception(err)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dchmod.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dchmod.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,16 +6,15 @@
     $ dchmod 755 ././some_lfn_file
     $ dchmod -R 700 ./
 """
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Core.Base.Script import Script
-from DIRAC import gLogger
-from DIRAC import S_OK
+from DIRAC import gLogger, S_OK
 
 
 class Params:
     def __init__(self):
         self.recursive = False
 
     def setRecursive(self, opt):
@@ -51,17 +50,17 @@
     fc = FileCatalog()
 
     for lfn in lfns:
         try:
             pathDict = {lfn: int(mode, base=8)}
             result = fc.changePathMode(pathDict, params.recursive)
             if not result["OK"]:
-                gLogger.error("Error:", result["Message"])
+                gLogger.error(result["Message"])
                 break
             if lfn in result["Value"]["Failed"]:
-                gLogger.error("Error:", result["Value"]["Failed"][lfn])
-        except Exception as x:
-            print("Exception:", str(x))
+                gLogger.error(result["Value"]["Failed"][lfn])
+        except Exception as err:
+            gLogger.exception(err)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dchown.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dchown.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,15 @@
     $ dchown atsareg ././some_lfn_file
     $ dchown -R pgay ./
 """
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Core.Base.Script import Script
-from DIRAC import gLogger
-from DIRAC import S_OK
+from DIRAC import gLogger, S_OK
 
 
 class Params:
     def __init__(self):
         self.recursive = False
 
     def setRecursive(self, opt):
@@ -51,17 +50,17 @@
     fc = FileCatalog()
 
     for lfn in lfns:
         try:
             pathDict = {lfn: owner}
             result = fc.changePathOwner(pathDict, params.recursive)
             if not result["OK"]:
-                gLogger.error("Error:", result["Message"])
+                gLogger.error(result["Message"])
                 break
             if lfn in result["Value"]["Failed"]:
-                gLogger.error("Error:", result["Value"]["Failed"][lfn])
-        except Exception as x:
-            print("Exception:", str(x))
+                gLogger.error(result["Value"]["Failed"][lfn])
+        except Exception as err:
+            gLogger.exception(err)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dconfig.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dconfig.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Configures ~/dirac/dcommands.conf. If run without arguments, lists contents of configuration file.
 
 Examples:
     $ dconfig -m (creates minimal config file in ~/dirac/dcommands.conf)
     $ dconfig (lists contents of ~/dirac/dcommands.conf)
 """
 import DIRAC
-from DIRAC import S_OK
+from DIRAC import gLogger, S_OK
 from DIRAC.Core.Base.Script import Script
 
 from DIRAC.Interfaces.Utilities.DCommands import (
     DConfig,
     createMinimalConfig,
 )
 from DIRAC.Interfaces.Utilities.DCommands import getDNFromProxy
@@ -55,20 +55,19 @@
     modified = False
 
     if not args:
         sections = dconfig.sections()
         for s in sections:
             retVal = dconfig.get(s, None)
             if not retVal["OK"]:
-                print("Error:", retVal["Message"])
+                gLogger.error(retVal["Message"])
                 DIRAC.exit(-1)
-            print(f"[{s}]")
+            gLogger.notice(f"[{s}]")
             for o, v in retVal["Value"]:
-                print(o, "=", v)
-            print
+                gLogger.notice(f"{o} = {v}")
         DIRAC.exit(0)
 
     for arg in args:
         value = None
         section = None
         option = None
         if "=" in arg:
@@ -80,23 +79,23 @@
 
         if value != None:
             dconfig.set(section, option, value)
             modified = True
         else:
             retVal = dconfig.get(section, option)
             if not retVal["OK"]:
-                print("Error:", retVal["Message"])
+                gLogger.error(retVal["Message"])
                 DIRAC.exit(-1)
             ret = retVal["Value"]
             if isinstance(ret, list):
-                print(f"[{section}]")
+                gLogger.notice(f"[{section}]")
                 for o, v in ret:
-                    print(o, "=", v)
+                    gLogger.notice(f"{o} = {v}")
             else:
-                print(option, "=", ret)
+                gLogger.notice(f"{option} = {ret}")
 
     if modified:
         dconfig.write()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dfind.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dfind.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dget.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dget.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 import DIRAC
 
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import DCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
-
 from DIRAC.Core.Base.Script import Script
+from DIRAC import gLogger
 
 
 class Params:
     def __init__(self):
         self.recursive = False
 
     def setRecursive(self, arg=None):
@@ -60,15 +60,15 @@
     catalog = DCatalog()
 
     from DIRAC.Interfaces.API.Dirac import Dirac
 
     dirac = Dirac()
 
     if len(args) < 1:
-        print("Error: Not enough arguments provided:")
+        gLogger.error("Not enough arguments provided:")
         Script.showHelp()
         DIRAC.exit(-1)
 
     # lfn
     lfn = pathFromArgument(session, args[0])
 
     localDir = os.getcwd()
@@ -76,37 +76,37 @@
 
     if len(args) > 1:
         # localDir provided must be last argument
         localDir = args[-1]
         lfns = [(pathFromArgument(session, lfn), localDir) for lfn in args[:-1]]
 
         if not os.path.isdir(localDir):
-            print("Error: Destination local path must be a directory")
+            gLogger.error("Destination local path must be a directory")
             DIRAC.exit(-1)
 
     exitCode = 0
 
     if params.getRecursive():
         newLFNs = []
         for lfn, localDir in lfns:
             # make sure lfn is an existing directory
             if not catalog.isDir(lfn):
                 if catalog.isFile(lfn):
                     # lfn is a file: simply add it to the list
                     newLFNs.append((lfn, localDir))
                     continue
                 exitCode = -1
-                print(f"Error: Invalid path: '{lfn}'")
+                gLogger.error(f"Invalid path: '{lfn}'")
                 continue
 
             retVal = catalog.findFilesByMetadata({}, lfn)
 
             if not retVal["OK"]:
                 exitCode = -2
-                print("Error:", retVal["Message"])
+                gLogger.error(retVal["Message"])
                 continue
 
             # compute new local destination for subtree files
             lfnDirname = os.path.dirname(lfn)
             for newLFN in retVal["Value"]:
                 newLocalDir = os.path.dirname(os.path.join(localDir, os.path.relpath(newLFN, lfnDirname)))
                 newLFNs.append((newLFN, newLocalDir))
@@ -116,14 +116,14 @@
         if params.getRecursive():
             if not os.path.exists(localDir):
                 os.makedirs(localDir)
 
         ret = dirac.getFile(lfn, localDir)
         if not ret["OK"]:
             exitCode = -3
-            print(f"Error: {ret['Message']}")
+            gLogger.error(ret["Message"])
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dgetenv.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dgetenv.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 """
 print DCommands session environment variables
 """
 import DIRAC
+from DIRAC import gLogger
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
 
 @Script()
 def main():
@@ -22,26 +23,26 @@
     args = Script.getPositionalArgs()
 
     session = DSession()
 
     if not args:
         retVal = session.listEnv()
         if not retVal["OK"]:
-            print("Error:", retVal["Message"])
+            gLogger.error(retVal["Message"])
             DIRAC.exit(-1)
         for o, v in retVal["Value"]:
-            print(o + "=" + v)
+            gLogger.notice(f"{o} = {v}")
         DIRAC.exit(0)
 
     section, option = arg.split(".") if "." in (arg := args[0]) else (None, arg)
 
     result = session.get(section, option) if section else session.getEnv(option)
 
     if not result["OK"]:
-        print("Error:", result["Message"])
+        gLogger.error(result["Message"])
         DIRAC.exit(-1)
 
-    print(result["Value"])
+    gLogger.notice(result["Value"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dinit.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dinit.py`

 * *Files 22% similar despite different names*

```diff
@@ -51,35 +51,35 @@
 
     session = None
     if params.fromProxy:
         retVal = Script.enableCS()
         ConfigCache(forceRefresh=True).cacheConfig()
 
         if not retVal["OK"]:
-            print("Error:", retVal["Message"])
+            gLogger.error(retVal["Message"])
             DIRAC.exit(-1)
         session = sessionFromProxy()
     else:
         session = DSession(profile)
 
     if not session:
-        print("Error: Session couldn't be initialized")
+        gLogger.error("Session couldn't be initialized")
         DIRAC.exit(-1)
 
     session.write()
 
     try:
         session.checkProxyOrInit()
-    except Exception as e:
-        print("Error:", e)
+    except Exception as err:
+        gLogger.exception(err)
         DIRAC.exit(-1)
 
     retVal = session.proxyInfo()
     if not retVal["OK"]:
-        print(retVal["Message"])
+        gLogger.error(retVal["Message"])
         DIRAC.exit(-1)
 
-    print(ProxyInfo.formatProxyInfoAsString(retVal["Value"]))
+    gLogger.notice(ProxyInfo.formatProxyInfoAsString(retVal["Value"]))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_add_group.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_add_group.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_add_host.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_add_host.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_add_user.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_add_user.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_allow_site.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_allow_site.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_ban_site.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_ban_site.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_ce_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_ce_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_delete_user.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_delete_user.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_banned_sites.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_banned_sites.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilot_output.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilot_output.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilots.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_job_pilots.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_logging_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_logging_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_output.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_pilot_output.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_get_site_mask.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_get_site_mask.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_list_hosts.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_list_hosts.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_list_users.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_list_users.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_modify_user.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_modify_user.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_pilot_summary.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_pilot_summary.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_reset_job.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_reset_job.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_service_ports.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_service_ports.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_set_site_protocols.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_set_site_protocols.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_site_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_site_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_site_mask_logging.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_site_mask_logging.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_admin_sync_users_from_file.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_admin_sync_users_from_file.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_get_file.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_get_file.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_accessURL.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_accessURL.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_metadata.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_metadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_replicas.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_lfn_replicas.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_accessURL.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_accessURL.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_metadata.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_pfn_metadata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_dms_replicate_lfn.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_dms_replicate_lfn.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_framework_ping_service.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_framework_ping_service.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_framework_self_ping.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_framework_self_ping.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_utils_file_adler.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_utils_file_adler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_utils_file_md5.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_utils_file_md5.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_get_normalized_queue_length.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_get_normalized_queue_length.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_get_queue_normalization.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_get_queue_normalization.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_attributes.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_attributes.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_delete.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_delete.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_input.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_input.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_jdl.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_jdl.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output_data.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_get_output_data.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_kill.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_kill.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_logging_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_logging_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_parameters.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_parameters.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_peek.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_peek.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_reschedule.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_reschedule.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_status.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_status.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_job_submit.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_job_submit.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_jobs_select_output_search.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_jobs_select_output_search.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dirac_wms_select_jobs.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dirac_wms_select_jobs.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dkill.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dkill.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 """
   Kill or delete DIRAC job
 """
 import DIRAC
+from DIRAC import gLogger
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 
 
 class Params:
     def __init__(self):
@@ -62,19 +63,19 @@
         result = session.getUserName()
         if result["OK"]:
             userName = result["Value"]
 
             monitoring = JobMonitoringClient()
             result = monitoring.getJobs({"Owner": userName})
             if not result["OK"]:
-                print("ERROR:", result["Message"])
+                gLogger.error(result["Message"])
             else:
                 jobs += map(int, result["Value"])
         else:
-            print("ERROR:", result["Message"])
+            gLogger.error(result["Message"])
 
     errors = []
     for job in jobs:
         result = None
         if params.delete:
             result = wmsClient.deleteJob(job)
         else:
@@ -82,17 +83,17 @@
         if not result["OK"]:
             errors.append(result["Message"])
             exitCode = 2
         elif params.getVerbose():
             action = "killed"
             if params.getDelete():
                 action = "deleted"
-            print(action, "job", job)
+            gLogger.notice(f"{action} job {job}")
 
     for error in errors:
-        print("ERROR:", error)
+        gLogger.error(str(error))
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dlogging.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dlogging.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 """
   Retrieve logging information for a DIRAC job
 """
 import DIRAC
+from DIRAC import gLogger
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import ArrayFormatter
 from DIRAC.WorkloadManagementSystem.Client.JobMonitoringClient import JobMonitoringClient
 from DIRAC.Core.Base.Script import Script
 
 
 class Params:
@@ -40,20 +41,20 @@
     monitoring = JobMonitoringClient()
     af = ArrayFormatter(params.getFmt())
     headers = ["Status", "MinorStatus", "ApplicationStatus", "Time", "Source"]
     errors = []
     for job in jobs:
         result = monitoring.getJobLoggingInfo(job)
         if result["OK"]:
-            print(af.listFormat(result["Value"], headers, sort=headers.index("Time")))
+            gLogger.notice(af.listFormat(result["Value"], headers, sort=headers.index("Time")))
         else:
             errors.append(result["Message"])
             exitCode = 2
 
     for error in errors:
-        print("ERROR:", error)
+        gLogger.error(error)
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dls.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dls.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     $ dls ..
     $ dls /
 """
 import os
 import sys
 import getopt
 
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 from DIRAC.Core.Base.Script import Script
 
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import createCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArguments
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
@@ -179,15 +179,15 @@
             try:
                 result = self.fc.getReplicas(path)
                 if result["OK"]:
                     if result["Value"]["Successful"]:
                         for se, entry in result["Value"]["Successful"][path].items():
                             replicas.append(se.ljust(15) + " " + entry)
                     else:
-                        print("Replicas: ", result)  # [ 'Message' ]
+                        gLogger.notice("Replicas: ", result)  # [ 'Message' ]
             except Exception as x:
                 replicas.append("replicas failed:" + str(x))
             return tuple(replicas)
 
         def do_ls(self, args):
             """Lists directory entries at <path>
 
@@ -220,16 +220,16 @@
                 "human-readable",
             ]
             path = self.cwd
             if argss:
                 try:
                     optlist, arguments = getopt.getopt(argss, short_opts, long_opts)
                 except getopt.GetoptError as e:
-                    print(str(e))
-                    print(self.do_ls.__doc__)
+                    gLogger.notice(str(e))
+                    gLogger.notice(self.do_ls.__doc__)
                     return
                 # Duplicated options are allowed: later options have precedence, e.g.,
                 # '-ltSt' will be order by time
                 # '-ltStS' will be order by size
                 options = [opt for (opt, arg) in optlist]
                 for opt in options:
                     if opt in ["-l", "--long"]:
@@ -272,73 +272,69 @@
             # remove last character if it is "/"
             if path[-1] == "/" and path != "/":
                 path = path[:-1]
 
             # Check if the target path is a file
             result = self.fc.isFile(path)
             if not result["OK"]:
-                print("Error: can not verify path")
+                gLogger.error("Can not verify path")
                 return
             elif path in result["Value"]["Successful"] and result["Value"]["Successful"][path]:
                 result = self.fc.getFileMetadata(path)
                 dList = ReplicaDirectoryListing()
                 fileDict = result["Value"]["Successful"][path]
 
                 replicas = self.getReplicas(path)
 
                 dList.addFileWithReplicas(os.path.basename(path), fileDict, numericid, replicas)
                 dList.printListing(reverse, timeorder, sizeorder, humanread)
                 return
 
             result = self.fc.isDirectory(path)
             if not result["OK"]:
-                print("Error: can not verify path")
+                gLogger.error("Can not verify path")
                 return
             elif path not in result["Value"]["Successful"] or not result["Value"]["Successful"][path]:
-                print(f'Error: "{path}" doesn\'t exist')
+                gLogger.error(f'"{path}" doesn\'t exist')
                 return
 
             # Get directory contents now
             try:
                 result = self.fc.listDirectory(path, long)
                 dList = ReplicaDirectoryListing()
                 if result["OK"]:
                     if result["Value"]["Successful"]:
                         for entry in result["Value"]["Successful"][path]["Files"]:
                             fname = entry.split("/")[-1]
-                            # print(entry, fname)
-                            # fname = entry.replace( self.cwd,'' ).replace( '/','' )
                             if long:
                                 fileDict = result["Value"]["Successful"][path]["Files"][entry]["MetaData"]
                                 if fileDict:
                                     replicas = self.getReplicas(os.path.join(path, fname))
                                     dList.addFileWithReplicas(fname, fileDict, numericid, replicas)
                             else:
                                 dList.addSimpleFile(fname)
                         for entry in result["Value"]["Successful"][path]["SubDirs"]:
                             dname = entry.split("/")[-1]
-                            # print(entry, dname)
-                            # dname = entry.replace( self.cwd,'' ).replace( '/','' )
                             if long:
                                 dirDict = result["Value"]["Successful"][path]["SubDirs"][entry]
                                 if dirDict:
                                     dList.addDirectory(dname, dirDict, numericid)
                             else:
                                 dList.addSimpleFile(dname)
                         for entry in result["Value"]["Successful"][path]["Links"]:
                             pass
 
                         if long:
                             dList.printListing(reverse, timeorder, sizeorder, humanread)
                         else:
                             dList.printOrdered()
                 else:
-                    print("Error:", result["Message"])
-            except Exception as x:
-                print("Error:", str(x))
+                    gLogger.error(result["Message"])
+            except Exception as err:
+                gLogger.exception(err)
 
     session = DSession()
 
     fccli = None
 
     if params.getReplicas():
         fccli = ReplicaFileCatalogClientCLI(createCatalog())
@@ -388,16 +384,16 @@
                 params.setTime(False)
                 optstr = optstr + "-S "
             else:
                 params.setSize(False)
                 optstr = optstr + "-t "
 
         except getopt.GetoptError as e:
-            print(str(e))
-            print(fccli.do_ls.__doc__)
+            gLogger.error(str(e))
+            gLogger.notice(fccli.do_ls.__doc__)
             exit(1)
 
     for p in pathFromArguments(session, args):
         print(f"{p}:")
         fccli.do_ls(optstr + p)
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dmeta.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dmeta.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Examples:
       $ dmeta add ./some_lfn_file some_meta="some_value"',
       $ dmeta -i f testindex=int
       $ dmeta ls ./some_lfn_file",
       $ dmeta rm ./some_lfn_file some_meta",
 """
 import DIRAC
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import DCatalog
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 
 
@@ -35,60 +35,60 @@
     def run(self, lfn, metas):
         metadict = {}
         for meta in metas:
             name, value = meta.split("=")
             metadict[name] = value
         result = self.fcClient.setMetadataBulk({lfn: metadict})
         if not result["OK"]:
-            print("Error:", result["Message"])
+            gLogger.error(result["Message"])
 
 
 class DMetaRm(DMetaCommand):
     def __init__(self, fcClient):
         self.fcClient = fcClient
 
     def run(self, lfn, metas):
         result = self.fcClient.removeMetadata({lfn: metas})
         if not result["OK"]:
-            print("Error:", result["Message"])
+            gLogger.error(result["Message"])
 
 
 class DMetaList(DMetaCommand):
     def __init__(self, catalog):
         self.catalog = catalog
 
     def run(self, lfn, metas):
         retVal = self.catalog.getMeta(lfn)
 
         if not retVal["OK"]:
-            print("Error:", retVal["Message"])
+            gLogger.error(retVal["Message"])
             DIRAC.exit(-1)
         metadict = retVal["Value"]
 
         if not metas:
             for k, v in metadict.items():
-                print(k + "=" + str(v))
+                gLogger.notice(f"{k} = {v}")
         else:
             for meta in metas:
                 if meta in metadict.keys():
-                    print(meta + "=" + metadict[meta])
+                    gLogger.notice(f"{meta} = {metadict[meta]}")
 
 
 from DIRAC.Core.Base.Script import Script
 
 
 @Script()
 def main():
     class Params:
         def __init__(self):
             self.index = False
             self.listIndex = False
 
         def setIndex(self, arg):
-            print("Setting index:", arg)
+            gLogger.notice(f"Setting index: {arg}")
             self.index = arg
             return S_OK()
 
         def getIndex(self):
             return self.index
 
         def setListIndex(self, arg):
@@ -136,41 +136,41 @@
                 elif mtype.lower() == "float":
                     rtype = "FLOAT"
                 elif mtype.lower() == "date":
                     rtype = "DATETIME"
                 elif mtype.lower() == "metaset":
                     rtype = "MetaSet"
                 else:
-                    print(f"Error: illegal metadata type {mtype}")
+                    gLogger.error(f"Error: illegal metadata type {mtype}")
                     DIRAC.exit(-1)
                 res = fc.addMetadataField(meta, rtype, fdType)
                 if not res["OK"]:
-                    print(res["Message"])
+                    gLogger.error(res["Message"])
                     DIRAC.exit(-1)
         DIRAC.exit(0)
 
     if params.getListIndex():
         fccli.do_meta("show")
         DIRAC.exit(0)
 
     meta_commands = {
         "add": DMetaAdd(catalog.catalog),
         "rm": DMetaRm(catalog.catalog),
         "ls": DMetaList(catalog),
     }
 
     if len(args) < 2:
-        print(f"Error: Not enough arguments provided\n{Script.scriptName}:")
+        gLogger.error(f"Error: Not enough arguments provided\n{Script.scriptName}:")
         Script.showHelp(exitCode=-1)
 
     command = args[0]
 
     if command not in meta_commands.keys():
-        print(f'Error: Unknown dmeta command "{command}"')
-        print(f"{Script.scriptName}:")
+        gLogger.error(f'Unknown dmeta command "{command}"')
+        gLogger.notice(f"{Script.scriptName}:")
         Script.showHelp(exitCode=-1)
 
     command = meta_commands[command]
 
     lfn = pathFromArgument(session, args[1])
 
     metas = args[2:]
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dmkdir.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dmkdir.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 """
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import DCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArguments
 from DIRAC.Interfaces.Utilities.DCommands import createCatalog
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Core.Base.Script import Script
+from DIRAC import gLogger
 
 
 @Script()
 def main():
     configCache = ConfigCache()
     Script.registerArgument(["Path: path to new directory"])
     Script.parseCommandLine(ignoreErrors=True)
@@ -29,14 +30,14 @@
     session = DSession()
     catalog = createCatalog()
 
     result = catalog.createDirectory(pathFromArguments(session, args))
     if result["OK"]:
         if result["Value"]["Failed"]:
             for p in result["Value"]["Failed"]:
-                print(f'ERROR - "{p}":', result["Value"]["Failed"][p])
+                gLogger.error(f'"{p}":', result["Value"]["Failed"][p])
     else:
-        print("ERROR:", result["Message"])
+        gLogger.error(result["Message"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/doutput.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/doutput.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 """
   Retrieve output sandbox for a DIRAC job
 """
 import DIRAC
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Core.Base.Script import Script
 
 import os
 import datetime
 
 
@@ -122,26 +122,26 @@
         jobDate = toString(datetime.datetime.utcnow().date() - 30 * day)
 
         # Choose jobs in final state, no more than 30 days old
         for s in ["Done", "Failed"]:
             result = dirac.selectJobs(jobGroup=jobGroup, date=jobDate, status=s)
             if not result["OK"]:
                 if not "No jobs selected" in result["Message"]:
-                    print("Error:", result["Message"])
+                    gLogger.error(result["Message"])
                     exitCode = 2
             else:
                 args += result["Value"]
 
     jobs = []
 
     outputDir = params.getOutputDir() or os.path.curdir
 
     for arg in args:
         if os.path.isdir(os.path.join(outputDir, arg)) and not params.getNoJobDir():
-            print(f"Output for job {arg} already retrieved, remove the output directory to redownload")
+            gLogger.notice(f"Output for job {arg} already retrieved, remove the output directory to redownload")
         else:
             jobs.append(arg)
 
     if jobs:
         if not os.path.isdir(outputDir):
             os.makedirs(outputDir)
 
@@ -175,21 +175,21 @@
                 if result["OK"]:
                     inputs[job]["data"] = result["Value"]
                 else:
                     errors.append(result["Message"])
                     exitCode = 2
 
         for error in errors:
-            print("ERROR:", error)
+            gLogger.error(error)
 
         if params.getVerbose():
             for j, d in inputs.items():
                 if "osb" in d:
-                    print(f"{j}: OutputSandbox", d["osb"])
+                    gLogger.notice(f"{j}: OutputSandbox", d["osb"])
                 if "data" in d:
-                    print(f"{j}: OutputData", d["data"])
+                    gLogger.notice(f"{j}: OutputData", d["data"])
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dput.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dput.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Uploads a file to an SE and registers it in the file catalog.
 Uses the default SE specified in $HOME/.dirac/dcommands.conf unless overridden
 on the command line.
 """
 import os
 
 import DIRAC
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import DCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
 
@@ -72,15 +72,15 @@
     catalog = DCatalog()
 
     from DIRAC.Interfaces.API.Dirac import Dirac
 
     dirac = Dirac()
 
     if len(args) < 1:
-        print(f"Error: No argument provided\n{Script.scriptName}:")
+        gLogger.error(f"No argument provided\n{Script.scriptName}:")
         Script.showHelp(exitCode=-1)
 
     # local file
     localPath = args[0]
 
     # default lfn: same file name as localPath
     lfn = pathFromArgument(session, os.path.basename(localPath))
@@ -93,31 +93,33 @@
         pairs = []
         if catalog.isDir(lfn):
             # we can accept one ore more local files
             for lp in localPaths:
                 pairs.append((lp, os.path.join(lfn, os.path.basename(lp))))
         else:
             if len(localPaths) > 1:
-                print("Error: Destination LFN must be a directory when registering multiple local files")
+                gLogger.error("Destination LFN must be a directory when registering multiple local files")
                 DIRAC.exit(-1)
 
             # lfn filename replace local filename
             pairs.append((localPath, lfn))
 
     # destination SE
     se = params.getDestinationSE()
     if not se:
         retVal = session.getEnv("default_se", "NO DEFAULT")
         # the returned error message is not very user friendly
         # use "NO DEFAULT" to distinguish no default SE set from all
         # other error cases
         if not retVal["OK"]:
-            print("Error:", retVal["Message"])
+            gLogger.error(retVal["Message"])
         if retVal["Value"] == "NO DEFAULT":
-            print("Error: No default SE specified, please set default SE or specify SE on command line using -D option")
+            gLogger.error(
+                "No default SE specified, please set default SE or specify SE on command line using -D option"
+            )
             DIRAC.exit(-1)
         se = retVal["Value"]
 
     exitCode = 0
 
     if params.getRecursive():
         newPairs = []
@@ -132,14 +134,14 @@
         pairs = newPairs
 
     for localPath, lfn in pairs:
         ret = dirac.addFile(lfn, localPath, se, printOutput=False)
 
         if not ret["OK"]:
             exitCode = -2
-            print(f"Error: {lfn}:", ret["Message"])
+            gLogger.error(f"{lfn}:", ret["Message"])
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/drepl.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/drepl.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * random(N) - replicatefile to N randomly chosen SEs from the list in option "replication_ses"
 
 Examples
     $ drepl ./some_lfn_file
     $ drepl -D SOME-DESTINATION-SE-disk ./some_lfn_file
 """
 import DIRAC
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 from DIRAC.Core.Base.Script import Script
 
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArguments
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
 
@@ -94,15 +94,15 @@
     exitCode = 0
 
     for lfn in lfns:
         for dst in dsts:
             ret = dirac.replicateFile(lfn, dst, srcopt)
 
             if not ret["OK"]:
-                print(f"Error: {lfn} -> {dst}:", ret["Message"])
+                gLogger.error(f"{lfn} -> {dst}:", ret["Message"])
                 exitCode = -2
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dreplicas.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dreplicas.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 """
 Print list replicas for files in the FileCatalog
 """
 import DIRAC
+from DIRAC import gLogger
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Core.Utilities.ReturnValues import returnSingleResult
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import DCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
@@ -28,19 +29,19 @@
     for arg in args:
         # lfn
         lfn = pathFromArgument(session, args[0])
         # fccli.do_replicas( lfn )
         ret = returnSingleResult(catalog.catalog.getReplicas(lfn))
         if ret["OK"]:
             replicas = ret["Value"]
-            print(lfn + ":")
+            gLogger.notice(f"{lfn}:")
             for se, path in replicas.items():
-                print("  ", se, path)
+                gLogger.notice("  ", f"{se} {path}")
         else:
-            print(f"Error: {lfn}:", ret["Message"])
+            gLogger.error(f"{lfn}:", ret["Message"])
             exitCode = -2
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/drm.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/drm.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 Examples:
     $ drm ./some_lfn_file
 """
 import os
 
 import DIRAC
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import DCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
 
@@ -50,75 +50,74 @@
 
     args = Script.getPositionalArgs()
 
     session = DSession()
     catalog = DCatalog()
 
     if not args and not lfnFileName:
-        print(f"Error: No argument provided\n{Script.scriptName}:")
+        gLogger.error(f"No argument provided\n{Script.scriptName}:")
         Script.showHelp(exitCode=-1)
 
     lfns = set()
     for path in args:
         lfns.add(pathFromArgument(session, path))
 
     if lfnFileName:
         if not os.path.exists(lfnFileName):
-            print(f"Error: non-existent file {lfnFileName}:")
+            gLogger.error(f"non-existent file {lfnFileName}:")
             DIRAC.exit(-1)
         lfnFile = open(lfnFileName)
         lfnList = lfnFile.readlines()
         lfnSet = {pathFromArgument(session, lfn.strip()) for lfn in lfnList if lfn}
         lfns.update(lfnSet)
 
     from DIRAC.Interfaces.API.Dirac import Dirac
-    from DIRAC import gLogger
     from DIRAC.Core.Utilities.ReturnValues import returnSingleResult
     from DIRAC.DataManagementSystem.Client.DataManager import DataManager
 
     dirac = Dirac()
     dm = DataManager()
 
     nLfns = len(lfns)
     if nLfns > 1:
-        gLogger.notice("Removing %d objects" % nLfns)
+        gLogger.notice(f"Removing {nLfns} objects")
 
     exitCode = 0
     goodCounter = 0
     badCounter = 0
     for lfn in lfns:
         if rmDirFlag and not catalog.isFile(lfn):
             result = returnSingleResult(dm.cleanLogicalDirectory(lfn))
             if result["OK"]:
                 goodCounter += 1
             else:
-                print("ERROR:", result["Message"])
+                gLogger.error(result["Message"])
                 badCounter += 1
                 exitCode = 3
         else:
             if targetSE:
                 result = returnSingleResult(dirac.removeReplica(lfn, targetSE, printOutput=False))
             else:
                 result = returnSingleResult(dirac.removeFile(lfn, printOutput=False))
             if not result["OK"]:
                 if "No such file or directory" == result["Message"]:
                     gLogger.notice(f"{lfn} no such file")
                 else:
-                    gLogger.error(f"ERROR {lfn}: {result['Message']}")
+                    gLogger.error(f"{lfn}: {result['Message']}")
                     badCounter += 1
                     exitCode = 2
             else:
                 goodCounter += 1
                 if goodCounter % 10 == 0:
-                    gLogger.notice("%d files removed" % goodCounter)
+                    gLogger.notice(f"{goodCounter} files removed")
                     if badCounter:
-                        gLogger.notice("%d files failed removal" % badCounter)
+                        gLogger.notice(f"{badCounter} files failed removal")
 
-    gLogger.notice("\n%d object(s) removed in total" % goodCounter)
+    gLogger.notice(f"\n{goodCounter} object(s) removed in total")
     if badCounter:
-        gLogger.notice("%d object(s) failed removal in total" % badCounter)
+        gLogger.notice(f"{badCounter} object(s) failed removal in total")
 
     DIRAC.exit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/drmdir.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/drmdir.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,17 +2,16 @@
 """
 remove FileCatalog directories. Attention ! This command does not remove
 directories and files on the physical storage.
 
 Examples:
     $ drmdir ./some_lfn_directory
 """
+from DIRAC import gLogger
 from DIRAC.Core.Base.Script import Script
-
-
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DCommands import createCatalog
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArguments
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 
 
 @Script()
@@ -27,14 +26,14 @@
     session = DSession()
     catalog = createCatalog()
 
     result = catalog.removeDirectory(pathFromArguments(session, args))
     if result["OK"]:
         if result["Value"]["Failed"]:
             for p in result["Value"]["Failed"]:
-                print(f'ERROR - "{p}":', result["Value"]["Failed"][p])
+                gLogger.error(f'"{p}":', result["Value"]["Failed"][p])
     else:
-        print("ERROR:", result["Message"])
+        gLogger.error(result["Message"])
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dsize.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dsize.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dstat.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dstat.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
   Example:
     $ dstat -a -u your.dirac.username
 
 """
 import datetime
 
 from DIRAC import exit as DIRACExit, S_OK, S_ERROR
+from DIRAC import gLogger
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import ArrayFormatter
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Core.Utilities.TimeUtilities import toString, day
 from DIRAC.WorkloadManagementSystem.Client.JobStatus import JOB_STATES, JOB_FINAL_STATES
 from DIRAC.WorkloadManagementSystem.Client.JobMonitoringClient import (
@@ -222,34 +223,34 @@
             owner=userName,
             date=jobDate,
             jobGroup=params.getJobGroup(),
             jobName=params.getJobName(),
         )
 
         if not result["OK"]:
-            print("Error:", result["Message"])
+            gLogger.error(result["Message"])
             DIRACExit(-1)
 
         jobs = result["Value"]
 
     try:
         jobs = [int(job) for job in jobs]
     except Exception as x:
-        print("Expected integer for jobID")
+        gLogger.error("Expected integer for jobID")
         exitCode = 2
         DIRACExit(exitCode)
 
     summaries = {}
     statuses = params.getStatus()
 
     # split summary requests in chunks of a reasonable size (saves memory)
     for chunk in chunks(jobs, 1000):
         result = getJobSummary(chunk)
         if not result["OK"]:
-            print("ERROR:", result["Message"])
+            gLogger.error(result["Message"])
             DIRACExit(2)
 
         # filter on job statuses
         if "all" in statuses:
             summaries = result["Value"]
         else:
             for j in result["Value"]:
@@ -257,14 +258,14 @@
                     summaries[j] = result["Value"][j]
 
     for s in summaries.values():
         s["JobID"] = int(s["JobID"])
 
     af = ArrayFormatter(params.getFmt())
 
-    print(af.dictFormat(summaries, ["JobID"] + params.getFields(), sort="JobID"))
+    gLogger.notice(af.dictFormat(summaries, ["JobID"] + params.getFields(), sort="JobID"))
 
     DIRACExit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Interfaces/scripts/dsub.py` & `DIRAC-8.1.0a9/src/DIRAC/Interfaces/scripts/dsub.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Default JDL can be configured from session in the "JDL" option
 """
 import os.path
 import sys
 import re
 import tempfile
 
-from DIRAC import S_OK
+from DIRAC import S_OK, gLogger
 from DIRAC import exit as DIRACexit
 from DIRAC.Interfaces.Utilities.DCommands import pathFromArgument
 from DIRAC.Interfaces.Utilities.DConfigCache import ConfigCache
 from DIRAC.Interfaces.Utilities.DCommands import DSession
 from DIRAC.Interfaces.API.Dirac import Dirac
 from DIRAC.Core.Base.Script import Script
 from DIRAC.Core.Utilities.ClassAd.ClassAdLight import ClassAd
@@ -406,17 +406,17 @@
     if jdlExecutable and not cmd:
         cmd = jdlExecutable
 
     tempFiles = []
     if cmd is None:
         # get executable script from stdin
         if sys.stdin.isatty():
-            print("\nThe executable is not given")
-            print("Type in the executable script lines, finish with ^D")
-            print("or exit job submission with ^C\n")
+            gLogger.notice("\nThe executable is not given")
+            gLogger.notice("Type in the executable script lines, finish with ^D")
+            gLogger.notice("or exit job submission with ^C\n")
 
         lines = sys.stdin.readlines()
 
         # Manage JDL directives inserted in cmd
         jdlDirectives = parseScriptLinesJDLDirectives(lines)
         classAdJob.contents.update(jdlDirectives)
         # re-apply parameters options to take priority over script JDL directives
@@ -449,32 +449,32 @@
             classAdJob.insertAttributeString("Executable", os.path.basename(cmd))
         else:
             classAdJob.insertAttributeString("Executable", cmd)
 
         uploadExec = params.getForceExecUpload() or not cmd.startswith("/")
         if uploadExec:
             if not os.path.isfile(cmd):
-                print(f'ERROR: executable file "{cmd}" not found')
+                gLogger.error(f'Executable file "{cmd}" not found')
                 DIRACexit(2)
 
             classAdAppendToInputSandbox(classAdJob, cmd)
 
             # set job name based on script file name
             if not classAdJob.lookupAttribute("JobName"):
                 classAdJob.insertAttributeString("JobName", cmd)
 
         if cmdArgs:
             classAdJob.insertAttributeString("Arguments", " ".join(cmdArgs))
 
     classAdJobs = params.parameterizeClassAd(classAdJob)
 
     if params.getVerbose():
-        print("JDL:")
+        gLogger.notice("JDL:")
         for p in params.parameterizeClassAd(classAdJob):
-            print(p.asJDL())
+            gLogger.notice(p.asJDL())
 
     jobIDs = []
 
     for classAdJob in classAdJobs:
         jdlString = classAdJob.asJDL()
         result = dirac.submitJob(jdlString)
         if result["OK"]:
@@ -484,27 +484,27 @@
                 jobIDs += result["Value"]
         else:
             errorList.append((jdlString, result["Message"]))
             exitCode = 2
 
     if jobIDs:
         if params.getVerbose():
-            print(
+            gLogger.notice(
                 "JobID:",
             )
-        print(",".join(map(str, jobIDs)))
+        gLogger.notice(",".join(map(str, jobIDs)))
 
     # remove temporary generated files, if any
     for f in tempFiles:
         try:
             os.unlink(f)
-        except Exception as e:
-            errorList.append(str(e))
+        except Exception as err:
+            errorList.append(err)
 
     for error in errorList:
-        print("ERROR %s: %s" % error)
+        gLogger.error(f"{error}")
 
     DIRACexit(exitCode)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/DataOperationSender.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/DataOperationSender.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/MonitoringClient.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/MonitoringClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/MonitoringReporter.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/MonitoringReporter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/ServerUtils.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/ServerUtils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/AgentMonitoring.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/AgentMonitoring.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/BaseType.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/BaseType.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/DataOperation.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/DataOperation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/FailedDataOperation.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/FailedDataOperation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/PilotSubmissionMonitoring.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/PilotSubmissionMonitoring.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/PilotsHistory.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/PilotsHistory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/RMSMonitoring.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/RMSMonitoring.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/ServiceMonitoring.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/ServiceMonitoring.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Client/Types/WMSHistory.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Client/Types/WMSHistory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/MonitoringDB.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/MonitoringDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/DB/test/Test_monitoringdb.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/DB/test/Test_monitoringdb.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/Service/MonitoringHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/Service/MonitoringHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/DBUtils.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/DBUtils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/MainReporter.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/MainReporter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/BasePlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/BasePlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/RMSMonitoringPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/RMSMonitoringPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/MonitoringSystem/private/Plotters/WMSHistoryPlotter.py` & `DIRAC-8.1.0a9/src/DIRAC/MonitoringSystem/private/Plotters/WMSHistoryPlotter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Client/ProductionClient.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Client/ProductionClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Client/ProductionStep.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Client/ProductionStep.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/DB/ProductionDB.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/DB/ProductionDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/DB/ProductionDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/DB/ProductionDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Service/ProductionManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Service/ProductionManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Service/TornadoProductionManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Service/TornadoProductionManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/ProdTransManager.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/ProdTransManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/ProdValidator.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/ProdValidator.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/Utilities/StateMachine.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/Utilities/StateMachine.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_add_trans.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_add_trans.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_clean.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_clean.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_complete.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_complete.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_delete.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_delete.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_all.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_all.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_description.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_description.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_trans.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_get_trans.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_start.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_start.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ProductionSystem/scripts/dirac_prod_stop.py` & `DIRAC-8.1.0a9/src/DIRAC/ProductionSystem/scripts/dirac_prod_stop.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/CleanReqDBAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/CleanReqDBAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestExecutingAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestExecutingAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/ForwardDISET.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/ForwardDISET.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/test/ForwardDISETTests.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Agent/RequestOperations/test/ForwardDISETTests.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/File.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/File.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/Operation.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/Operation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/ReqClient.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/ReqClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/Request.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/Request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/Test_File.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/Test_File.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/Test_Operation.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/Test_Operation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Client/test/Test_Request.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Client/test/Test_Request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/RequestDB.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/RequestDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/test/RMSTestScenari.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/test/RMSTestScenari.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/DB/test/Test_RequestDB.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/DB/test/Test_RequestDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/ReqManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/ReqManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/ReqProxyHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/ReqProxyHandler.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,18 +163,18 @@
             gLogger.exception(err)
             return S_ERROR(err)
         return S_OK(cachedRequests)
 
     types_putRequest = [str]
 
     def export_putRequest(self, requestJSON):
-        """forward request from local RequestDB to central RequestManager
+        """Dump the request in a local cache for later forwarding
 
         :param self: self reference
-        :param str requestType: request type
+        :param str requestJSON: json dump of the request
         """
 
         requestDict = json.loads(requestJSON)
         requestName = requestDict.get("RequestID", requestDict.get("RequestName", "***UNKNOWN***"))
         gLogger.info("putRequest: got request", f"{requestName}")
 
         # We only need the object to check the authorization
@@ -185,29 +185,21 @@
         if not isAuthorized:
             return S_ERROR(DErrno.ENOAUTH, "Credentials in the requests are not allowed")
 
         forwardable = self.__forwardable(requestDict)
         if not forwardable["OK"]:
             gLogger.warn("putRequest: ", f"{forwardable['Message']}")
 
-        setRequest = self.requestManager().putRequest(requestJSON)
-        if not setRequest["OK"]:
-            gLogger.error(
-                "setRequest: unable to set request", f"'{requestName}' @ RequestManager: {setRequest['Message']}"
-            )
-            # # put request to the request file cache
-            save = self.__saveRequest(requestName, requestJSON)
-            if not save["OK"]:
-                gLogger.error("setRequest: unable to save request to the cache", save["Message"])
-                return save
-            gLogger.info("setRequest: ", f"{requestName} is saved to {save['Value']} file")
-            return S_OK({"set": False, "saved": True})
-
-        gLogger.info("setRequest: ", f"request '{requestName}' has been set to the ReqManager")
-        return S_OK({"set": True, "saved": False})
+        # # put request to the request file cache
+        save = self.__saveRequest(requestName, requestJSON)
+        if not save["OK"]:
+            gLogger.error("setRequest: unable to save request to the cache", save["Message"])
+            return save
+        gLogger.info("setRequest: ", f"{requestName} is saved to {save['Value']} file")
+        return S_OK({"set": False, "saved": True})
 
     @staticmethod
     def __forwardable(requestDict):
         """check if request if forwardable
 
         The sub-request of type transfer:putAndRegister, removal:physicalRemoval and removal:reTransfer are
         definitely not, they should be executed locally, as they are using local fs.
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/Service/test/OperationHandlerBaseTests.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/Service/test/OperationHandlerBaseTests.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/OperationHandlerBase.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/OperationHandlerBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/RequestTask.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/RequestTask.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/RequestValidator.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/RequestValidator.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/Test_OperationHandlerBase.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/Test_OperationHandlerBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/Test_RequestTask.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/Test_RequestTask.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/private/test/Test_RequestValidator.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/private/test/Test_RequestValidator.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_list_req_cache.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_list_req_cache.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_reqdb_summary.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_reqdb_summary.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_request.py` & `DIRAC-8.1.0a9/src/DIRAC/RequestManagementSystem/scripts/dirac_rms_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/CacheFeederAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/CacheFeederAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/ElementInspectorAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/ElementInspectorAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/EmailAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/EmailAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/RucioRSSAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/RucioRSSAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/SiteInspectorAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/SiteInspectorAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/SummarizeLogsAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/SummarizeLogsAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/TokenAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/TokenAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ElementInspectorAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ElementInspectorAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ResourceStatusSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_ResourceStatusSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_SiteInspectorAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Agent/test/Test_Agent_SiteInspectorAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/ResourceManagementClient.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/ResourceManagementClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/ResourceStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/ResourceStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/ResourceStatusClient.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/ResourceStatusClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Client/SiteStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Client/SiteStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/Command.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/Command.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/CommandCaller.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/CommandCaller.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/DowntimeCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/DowntimeCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/FreeDiskSpaceCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/FreeDiskSpaceCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/GGUSTicketsCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/GGUSTicketsCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/GOCDBSyncCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/GOCDBSyncCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/JobCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/JobCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/MacroCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/MacroCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/PilotCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/PilotCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/PropagationCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/PropagationCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/TransferCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/TransferCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBStatusCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBStatusCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBSyncCommand.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Command/test/Test_RSS_Command_GOCDBSyncCommand.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/ResourceManagementDB.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/ResourceManagementDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/DB/ResourceStatusDB.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/DB/ResourceStatusDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysActivePolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysActivePolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysBannedPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysBannedPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysDegradedPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysDegradedPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/AlwaysProbingPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/AlwaysProbingPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/CEAvailabilityPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/CEAvailabilityPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/Configurations.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/Configurations.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/DowntimePolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/DowntimePolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/FreeDiskSpacePolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/FreeDiskSpacePolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/GGUSTicketsPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/GGUSTicketsPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobDoneRatioPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobDoneRatioPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobEfficiencyPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobRunningMatchedRatioPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobRunningMatchedRatioPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/JobRunningWaitingRatioPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/JobRunningWaitingRatioPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/PilotEfficiencyPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/PilotEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/PropagationPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/PropagationPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_AlwaysActivePolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_AlwaysActivePolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_CEAvailabilityPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_CEAvailabilityPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_Configurations.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_DTPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_DTPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_FreeDiskSpacePolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_FreeDiskSpacePolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_GGUSTicketsPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_GGUSTicketsPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobDoneRatioPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobDoneRatioPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobEfficiencyPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningMatchedRatioPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningMatchedRatioPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningWaitingRatioPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_JobRunningWaitingRatioPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_PilotEfficiencyPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Policy/test/Test_RSS_Policy_PilotEfficiencyPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/BaseAction.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/BaseAction.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/EmailAction.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogPolicyResultAction.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogPolicyResultAction.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogStatusAction.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/LogStatusAction.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/SlackAction.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/Actions/SlackAction.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PDP.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PDP.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PEP.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PEP.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyBase.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyCaller.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/PolicyCaller.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/StateMachine.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/StateMachine.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/PolicySystem/test/Test_PolicySystem.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/PolicySystem/test/Test_PolicySystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/PublisherHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/PublisherHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/ResourceManagementHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/ResourceManagementHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Service/ResourceStatusHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Service/ResourceStatusHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/CSHelpers.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/CSHelpers.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/InfoGetter.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/InfoGetter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/RSSCache.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/RSSCache.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/RSSCacheNoThread.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/RSSCacheNoThread.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/RssConfiguration.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/RssConfiguration.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/Synchronizer.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/Synchronizer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/Utilities/Utils.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/Utilities/Utils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_list_status.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_list_status.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_db.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_db.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_dtcache.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_query_dtcache.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_status.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_status.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_token.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_set_token.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_sync.py` & `DIRAC-8.1.0a9/src/DIRAC/ResourceStatusSystem/scripts/dirac_rss_sync.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/DummyPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/DummyPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/FCConditionBasePlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/FCConditionBasePlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/FilenamePlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/FilenamePlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/ProxyPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/ProxyPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_FilenamePlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_FilenamePlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_ProxyPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/ConditionPlugins/test/Test_ProxyPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FCConditionParser.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FCConditionParser.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalog.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalog.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalogClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalogClient.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,14 +669,14 @@
         :returns: result from the TransferClient
         """
         if isinstance(seNames, str):
             seNames = seNames.split(",")
 
         seNames = json.dumps(seNames)
 
-        dfc = TransferClient(self.serverURL, timeout=3600)
+        dfc = TransferClient(self.serverURL, timeout=20000)
         return dfc.receiveFile(outputFilename, seNames)
 
     @checkCatalogArguments
     def getDirectoryDump(self, lfns, timeout=120):
         """Get the content of a directory recursively"""
         return self._getRPC(timeout=timeout).getDirectoryDump(lfns)
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalogClientBase.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalogClientBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/FileCatalogFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/FileCatalogFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/PoolXMLCatalog.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/PoolXMLCatalog.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/PoolXMLFile.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/PoolXMLFile.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/RucioFileCatalogClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/RucioFileCatalogClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/TSCatalogClient.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/TSCatalogClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/Test_FCConditionParser.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/Test_FCConditionParser.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/Test_FileCatalog.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/Test_FileCatalog.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Catalog/test/mock_FC.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Catalog/test/mock_FC.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ARC6ComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ARC6ComputingElement.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 **Code Documentation**
 """
 import os
 import stat
 
 import arc  # Has to work if this module is called #pylint: disable=import-error
 from DIRAC import S_OK, S_ERROR
-from DIRAC.Resources.Computing.ARCComputingElement import ARCComputingElement
+from DIRAC.Resources.Computing.ARCComputingElement import ARCComputingElement, prepareProxyToken
 
 
 class ARC6ComputingElement(ARCComputingElement):
     def __init__(self, ceUniqueID):
         """Standard constructor."""
         super().__init__(ceUniqueID)
         # To ease the association between pilots and jobs, we need to remove the "REST" information
@@ -82,25 +82,21 @@
 
             j.ServiceInformationURL = arc.URL(str(commonURL))
             j.ServiceInformationInterfaceName = "org.nordugrid.arcrest"
 
         j.PrepareHandler(self.usercfg)
         return j
 
+    @prepareProxyToken
     def submitJob(self, executableFile, proxy, numberOfJobs=1):
         """Method to submit job"""
 
         # Assume that the ARC queues are always of the format nordugrid-<batchSystem>-<queue>
         # And none of our supported batch systems have a "-" in their name
         self.arcQueue = self.queue.split("-", 2)[2]
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
 
         self.log.verbose(f"Executable file path: {executableFile}")
         if not os.access(executableFile, 5):
             os.chmod(executableFile, stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH + stat.S_IXOTH)
 
         batchIDList = []
         stampDict = {}
@@ -170,25 +166,20 @@
         if batchIDList:
             result = S_OK(batchIDList)
             result["PilotStampDict"] = stampDict
         else:
             result = S_ERROR("No pilot references obtained from the ARC job submission")
         return result
 
+    @prepareProxyToken
     def getCEStatus(self):
         """Method to return information on running and pending jobs.
         We hope to satisfy both instances that use robot proxies and those which use proper configurations.
         """
 
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
-
         # Creating an endpoint
         endpoint = arc.Endpoint(self.ceHost, arc.Endpoint.COMPUTINGINFO, self.computingInfoEndpoint)
 
         # Get the ExecutionTargets of the ComputingElement (Can be REST, EMI-ES or GRIDFTP)
         retriever = arc.ComputingServiceRetriever(self.usercfg, [endpoint])
         retriever.wait()  # Takes a bit of time to get and parse the ldap information
         targetsWithQueues = retriever.GetExecutionTargets()
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ARCComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ARCComputingElement.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,14 +83,37 @@
     "Wiped": PilotStatus.ABORTED,
     "Deleted": PilotStatus.ABORTED,
     "Hold": PilotStatus.FAILED,
     "Undefined": PilotStatus.UNKNOWN,
 }
 
 
+def prepareProxyToken(func):
+    """Decorator to set up proxy or token as necessary"""
+
+    def wrapper(*args, **kwargs):
+        # Get the reference to the CE class object
+        self = args[0]
+
+        # Prepare first the proxy
+        result = self._prepareProxy()
+        if not result["OK"]:
+            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
+            return result
+        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
+
+        # Set the token in the environment if needed
+        if self.token:
+            os.environ["BEARER_TOKEN"] = self.token["access_token"]
+
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
 class ARCComputingElement(ComputingElement):
     _arcLevels = ["DEBUG", "VERBOSE", "INFO", "WARNING", "ERROR", "FATAL"]
 
     #############################################################################
     def __init__(self, ceUniqueID):
         """Standard constructor."""
         super().__init__(ceUniqueID)
@@ -279,21 +302,17 @@
                 logstdout.setFormat(arc.ShortFormat)
                 arc.Logger_getRootLogger().addDestination(logstdout)
                 arc.Logger_getRootLogger().setThreshold(getattr(arc, logLevel))
 
         return S_OK()
 
     #############################################################################
+    @prepareProxyToken
     def submitJob(self, executableFile, proxy, numberOfJobs=1, inputs=None, outputs=None):
         """Method to submit job"""
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
 
         self.log.verbose(f"Executable file path: {executableFile}")
         if not os.access(executableFile, 5):
             os.chmod(executableFile, stat.S_IRWXU | stat.S_IRGRP | stat.S_IXGRP | stat.S_IROTH + stat.S_IXOTH)
 
         executables = None
         if self.preamble:
@@ -373,23 +392,18 @@
                 f"{message} authentication error - screwed up / expired proxy? Renew / upload pilot proxy on machine?"
             )
         if result.isSet(arc.SubmissionStatus.ERROR_FROM_ENDPOINT):  # pylint: disable=no-member
             self.log.warn(f"{message} some error from the CE - possibly CE problems?")
         self.log.warn(f"{message} ... maybe above messages will give a hint.")
 
     #############################################################################
+    @prepareProxyToken
     def killJob(self, jobIDList):
         """Kill the specified jobs"""
 
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
-
         jobList = list(jobIDList)
         if isinstance(jobIDList, str):
             jobList = [jobIDList]
 
         self.log.debug(f"Killing jobs {jobIDList}")
         jobs = []
         for jobID in jobList:
@@ -402,33 +416,29 @@
             if not job_supervisor.Cancel():
                 errorString = " - ".join(jobList).strip()
                 return S_ERROR(f"Failed to kill at least one of these jobs: {errorString}. CE(?) not reachable?")
 
         return S_OK()
 
     #############################################################################
+    @prepareProxyToken
     def getCEStatus(self):
         """Method to return information on running and pending jobs.
         We hope to satisfy both instances that use robot proxies and those which use proper configurations.
         """
 
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
-
         # Try to find out which VO we are running for.
         vo = ""
         res = getVOfromProxyGroup()
         if res["OK"]:
             vo = res["Value"]
 
         result = S_OK()
         result["SubmittedJobs"] = 0
+
         if not vo:
             # Presumably the really proper way forward once the infosys-discuss WG comes up with a solution
             # and it is implemented. Needed for DIRAC instances which use robot certificates for pilots.
             if self.endpointType == "Gridftp":
                 endpoints = [
                     arc.Endpoint(
                         str("ldap://" + self.ceHost + "/MDS-Vo-name=local,o=grid"),
@@ -481,23 +491,18 @@
             except IndexError:
                 res = S_ERROR(f"Unknown ldap failure for site {self.ceHost}")
                 return res
 
         return result
 
     #############################################################################
+    @prepareProxyToken
     def getJobStatus(self, jobIDList):
         """Get the status information for the given list of jobs"""
 
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
-
         jobTmpList = list(jobIDList)
         if isinstance(jobIDList, str):
             jobTmpList = [jobIDList]
 
         # Pilots are stored with a DIRAC stamp (":::XXXXX") appended
         jobList = []
         for j in jobTmpList:
@@ -566,24 +571,20 @@
 
         if not resultDict:
             return S_ERROR("No job statuses returned")
 
         return S_OK(resultDict)
 
     #############################################################################
+    @prepareProxyToken
     def getJobOutput(self, jobID, workingDirectory=None):
         """Get the specified job standard output and error files.
         Standard output and error are returned as strings.
         If further outputs are retrieved, they are stored in workingDirectory.
         """
-        result = self._prepareProxy()
-        if not result["OK"]:
-            self.log.error("ARCComputingElement: failed to set up proxy", result["Message"])
-            return result
-        self.usercfg.ProxyPath(os.environ["X509_USER_PROXY"])
 
         if jobID.find(":::") != -1:
             pilotRef, stamp = jobID.split(":::")
         else:
             pilotRef = jobID
             stamp = ""
         if not stamp:
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/AREXComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/AREXComputingElement.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,23 @@
         if os.environ.get("BEARER_TOKEN"):
             self.headers["Authorization"] = "Bearer " + os.environ["BEARER_TOKEN"]
 
         return S_OK()
 
     #############################################################################
 
+    def setToken(self, token, valid):
+        """Set the token and update the headers
+
+        :param token: OAuth2Token object or dictionary containing token structure
+        :param int valid: validity period in seconds
+        """
+        super().setToken(token, valid)
+        self.headers["Authorization"] = "Bearer " + self.token["access_token"]
+
     def _arcToDiracID(self, arcJobID):
         """Convert an ARC jobID into a DIRAC jobID.
         Example: 1234 becomes https://<ce>:<port>/arex/1234
 
         :param str: ARC jobID
         :return: DIRAC jobID
         """
@@ -539,28 +548,39 @@
             timeLeft = timeLeftRes["Value"]
             if timeLeft < self.proxyTimeLeftBeforeRenewal:
                 self.log.debug(
                     "Renewing proxy for job",
                     f"{arcJob} whose proxy expires at {timeLeft}",
                 )
                 # Proxy needs to be renewed - try to renew it
+                # First, get a new CSR from the delegation
                 params = {"action": "renew"}
                 query = self._urlJoin(os.path.join("delegations", delegationID))
 
                 response = self.session.post(
                     query,
                     headers=self.headers,
                     params=params,
                     timeout=self.arcRESTTimeout,
                 )
+
                 if response.ok:
-                    self.log.debug("Proxy successfully renewed", f"for job {arcJob}")
+                    # Then, sign and upload the certificate
+                    result = self.__uploadCertificate(delegationID, response.text)
+                    if result["OK"]:
+                        self.log.debug("Proxy successfully renewed", f"for job {arcJob}")
+                    else:
+                        self.log.debug(
+                            "Proxy not renewed, failed to send renewed proxy",
+                            f"for job {arcJob} with delegation {delegationID}:",
+                            result["Message"],
+                        )
                 else:
                     self.log.debug(
-                        "Proxy not renewed",
+                        "Proxy not renewed, failed to get CSR",
                         f"for job {arcJob} with delegation {delegationID}",
                     )
             else:  # No need to renew. Proxy is long enough
                 continue
         return S_OK()
 
     #############################################################################
@@ -732,15 +752,15 @@
             return result
         self.session.cert = Locations.getProxyLocation()
 
         # Extract stamp from the Job ID
         if ":::" in jobID:
             jobRef, stamp = jobID.split(":::")
         else:
-            return S_ERROR(f"DIRAC stamp not defined for {jobRef}")
+            return S_ERROR(f"DIRAC stamp not defined for {jobID}")
         job = self._DiracToArcID(jobRef)
 
         # Get the list of available outputs
         result = self._getListOfAvailableOutputs(jobRef, job)
         if not result["OK"]:
             return result
         remoteOutputs = result["Value"]
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BOINCComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BOINCComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/Condor.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/Condor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/GE.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/GE.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/Host.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/Host.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/LSF.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/LSF.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/OAR.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/OAR.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/SLURM.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/SLURM.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/HTCondorResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/HTCondorResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/LSFResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/LSFResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/MJFResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/MJFResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/PBSResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/PBSResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/ResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/ResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SGEResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SGEResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SLURMResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/SLURMResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/TimeLeft.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/TimeLeft.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_LSFResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_LSFResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_PBSResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_PBSResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_SGEResourceUsage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_SGEResourceUsage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_TimeLeft.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/TimeLeft/test/Test_TimeLeft.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/Torque.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/Torque.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/executeBatch.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/executeBatch.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/BatchSystems/test/Test_SLURM.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/BatchSystems/test/Test_SLURM.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/CREAMComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/CREAMComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/CloudComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/CloudComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ComputingElement.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 
     def __init__(self, ceName):
         """Standard constructor"""
         self.log = gLogger.getSubLogger(ceName)
         self.ceName = ceName
         self.ceParameters = {}
         self.proxy = ""
+        self.token = None
         self.valid = None
         self.mandatoryParameters = []
         self.batchSystem = None
         self.taskResults = {}
         self.minProxyTime = gConfig.getValue("/Registry/MinProxyLifeTime", 10800)  # secs
         self.defaultProxyTime = gConfig.getValue("/Registry/DefaultProxyLifeTime", 43200)  # secs
         self.proxyCheckPeriod = gConfig.getValue("/Registry/ProxyCheckingPeriod", 3600)  # secs
@@ -79,15 +80,18 @@
         self.initializeParameters()
         self.log.debug("CE parameters", self.ceParameters)
 
     def setProxy(self, proxy, valid=0):
         """Set proxy for this instance"""
         self.proxy = proxy
         self.valid = datetime.datetime.utcnow() + second * valid
-        return S_OK()
+
+    def setToken(self, token, valid=0):
+        self.token = token
+        self.valid = datetime.datetime.utcnow() + second * valid
 
     def _prepareProxy(self):
         """Set the environment variable X509_USER_PROXY"""
         if not self.proxy:
             result = getProxyInfo()
             if not result["OK"]:
                 return S_ERROR("No proxy available")
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/ComputingElementFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/ComputingElementFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/HTCondorCEComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/HTCondorCEComputingElement.py`

 * *Files 9% similar despite different names*

```diff
@@ -32,37 +32,40 @@
    readable and writeable).  Also temporary files like condor submit files are kept here. This option is only read
    from the global Resources/Computing/HTCondorCE location.
 
 **Proxy renewal or lifetime**
 
 When not using a local condor_schedd, add ``delegate_job_GSI_credentials_lifetime = 0`` to the ``ExtraSubmitString``.
 
-When using a local condor_schedd look at the HTCondor documenation for enabling the proxy refresh.
+When using a local condor_schedd look at the HTCondor documentation for enabling the proxy refresh.
 
 **Code Documentation**
 """
 # Note: if you read this documentation in the source code and not via the sphinx
 # created documentation, there should only be one slash when setting the option,
 # but "\n" gets rendered as a linebreak in sphinx
 
 import datetime
 import errno
 import os
 import subprocess
 import tempfile
 import threading
+import textwrap
 
 from DIRAC import S_ERROR, S_OK, gConfig
 from DIRAC.Core.Utilities.File import makeGuid, mkDir
 from DIRAC.Core.Utilities.Grid import executeGridCommand
 from DIRAC.Core.Utilities.List import breakListIntoChunks
-from DIRAC.Resources.Computing.BatchSystems.Condor import parseCondorStatus, treatCondorHistory
 from DIRAC.Resources.Computing.ComputingElement import ComputingElement
 from DIRAC.WorkloadManagementSystem.Client import PilotStatus
 from DIRAC.WorkloadManagementSystem.Client.PilotManagerClient import PilotManagerClient
+from DIRAC.Core.Utilities.File import makeGuid
+from DIRAC.FrameworkSystem.private.authorization.utils.Tokens import writeToTokenFile
+from DIRAC.Resources.Computing.BatchSystems.Condor import parseCondorStatus
 
 MANDATORY_PARAMETERS = ["Queue"]
 DEFAULT_WORKINGDIRECTORY = "/opt/dirac/pro/runit/WorkloadManagement/SiteDirectorHT"
 DEFAULT_DAYSTOKEEPREMOTELOGS = 1
 DEFAULT_DAYSTOKEEPLOGS = 15
 
 
@@ -138,17 +141,18 @@
         # FIXME: just use gConfig.getValue("Resources/Computing/CEDefaults/HTCondorCE/WorkingDirectory", DEFAULT_WORKINGDIRECTORY) from v8.2
         self.workingDirectory = gConfig.getValue(
             "Resources/Computing/CEDefaults/HTCondorCE/WorkingDirectory",
             gConfig.getValue("Resources/Computing/HTCondorCE/WorkingDirectory", DEFAULT_WORKINGDIRECTORY),
         )
         self.useLocalSchedd = True
         self.remoteScheddOptions = ""
+        self.tokenFile = None
 
     #############################################################################
-    def __writeSub(self, executable, nJobs, location, processors, pilotStamps):
+    def __writeSub(self, executable, nJobs, location, processors, pilotStamps, tokenFile=None):
         """Create the Sub File for submission.
 
         :param str executable: name of the script to execute
         :param int nJobs: number of desired jobs
         :param str location: directory that should contain the result of the jobs
         :param int processors: number of CPU cores to allocate
         :param list pilotStamps: list of pilot stamps (strings)
@@ -162,14 +166,23 @@
         self.log.debug(f"ExtraSubmitString:\n### \n {self.extraSubmitString} \n###")
 
         fd, name = tempfile.mkstemp(suffix=".sub", prefix="HTCondorCE_", dir=self.workingDirectory)
         subFile = os.fdopen(fd, "w")
 
         executable = os.path.join(self.workingDirectory, executable)
 
+        useCredentials = ""
+        if tokenFile:
+            useCredentials = textwrap.dedent(
+                f"""
+                use_scitokens = true
+                scitokens_file = {tokenFile}
+                """
+            )
+
         # This is used to remove outputs from the remote schedd
         # Used in case a local schedd is not used
         periodicRemove = "periodic_remove = "
         periodicRemove += "(JobStatus == 4) && "
         periodicRemove += f"(time() - EnteredCurrentStatus) > ({self.daysToKeepRemoteLogs} * 24 * 3600)"
 
         localScheddOptions = (
@@ -183,14 +196,15 @@
 
         targetUniverse = "grid" if self.useLocalSchedd else "vanilla"
 
         sub = """
 executable = %(executable)s
 universe = %(targetUniverse)s
 use_x509userproxy = true
+%(useCredentials)s
 output = $(Cluster).$(Process).out
 error = $(Cluster).$(Process).err
 log = $(Cluster).$(Process).log
 environment = "HTCONDOR_JOBID=$(Cluster).$(Process) DIRAC_PILOT_STAMP=$(stamp)"
 initialdir = %(initialDir)s
 grid_resource = condor %(ceName)s %(ceName)s:9619
 transfer_output_files = ""
@@ -209,14 +223,15 @@
             processors=processors,
             ceName=self.ceName,
             extraString=self.extraSubmitString,
             initialDir=os.path.join(self.workingDirectory, location),
             localScheddOptions=localScheddOptions,
             targetUniverse=targetUniverse,
             pilotStampList=",".join(pilotStamps),
+            useCredentials=useCredentials,
         )
         subFile.write(sub)
         subFile.close()
         return name
 
     def _reset(self):
         self.queue = self.ceParameters["Queue"]
@@ -232,14 +247,48 @@
 
         self.remoteScheddOptions = "" if self.useLocalSchedd else f"-pool {self.ceName}:9619 -name {self.ceName} "
 
         self.log.debug("Using local schedd:", self.useLocalSchedd)
         self.log.debug("Remote scheduler option:", self.remoteScheddOptions)
         return S_OK()
 
+    def _executeCondorCommand(self, cmd, keepTokenFile=False):
+        """Execute condor command in a specially prepared environment
+
+        :param list cmd: list of the condor command elements
+        :param bool keepTokenFile: flag to reuse or not the previously created token file
+        :return: S_OK/S_ERROR - the result of the executeGridCommand() call
+        """
+
+        if self.token:
+            # Create a new token file if we do not keep it across several calls
+            if not self.tokenFile or not keepTokenFile:
+                self.tokenFile = tempfile.NamedTemporaryFile(
+                    suffix=".token", prefix="HTCondorCE_", dir=self.workingDirectory
+                )
+                writeToTokenFile(self.token["access_token"], self.tokenFile.name)
+
+            htcEnv = {
+                "_CONDOR_SEC_CLIENT_AUTHENTICATION_METHODS": "SCITOKENS",
+                "_CONDOR_SCITOKENS_FILE": self.tokenFile.name,
+            }
+        else:
+            htcEnv = {"_CONDOR_SEC_CLIENT_AUTHENTICATION_METHODS": "GSI"}
+
+        result = executeGridCommand(
+            self.proxy,
+            cmd,
+            gridEnvScript=self.gridEnv,
+            gridEnvDict=htcEnv,
+        )
+        # Remove token file if we do not want to keep it
+        self.tokenFile = self.tokenFile if keepTokenFile else None
+
+        return result
+
     #############################################################################
     def submitJob(self, executableFile, proxy, numberOfJobs=1):
         """Method to submit job"""
 
         self.log.verbose("Executable file path:", executableFile)
         if not os.access(executableFile, 5):
             os.chmod(executableFile, 0o755)
@@ -251,36 +300,46 @@
         for _i in range(numberOfJobs):
             jobStamp = commonJobStampPart + makeGuid()[:5]
             jobStamps.append(jobStamp)
 
         # We randomize the location of the pilot output and log, because there are just too many of them
         location = logDir(self.ceName, commonJobStampPart)
         nProcessors = self.ceParameters.get("NumberOfProcessors", 1)
-        subName = self.__writeSub(executableFile, numberOfJobs, location, nProcessors, jobStamps)
+        if self.token:
+            self.tokenFile = tempfile.NamedTemporaryFile(
+                suffix=".token", prefix="HTCondorCE_", dir=self.workingDirectory
+            )
+            writeToTokenFile(self.token["access_token"], self.tokenFile.name)
+        subName = self.__writeSub(
+            executableFile, numberOfJobs, location, nProcessors, jobStamps, tokenFile=self.tokenFile
+        )
 
         cmd = ["condor_submit", "-terse", subName]
         # the options for submit to remote are different than the other remoteScheddOptions
         # -remote: submit to a remote condor_schedd and spool all the required inputs
         scheddOptions = [] if self.useLocalSchedd else ["-pool", f"{self.ceName}:9619", "-remote", self.ceName]
         for op in scheddOptions:
             cmd.insert(-1, op)
 
-        result = executeGridCommand(self.proxy, cmd, self.gridEnv)
+        result = self._executeCondorCommand(cmd, keepTokenFile=True)
         self.log.verbose(result)
         os.remove(subName)
+        self.tokenFile = None
         if not result["OK"]:
             self.log.error("Failed to submit jobs to htcondor", result["Message"])
             return result
 
-        if result["Value"][0]:
+        status, stdout, stderr = result["Value"]
+
+        if status:
             # We have got a non-zero status code
-            errorString = result["Value"][2] if result["Value"][2] else result["Value"][1]
+            errorString = stderr if stderr else stdout
             return S_ERROR(f"Pilot submission failed with error: {errorString.strip()}")
 
-        pilotJobReferences = self.__getPilotReferences(result["Value"][1].strip())
+        pilotJobReferences = self.__getPilotReferences(stdout.strip())
         if not pilotJobReferences["OK"]:
             return pilotJobReferences
         pilotJobReferences = pilotJobReferences["Value"]
 
         self.log.verbose("JobStamps:", jobStamps)
         self.log.verbose("pilotRefs:", pilotJobReferences)
 
@@ -299,28 +358,34 @@
         if not jobIDList:
             return S_OK()
         if isinstance(jobIDList, str):
             jobIDList = [jobIDList]
 
         self.log.verbose("KillJob jobIDList", jobIDList)
 
+        self.tokenFile = None
+
         for jobRef in jobIDList:
             job, _, jobID = condorIDAndPathToResultFromJobRef(jobRef)
             self.log.verbose("Killing pilot", job)
             cmd = ["condor_rm"]
             cmd.extend(self.remoteScheddOptions.strip().split(" "))
             cmd.append(jobID)
-            result = executeGridCommand(self.proxy, cmd, self.gridEnv)
+            result = self._executeCondorCommand(cmd, keepTokenFile=True)
             if not result["OK"]:
+                self.tokenFile = None
                 return S_ERROR(f"condor_rm failed completely: {result['Message']}")
             status, stdout, stderr = result["Value"]
             if status != 0:
                 self.log.warn("Failed to kill pilot", f"{job}: {stdout}, {stderr}")
+                self.tokenFile = None
                 return S_ERROR(f"Failed to kill pilot {job}: {stderr}")
 
+        self.tokenFile = None
+
         return S_OK()
 
     #############################################################################
     def getCEStatus(self):
         """Method to return information on running and pending jobs.
 
         Warning: information currently returned depends on the PilotManager and not HTCondor.
@@ -362,48 +427,81 @@
         resultDict = {}
         condorIDs = {}
         # Get all condorIDs so we can just call condor_q and condor_history once
         for jobRef in jobIDList:
             job, _, jobID = condorIDAndPathToResultFromJobRef(jobRef)
             condorIDs[job] = jobID
 
+        self.tokenFile = None
+
         qList = []
         for _condorIDs in breakListIntoChunks(condorIDs.values(), 100):
             # This will return a list of 1245.75 3
-            status, stdout_q = subprocess.getstatusoutput(
-                f"condor_q {self.remoteScheddOptions} {' '.join(_condorIDs)} -af:j JobStatus "
-            )
+            cmd = ["condor_q"]
+            cmd.extend(self.remoteScheddOptions.strip().split(" "))
+            cmd.extend(_condorIDs)
+            cmd.extend(["-af:j", "JobStatus"])
+            result = self._executeCondorCommand(cmd, keepTokenFile=True)
+            if not result["OK"]:
+                self.tokenFile = None
+                return S_ERROR(f"condor_q failed completely: {result['Message']}")
+            status, stdout, stderr = result["Value"]
             if status != 0:
-                return S_ERROR(stdout_q)
-            _qList = stdout_q.strip().split("\n")
+                self.tokenFile = None
+                return S_ERROR(stdout + stderr)
+            _qList = stdout.strip().split("\n")
             qList.extend(_qList)
 
             # FIXME: condor_history does only support j for autoformat from 8.5.3,
             # format adds whitespace for each field This will return a list of 1245 75 3
-            # needs to cocatenate the first two with a dot
-            condorHistCall = "condor_history {} {} -af ClusterId ProcId JobStatus".format(
-                self.remoteScheddOptions,
-                " ".join(_condorIDs),
-            )
+            # needs to concatenate the first two with a dot
+            condorHistCall = ["condor_history"]
+            condorHistCall.extend(self.remoteScheddOptions.strip().split(" "))
+            condorHistCall.extend(_condorIDs)
+            condorHistCall.extend(["-af", "ClusterId", "ProcId", "JobStatus"])
 
-            treatCondorHistory(condorHistCall, qList)
+            self._treatCondorHistory(condorHistCall, qList)
 
         for job, jobID in condorIDs.items():
             pilotStatus = parseCondorStatus(qList, jobID)
             if pilotStatus == "HELD":
                 # make sure the pilot stays dead and gets taken out of the condor_q
-                _rmStat, _rmOut = subprocess.getstatusoutput(f"condor_rm {self.remoteScheddOptions} {jobID} ")
-                # self.log.debug( "condor job killed: job %s, stat %s, message %s " % ( jobID, rmStat, rmOut ) )
+                cmd = f"condor_rm {self.remoteScheddOptions} {jobID}".split()
+                _result = self._executeCondorCommand(cmd, keepTokenFile=True)
                 pilotStatus = PilotStatus.ABORTED
 
             resultDict[job] = pilotStatus
 
+        self.tokenFile = None
+
         self.log.verbose(f"Pilot Statuses: {resultDict} ")
         return S_OK(resultDict)
 
+    def _treatCondorHistory(self, condorHistCall, qList):
+        """concatenate clusterID and processID to get the same output as condor_q
+        until we can expect condor version 8.5.3 everywhere
+
+        :param str condorHistCall: condor_history command to run
+        :param list qList: list of jobID and status from condor_q output, will be modified in this function
+        :returns: None
+        """
+
+        result = self._executeCondorCommand(condorHistCall)
+        if not result["OK"]:
+            return S_ERROR(f"condorHistCall failed completely: {result['Message']}")
+
+        status_history, stdout_history, stderr_history = result["Value"]
+
+        # Join the ClusterId and the ProcId and add to existing list of statuses
+        if status_history == 0:
+            for line in stdout_history.split("\n"):
+                values = line.strip().split()
+                if len(values) == 3:
+                    qList.append("%s.%s %s" % tuple(values))
+
     def getJobLog(self, jobID):
         """Get pilot job logging info from HTCondor
 
         :param str jobID: pilot job identifier
         :return: string representing the logging info of a given pilot job
         """
         self.log.verbose("Getting logging info for jobID", jobID)
@@ -440,28 +538,29 @@
         except OSError as e:
             errorMessage = "Failed to create the pilot output directory"
             self.log.exception(errorMessage, iwd)
             return S_ERROR(e.errno, f"{errorMessage} ({iwd})")
 
         if not self.useLocalSchedd:
             cmd = ["condor_transfer_data", "-pool", f"{self.ceName}:9619", "-name", self.ceName, condorID]
-            result = executeGridCommand(self.proxy, cmd, self.gridEnv)
+            result = self._executeCondorCommand(cmd)
             self.log.verbose(result)
 
             # Getting 'logging' without 'error' and 'output' is possible but will generate command errors
             # We do not check the command errors if we only want 'logging'
             if "error" in outTypes or "output" in outTypes:
                 errorMessage = "Failed to get job output from htcondor"
                 if not result["OK"]:
                     self.log.error(errorMessage, result["Message"])
                     return result
                 # Even if result is OK, the actual exit code of cmd can still be an error
-                if result["OK"] and result["Value"][0] != 0:
-                    outMessage = result["Value"][1].strip()
-                    errMessage = result["Value"][2].strip()
+                status, stdout, stderr = result["Value"]
+                if status != 0:
+                    outMessage = stdout.strip()
+                    errMessage = stderr.strip()
                     varMessage = outMessage + " " + errMessage
                     self.log.error(errorMessage, varMessage)
                     return S_ERROR(f"{errorMessage}: {varMessage}")
 
         outputsSuffix = {"output": "out", "error": "err", "logging": "log"}
         outputs = {}
         for output, suffix in outputsSuffix.items():
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/InProcessComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/InProcessComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/LocalComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/LocalComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/PilotBundle.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/PilotBundle.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/PoolComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/PoolComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SSHBatchComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SSHBatchComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SSHComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SSHComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SingularityComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SingularityComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/SudoComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/SudoComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/cloudinit.template` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/cloudinit.template`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_HTCondorCEComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_HTCondorCEComputingElement.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,22 @@
 
     for jobID, expected in expectedResults.items():
         assert HTCE.parseCondorStatus(statusLines, jobID) == expected
 
 
 def test_getJobStatus(mocker):
     """Test HTCondorCE getJobStatus"""
-    mocker.patch(MODNAME + ".subprocess.getstatusoutput", side_effect=([(0, "\n".join(STATUS_LINES)), (0, 0)]))
-    patchPopen = mocker.patch("DIRAC.Resources.Computing.BatchSystems.Condor.subprocess.Popen")
-    patchPopen.return_value.communicate.side_effect = [("\n".join(HISTORY_LINES), "")]
-    patchPopen.return_value.returncode = 0
+    mocker.patch(
+        MODNAME + ".executeGridCommand",
+        side_effect=[
+            S_OK((0, "\n".join(STATUS_LINES), "")),
+            S_OK((0, "\n".join(HISTORY_LINES), "")),
+            S_OK((0, "", "")),
+        ],
+    )
     mocker.patch(MODNAME + ".HTCondorCEComputingElement._HTCondorCEComputingElement__cleanup")
 
     htce = HTCE.HTCondorCEComputingElement(12345)
     ret = htce.getJobStatus(
         [
             "htcondorce://condorce.foo.arg/123.0:::abc321",
             "htcondorce://condorce.foo.arg/123.1:::c3b2a1",
@@ -162,15 +166,15 @@
     ceParameters = setUp
     htce = HTCE.HTCondorCEComputingElement(12345)
     htce.ceParameters = ceParameters
     htce.useLocalSchedd = localSchedd
     ceName = "condorce.cern.ch"
     htce.ceName = ceName
 
-    execMock = mocker.patch(MODNAME + ".executeGridCommand", return_value=S_OK((0, "123.0 - 123.0")))
+    execMock = mocker.patch(MODNAME + ".executeGridCommand", return_value=S_OK((0, "123.0 - 123.0", "")))
     mocker.patch(
         MODNAME + ".HTCondorCEComputingElement._HTCondorCEComputingElement__writeSub", return_value="dirac_pilot"
     )
     mocker.patch(MODNAME + ".os")
 
     result = htce.submitJob("pilot", "proxy", 1)
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_InProcessComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_InProcessComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_PoolComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_PoolComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Computing/test/Test_SSHComputingElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Computing/test/Test_SSHComputingElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/CheckInIdProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/CheckInIdProvider.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ IdProvider based on OAuth2 protocol
 """
 from authlib.oauth2.rfc6749.util import scope_to_list
 
-from DIRAC import S_OK
 from DIRAC.Resources.IdProvider.OAuth2IdProvider import OAuth2IdProvider
 from DIRAC.ConfigurationSystem.Client.Helpers.Registry import getVOForGroup, getGroupOption
 
 
 class CheckInIdProvider(OAuth2IdProvider):
     def getGroupScopes(self, group):
         """Get group scopes
@@ -17,8 +16,8 @@
         """
         idPScope = getGroupOption(group, "IdPRole")
         if not idPScope:
             idPScope = "eduperson_entitlement?value=urn:mace:egi.eu:group:{}:role={}#aai.egi.eu".format(
                 getVOForGroup(group),
                 group.split("_")[1],
             )
-        return S_OK(scope_to_list(idPScope))
+        return scope_to_list(idPScope)
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/IAMIdProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/IAMIdProvider.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """ IdProvider based on OAuth2 protocol
 """
 from authlib.oauth2.rfc6749.util import scope_to_list
 
-from DIRAC import S_OK
 from DIRAC.Resources.IdProvider.OAuth2IdProvider import OAuth2IdProvider
 from DIRAC.ConfigurationSystem.Client.Helpers.Registry import getVOForGroup, getGroupOption
 
 
 class IAMIdProvider(OAuth2IdProvider):
     def getGroupScopes(self, group):
         """Get group scopes
@@ -14,8 +13,8 @@
         :param str group: DIRAC group
 
         :return: list
         """
         idPScope = getGroupOption(group, "IdPRole")
         if not idPScope:
             idPScope = f"wlcg.groups:/{getVOForGroup(group)}/{group.split('_')[1]}"
-        return S_OK(scope_to_list(idPScope))
+        return scope_to_list(idPScope)
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/IdProviderFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/IdProviderFactory.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 class IdProviderFactory:
     def __init__(self):
         """Standard constructor"""
         self.log = gLogger.getSubLogger(self.__class__.__name__)
         self.cacheMetadata = DictCache()
 
     @gCacheMetadata
-    def getMetadata(self, idP):
-        return self.cacheMetadata.get(idP) or {}
+    def getMetadata(self, idProvider):
+        return self.cacheMetadata.get(idProvider) or {}
 
     @gCacheMetadata
-    def addMetadata(self, idP, data, time=24 * 3600):
+    def addMetadata(self, idProvider, data, time=24 * 3600):
         if data:
-            self.cacheMetadata.add(idP, time, data)
+            self.cacheMetadata.add(idProvider, time, data)
 
     def getIdProviderForToken(self, token):
         """This method returns a IdProvider instance corresponding to the supplied
         issuer in a token.
 
         :param token: access token or dict with access_token key
 
@@ -68,15 +68,15 @@
         try:
             asMetaDict = collectMetadata(kwargs.get("issuer"), ignoreErrors=True)
         except Exception as e:
             return S_ERROR(str(e))
         self.log.debug("Search configuration for", name)
         clients = getDIRACClients()
         if name in clients:
-            # If it is a DIRAC default pre-registred client
+            # If it is a DIRAC default pre-registered client
             pDict = asMetaDict
             pDict.update(clients[name])
         else:
             # if it is external identity provider client
             result = getProviderInfo(name)
             if not result["OK"]:
                 self.log.error("Failed to read configuration", f"{name}: {result['Message']}")
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/OAuth2IdProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/OAuth2IdProvider.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,24 +10,22 @@
 from authlib.oauth2.rfc6749.util import scope_to_list, list_to_scope
 from authlib.oauth2.rfc6749.parameters import prepare_token_request
 from authlib.oauth2.rfc8628 import DEVICE_CODE_GRANT_TYPE
 from authlib.integrations.requests_client import OAuth2Session as _OAuth2Session
 from authlib.oidc.discovery.well_known import get_well_known_url
 from authlib.oauth2.rfc7636 import create_s256_code_challenge
 
-
-from DIRAC import S_OK, S_ERROR
+from DIRAC import S_OK, S_ERROR, gLogger
 from DIRAC.Core.Utilities import ThreadSafe
-from DIRAC.Resources.IdProvider.IdProvider import IdProvider
 from DIRAC.ConfigurationSystem.Client.Helpers.Registry import (
     getVOMSRoleGroupMapping,
-    getGroupOption,
-    getAllGroups,
     wrapIDAsDN,
     getVOs,
+    getGroupOption,
+    getAllGroups,
 )
 from DIRAC.FrameworkSystem.private.authorization.utils.Tokens import OAuth2Token
 from DIRAC.FrameworkSystem.private.authorization.utils.Requests import createOAuth2Request
 
 DEFAULT_HEADERS = {"Accept": "application/json", "Content-Type": "application/x-www-form-urlencoded;charset=UTF-8"}
 
 gJWKs = ThreadSafe.Synchronizer()
@@ -40,15 +38,14 @@
 
     :param dict claimDict: claims
     :param dict attributes: contain claim and regex to parse it
 
     :return: dict
     """
     profile = {}
-    result = None
     for claim, reg in attributes.items():
         if claim not in claimDict:
             continue
         profile[claim] = {}
         if isinstance(claimDict[claim], dict):
             result = claimParser(claimDict[claim], reg)
             if result:
@@ -145,60 +142,92 @@
 
         if callable(self.update_token):
             self.update_token(self.token, refresh_token=refresh_token)
 
         return self.token
 
 
-class OAuth2IdProvider(IdProvider, OAuth2Session):
+class OAuth2IdProvider(OAuth2Session):
     """Base class to describe the configuration of the OAuth2 client of the corresponding provider."""
 
     JWKS_REFRESH_RATE = 24 * 3600
     METADATA_REFRESH_RATE = 24 * 3600
+    DEFAULT_METADATA = {}
 
     def __init__(self, **kwargs):
         """Initialization"""
-        IdProvider.__init__(self, **kwargs)
         OAuth2Session.__init__(self, **kwargs)
+        self.log = gLogger.getSubLogger(self.__class__.__name__)
         self.metadata_fetch_last = 0
         self.issuer = self.metadata["issuer"]
         self.scope = self.scope or ""
         self.jwks = kwargs.get("jwks")
         self.verify = kwargs.get("verify", True)  # Decide if need to check CAs
         self.token_placement = kwargs.get("token_placement", "header")
         self.code_challenge_method = "S256"
         # self.token_endpoint_auth_method = kwargs.get('token_endpoint_auth_method') #, 'client_secret_post')
         self.server_metadata_url = kwargs.get("server_metadata_url", get_well_known_url(self.metadata["issuer"], True))
         self.jwks_fetch_last = time.time() - self.JWKS_REFRESH_RATE
+        meta = self.DEFAULT_METADATA
+        meta.update(kwargs)
+        self.setParameters(meta)
+        self._initialize()
         self.metadata_fetch_last = time.time() - self.METADATA_REFRESH_RATE
         self.log.debug(
             f'"{self.name}" OAuth2 IdP initialization done:',
             "\nclient_id: %s\nclient_secret: %s\nmetadata:\n%s"
             % (self.client_id, self.client_secret, pprint.pformat(self.metadata)),
         )
 
+    def _initialize(self):
+        """Initialization"""
+        self.name = self.parameters.get("ProviderName")
+
+    def setParameters(self, parameters: dict):
+        """Set parameters
+
+        :param dict parameters: parameters of the identity Provider
+        """
+        self.parameters = parameters
+
     def get_metadata(self, option=None):
         """Get metadata
 
         :param str option: option
 
         :return: option value
         """
         if not self.metadata.get(option):
             self.fetch_metadata()
         return self.metadata.get(option)
 
     @gMetadata
     def fetch_metadata(self):
-        """Fetch metada"""
+        """Fetch metadata"""
         if self.metadata_fetch_last < (time.time() - self.METADATA_REFRESH_RATE):
             data = self.get(self.server_metadata_url, withhold_token=True).json()
             self.metadata.update(data)
             self.metadata_fetch_last = time.time()
 
+    def getGroupScopes(self, group: str) -> list[str]:
+        """Get group scopes
+
+        :param group: DIRAC group
+        """
+        idPScope = getGroupOption(group, "IdPRole")
+        return scope_to_list(idPScope) if idPScope else []
+
+    def getScopeGroups(self, scope: str) -> list[str]:
+        """Get DIRAC groups related to scope"""
+        groups = []
+        for group in getAllGroups():
+            if (g_scope := self.getGroupScopes(group)) and set(g_scope).issubset(scope_to_list(scope)):
+                groups.append(group)
+        return groups
+
     @gJWKs
     def updateJWKs(self):
         """Update JWKs"""
         if self.jwks_fetch_last < (time.time() - self.JWKS_REFRESH_RATE):
             try:
                 self.jwks = self.get(self.get_metadata("jwks_uri"), withhold_token=True).json()
                 self.jwks_fetch_last = time.time()
@@ -334,15 +363,15 @@
         if not payload and token:
             payload = OAuth2Token(token).get_payload()
 
         credDict = self.parseBasic(payload)
         if not credDict.get("DIRACGroups"):
             credDict.update(self.parseEduperson(payload))
         if credDict.get("DIRACGroups"):
-            self.log.debug("Found next groups:", ", ".join(credDict["DIRACGroups"]))
+            self.log.debug("Found groups:", ", ".join(credDict["DIRACGroups"]))
             credDict["group"] = credDict["DIRACGroups"][0]
         return S_OK(credDict)
 
     def parseBasic(self, claimDict):
         """Parse basic claims
 
         :param dict claimDict: claims
@@ -395,15 +424,15 @@
                     for role in vos[vo]["VORoles"]:
                         groups = result["Value"]["VOMSDIRAC"].get(f"/{vo}/{role}")
                         if groups:
                             credDict["DIRACGroups"] = list(set(credDict.get("DIRACGroups", []) + groups))
         return credDict
 
     def deviceAuthorization(self, group=None):
-        """Authorizaion through DeviceCode flow"""
+        """Authorization through DeviceCode flow"""
         result = self.submitDeviceCodeAuthorizationFlow(group)
         if not result["OK"]:
             return result
         response = result["Value"]
 
         # Notify user to go to authorization endpoint
         if response.get("verification_uri_complete"):
@@ -523,37 +552,21 @@
             r = requests.post(
                 self.get_metadata("token_endpoint"),
                 data=dict(client_id=self.client_id, grant_type=DEVICE_CODE_GRANT_TYPE, device_code=deviceCode),
                 verify=self.verify,
             )
             token = r.json()
             if not token:
-                return S_ERROR("Resived token is empty!")
+                return S_ERROR("Received token is empty!")
             if "error" not in token:
                 self.token = token
                 return S_OK(token)
             if token["error"] != "authorization_pending":
                 return S_ERROR((token.get("error") or "unknown") + " : " + (token.get("error_description") or ""))
 
-    def getGroupScopes(self, group: str) -> list:
-        """Get group scopes
-
-        :param group: DIRAC group
-        """
-        idPScope = getGroupOption(group, "IdPRole")
-        return scope_to_list(idPScope) if idPScope else []
-
-    def getScopeGroups(self, scope: str) -> list:
-        """Get DIRAC groups related to scope"""
-        groups = []
-        for group in getAllGroups():
-            if (g_scope := self.getGroupScopes(group)) and set(g_scope).issubset(scope_to_list(scope)):
-                groups.append(group)
-        return groups
-
     def getUserProfile(self):
         """Get user profile
 
         :return: S_OK()/S_ERROR()
         """
         try:
             return S_OK(self.get(self.get_metadata("userinfo_endpoint")).json())
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/IdProvider/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/IdProvider/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/AbstractBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/AbstractBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/ElasticSearchBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/ElasticSearchBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/FileBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/FileBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/MessageQueueBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/MessageQueueBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/StderrBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/StderrBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/StdoutBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/StdoutBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogBackends/StdoutJsonBackend.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogBackends/StdoutJsonBackend.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/ModuleFilter.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/ModuleFilter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/PatternFilter.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/PatternFilter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/SensitiveDataFilter.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/SensitiveDataFilter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/LogFilters/test/Test_LogFilter.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/LogFilters/test/Test_LogFilter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQCommunication.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQCommunication.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQConnectionManager.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQConnectionManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQConnector.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQConnector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQConsumer.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQConsumer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/MQProducer.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/MQProducer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/Simple/StompInterface.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/Simple/StompInterface.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/StompMQConnector.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/StompMQConnector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQConnectionManager.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQConnectionManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQConsumer.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQConsumer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQProducer.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQProducer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/MessageQueue/test/Test_MQ_Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/MessageQueue/test/Test_MQ_Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/DIRACCAProxyProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/DIRACCAProxyProvider.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/PUSPProxyProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/PUSPProxyProvider.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/ProxyProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/ProxyProvider.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/ProxyProviderFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/ProxyProviderFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/test/Test_DIRACCAProxyProvider.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/test/Test_DIRACCAProxyProvider.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/ProxyProvider/test/Test_ProxyProviderFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/ProxyProvider/test/Test_ProxyProviderFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/CTAStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/CTAStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/DIPStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/DIPStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/EchoStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/EchoStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/FCOnlyStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/FCOnlyStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/FileStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_GSIFTPStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_GSIFTPStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_HTTPSStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_HTTPSStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_SRM2Storage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_SRM2Storage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_StorageBase.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_StorageBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/GFAL2_XROOTStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/GFAL2_XROOTStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/BDIIOccupancy.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/BDIIOccupancy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingHTTPJson.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingHTTPJson.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingJson.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/OccupancyPlugins/WLCGAccountingJson.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/RFIOStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/RFIOStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/S3Storage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/S3Storage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/StorageBase.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/StorageBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/StorageElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/StorageElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/StorageFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/StorageFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/FIXME_Test_RFIOPlugIn.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/FIXME_Test_RFIOPlugIn.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/FIXME_Test_StorageElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/FIXME_Test_StorageElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/FIXME_Test_StoragePlugIn.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/FIXME_Test_StoragePlugIn.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_FilePlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_FilePlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_GFAL2_XROOTStorage.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_GFAL2_XROOTStorage.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_StorageElement.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_StorageElement.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/Test_StorageFactory.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/Test_StorageFactory.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/Storage/test/test_utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/Storage/test/test_utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/scripts/dirac_resource_get_parameters.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/scripts/dirac_resource_get_parameters.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Resources/scripts/dirac_resource_info.py` & `DIRAC-8.1.0a9/src/DIRAC/Resources/scripts/dirac_resource_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/RequestFinalizationAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/RequestFinalizationAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/RequestPreparationAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/RequestPreparationAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/StageMonitorAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/StageMonitorAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Agent/StageRequestAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Agent/StageRequestAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/StorageManagerClient.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/StorageManagerClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Client/test/Test_Client_StorageManagementSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Client/test/Test_Client_StorageManagementSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/DB/StorageManagementDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Service/StorageManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Service/StorageManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/Service/TornadoStorageManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/Service/TornadoStorageManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_file.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_file.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_jobs.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_jobs.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_request.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_request.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_requests.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_monitor_requests.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_show_stats.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_show_stats.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_stage_files.py` & `DIRAC-8.1.0a9/src/DIRAC/StorageManagementSystem/scripts/dirac_stager_stage_files.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/DataRecoveryAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/DataRecoveryAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/InputDataAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/InputDataAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/MCExtensionAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/MCExtensionAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/RequestOperations/SetFileStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/RequestOperations/SetFileStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/RequestTaskAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/RequestTaskAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TaskManagerAgentBase.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TaskManagerAgentBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationAgentsUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationAgentsUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/TransformationPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/TransformationPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/ValidateOutputDataAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/WorkflowTaskAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/test/Test_Agent_TransformationSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/test/Test_Agent_TransformationSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Agent/test/Test_Plugins.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Agent/test/Test_Plugins.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/BodyPlugin/BaseBody.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/BodyPlugin/BaseBody.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/BodyPlugin/DummyBody.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/BodyPlugin/DummyBody.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/FileReport.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/FileReport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/PluginBase.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/PluginBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/RequestTasks.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/RequestTasks.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TaskManager.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TaskManager.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TaskManagerPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TaskManagerPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/Transformation.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/Transformation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationCLI.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationCLI.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationClient.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationFilesStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationFilesStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/TransformationStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/TransformationStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/WorkflowTasks.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/WorkflowTasks.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_RequestTasks.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_RequestTasks.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_TaskManagerPlugin.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_TaskManagerPlugin.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationClient.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_TransformationSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Client/test/Test_Client_WorkflowTasks.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Client/test/Test_Client_WorkflowTasks.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/ConfigTemplate.cfg`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/DB/TransformationDB.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/DB/TransformationDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/DB/TransformationDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/DB/TransformationDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Service/TransformationManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Service/TransformationManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/JobInfo.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/JobInfo.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/ReplicationCLIParameters.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/ReplicationCLIParameters.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/ReplicationTransformation.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/ReplicationTransformation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/ScriptUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/ScriptUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/Utilities/TransformationInfo.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/Utilities/TransformationInfo.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_production_runjoblocal.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_add_files.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_archive.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_archive.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_clean.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_clean.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_get_files.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_get_files.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_information.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_information.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_recover_data.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_recover_data.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_remove_output.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_remove_output.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_replication.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_replication.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_update_derived.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_update_derived.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/scripts/dirac_transformation_verify_outputdata.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/scripts/dirac_transformation_verify_outputdata.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_DRA.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_DRA.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_JobInfo.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_JobInfo.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_TransformationInfo.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_TransformationInfo.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/TransformationSystem/test/Test_replicationTransformation.py` & `DIRAC-8.1.0a9/src/DIRAC/TransformationSystem/test/Test_replicationTransformation.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/FailoverRequest.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/FailoverRequest.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/ModuleBase.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/ModuleBase.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/Script.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/Script.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/UploadOutputs.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/UploadOutputs.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Modules/test/Test_Modules.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Modules/test/Test_Modules.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/Utils.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/Utils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/Workflow/Utilities/test/Test_Utilities.py` & `DIRAC-8.1.0a9/src/DIRAC/Workflow/Utilities/test/Test_Utilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/JobAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/JobAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/JobCleaningAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/JobCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/OptimizerModule.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/OptimizerModule.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/PilotStatusAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/PilotStatusAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/PilotSyncAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/PilotSyncAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/PushJobAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/PushJobAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/SiteDirector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/SiteDirector.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from DIRAC.ConfigurationSystem.Client.Helpers import CSGlobals, Registry
 from DIRAC.ConfigurationSystem.Client.Helpers.Operations import Operations
 from DIRAC.ConfigurationSystem.Client.Helpers.Resources import getCESiteMapping
 from DIRAC.Core.Base.AgentModule import AgentModule
 from DIRAC.Core.Utilities.ObjectLoader import ObjectLoader
 from DIRAC.Core.Utilities.TimeUtilities import second, toEpochMilliSeconds
 from DIRAC.FrameworkSystem.Client.ProxyManagerClient import gProxyManager
+from DIRAC.FrameworkSystem.Client.TokenManagerClient import gTokenManager
 from DIRAC.MonitoringSystem.Client.MonitoringReporter import MonitoringReporter
 from DIRAC.ResourceStatusSystem.Client.ResourceStatus import ResourceStatus
 from DIRAC.ResourceStatusSystem.Client.SiteStatus import SiteStatus
 from DIRAC.WorkloadManagementSystem.Client import PilotStatus
 from DIRAC.WorkloadManagementSystem.Client.MatcherClient import MatcherClient
 from DIRAC.WorkloadManagementSystem.Client.ServerUtils import pilotAgentsDB
 from DIRAC.WorkloadManagementSystem.private.ConfigHelper import findGenericPilotCredentials
@@ -210,24 +211,30 @@
             ceTypes = ceTypesOption
 
         ces = None
         cesOption = self.am_getOption("CEs", ["any"])
         if cesOption and "any" not in [ce.lower() for ce in cesOption]:
             ces = cesOption
 
+        tags = self.am_getOption("Tags", [])
+        if not tags:
+            tags = None
+
         self.log.always("VO:", self.vo)
         if self.voGroups:
             self.log.always("Group(s):", self.voGroups)
         self.log.always("Sites:", siteNames)
         self.log.always("CETypes:", ceTypes)
         self.log.always("CEs:", ces)
         self.log.always("PilotDN:", self.pilotDN)
         self.log.always("PilotGroup:", self.pilotGroup)
 
-        result = self.resourcesModule.getQueues(community=self.vo, siteList=siteNames, ceList=ces, ceTypeList=ceTypes)
+        result = self.resourcesModule.getQueues(
+            community=self.vo, siteList=siteNames, ceList=ces, ceTypeList=ceTypes, tags=tags
+        )
         if not result["OK"]:
             return result
         result = getQueuesResolved(
             siteDict=result["Value"],
             queueCECache=self.queueCECache,
             gridEnv=self.gridEnv,
             setup=gConfig.getValue("/DIRAC/Setup", "unknown"),
@@ -430,14 +437,21 @@
             # Check returned proxy lifetime
             result = proxy.getRemainingSecs()  # pylint: disable=no-member
             if not result["OK"]:
                 return result
             lifetime_secs = result["Value"]
             ce.setProxy(proxy, lifetime_secs)
 
+            # Get valid token if needed
+            if "Token" in ce.ceParameters.get("Tag", []):
+                result = self.__getPilotToken()
+                if not result["OK"]:
+                    return result
+                ce.setToken(result["Value"], 3500)
+
             # now really submitting
             res = self._submitPilotsToQueue(pilotsToSubmit, ce, queueName)
             if not res["OK"]:
                 self.log.info("Failed pilot submission", f"Queue: {queueName}")
             else:
                 pilotList, stampDict = res["Value"]
 
@@ -445,14 +459,31 @@
                 self._addPilotTQReference(queueName, additionalInfo, pilotList, stampDict)
 
         # Summary after the cycle over queues
         self.log.info("Total number of pilots submitted in this cycle", f"{self.totalSubmittedPilots}")
 
         return S_OK()
 
+    def __getPilotToken(self):
+        """Get the token corresponding to the pilot user identity
+
+        :return: S_OK/S_ERROR, Token object as Value
+        """
+
+        result = Registry.getUsernameForDN(self.pilotDN)
+        if not result["OK"]:
+            return result
+        username = result["Value"]
+        result = gTokenManager.getToken(
+            username=username,
+            userGroup=self.pilotGroup,
+            requiredTimeLeft=3600,
+        )
+        return result
+
     def _ifAndWhereToSubmit(self):
         """Return a tuple that says if and where to submit pilots:
 
         (submit, anySite, jobSites, testSites)
         e.g.
         (True, False, {'Site1', 'Site2'}, {'Test1', 'Test2'})
 
@@ -1195,14 +1226,21 @@
         # This proxy is used for checking the pilot status and renewals
         # We really need at least a few hours otherwise the renewed
         # proxy may expire before we check again...
         result = ce.isProxyValid(3 * 3600)
         if not result["OK"]:
             ce.setProxy(proxy, 23300)
 
+        # Get valid token if needed
+        if "Token" in ce.ceParameters.get("Tag", []):
+            result = self.__getPilotToken()
+            if not result["OK"]:
+                return result
+            ce.setToken(result["Value"], 3500)
+
         result = ce.getJobStatus(stampedPilotRefs)
         if not result["OK"]:
             self.log.error("Failed to get pilots status from CE", f"{ceName}: {result['Message']}")
             return
         pilotCEDict = result["Value"]
 
         abortedPilots, getPilotOutput = self._updatePilotStatus(pilotRefs, pilotDict, pilotCEDict)
@@ -1297,19 +1335,19 @@
         for pRef in pilotDict:
             self.log.verbose("Preparing accounting record", f"for pilot {pRef}")
             pA = PilotAccounting()
             pA.setEndTime(pilotDict[pRef]["LastUpdateTime"])
             pA.setStartTime(pilotDict[pRef]["SubmissionTime"])
             retVal = Registry.getUsernameForDN(pilotDict[pRef]["OwnerDN"])
             if not retVal["OK"]:
-                userName = "unknown"
+                username = "unknown"
                 self.log.error("Can't determine username for dn", pilotDict[pRef]["OwnerDN"])
             else:
-                userName = retVal["Value"]
-            pA.setValueByKey("User", userName)
+                username = retVal["Value"]
+            pA.setValueByKey("User", username)
             pA.setValueByKey("UserGroup", pilotDict[pRef]["OwnerGroup"])
             result = getCESiteMapping(pilotDict[pRef]["DestinationSite"])
             if result["OK"] and result["Value"]:
                 pA.setValueByKey("Site", result["Value"][pilotDict[pRef]["DestinationSite"]].strip())
             else:
                 pA.setValueByKey("Site", "Unknown")
             pA.setValueByKey("GridCE", pilotDict[pRef]["DestinationSite"])
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/StalledJobAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/StalledJobAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/StatesAccountingAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/StatesAccountingAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/TaskQueuesAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/TaskQueuesAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobCleaningAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_JobCleaningAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PilotStatusAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PilotStatusAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PushJobAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_PushJobAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_SiteDirector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_SiteDirector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_StalledJobAgent.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Agent/test/Test_Agent_StalledJobAgent.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/CPUNormalization.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/CPUNormalization.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/DownloadInputData.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/InputDataByProtocol.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/InputDataByProtocol.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/InputDataResolution.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/InputDataResolution.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobManagerClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobManagerClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobMinorStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobMinorStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobMonitoringClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobMonitoringClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobReport.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobReport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/CachedJobState.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/CachedJobState.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobManifest.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobManifest.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobState.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobState/JobState.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobStateUpdateClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobStateUpdateClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/JobStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/JobStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/Limiter.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/Limiter.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/Matcher.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/Matcher.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/MatcherClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/MatcherClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/PilotManagerClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/PilotManagerClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/PilotStatus.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/PilotStatus.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/PoolXMLSlice.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/PoolXMLSlice.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/SandboxStoreClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/SandboxStoreClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/ServerUtils.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/ServerUtils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/WMSAdministratorClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/WMSAdministratorClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/WMSClient.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/WMSClient.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_DownloadInputData.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_DownloadInputData.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_WorkloadManagementSystem.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/Test_Client_WorkloadManagementSystem.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Client/test/Test_JobReport.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Client/test/Test_JobReport.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/ConfigTemplate.cfg` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/ConfigTemplate.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,16 @@
 
     # List of sites that will be treated by this SiteDirector ("any" can refer to any Site defined in the CS)
     Site = any
     # List of CE types that will be treated by this SiteDirector ("any" can refer to any CE defined in the CS)
     CETypes = any
     # List of CEs that will be treated by this SiteDirector ("any" can refer to any type of CE defined in the CS)
     CEs = any
+    # List of Tags that are required to be present in the CE/Queue definition
+    Tags =
 
     # The maximum length of a queue (in seconds). Default: 3 days
     MaxQueueLength = 259200
     # Log level of the pilots
     PilotLogLevel = INFO
     # Max number of pilots to submit per cycle
     MaxPilotsToSubmit = 100
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/ElasticJobParametersDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/ElasticJobParametersDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/JobLoggingDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/PilotAgentsDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/SandboxMetadataDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/SandboxMetadataDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.sql` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/TaskQueueDB.sql`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/DB/tests/Test_JobDB.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/DB/tests/Test_JobDB.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/Base/OptimizerExecutor.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/Base/OptimizerExecutor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/InputData.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/InputData.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/JobPath.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/JobPath.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/JobSanity.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/JobSanity.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/JobScheduling.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/JobScheduling.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Executor/test/Test_Executor.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Executor/test/Test_Executor.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapper.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapper.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapperTemplate.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/JobWrapperTemplate.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/Watchdog.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/Watchdog.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_JobWrapper.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_JobWrapper.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_Watchdog.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/Test_Watchdog.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/jobDescription.xml` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/JobWrapper/test/jobDescription.xml`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobMonitoringHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobMonitoringHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobPolicy.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobPolicy.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/JobStateUpdateHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/JobStateUpdateHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/MatcherHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/MatcherHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/OptimizationMindHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/OptimizationMindHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/PilotManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/PilotManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/SandboxStoreHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/SandboxStoreHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobManagerHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/TornadoJobManagerHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/WMSAdministratorHandler.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/WMSAdministratorHandler.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Service/WMSUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Service/WMSUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/JobParameters.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/JobParameters.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/JobStatusUtility.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/JobStatusUtility.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/ParametricJob.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/ParametricJob.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/PilotCStoJSONSynchronizer.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/PilotCStoJSONSynchronizer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/PilotWrapper.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/PilotWrapper.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/QueueUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/QueueUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/RemoteRunner.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/RemoteRunner.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/Utils.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/Utils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_JobStatusUtility.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_JobStatusUtility.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_ParametricJob.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_ParametricJob.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotCStoJSONSynchronizer.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotCStoJSONSynchronizer.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotWrapper.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_PilotWrapper.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_QueueUtilities.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/Utilities/test/Test_QueueUtilities.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/ConfigHelper.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/ConfigHelper.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/SharesCorrector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/SharesCorrector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseCorrector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseCorrector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseHistoryCorrector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/BaseHistoryCorrector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/MonitoringHistoryCorrector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/MonitoringHistoryCorrector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/private/correctors/WMSHistoryCorrector.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/private/correctors/WMSHistoryCorrector.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_kill_pilot.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_kill_pilot.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_show_task_queues.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_show_task_queues.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_sync_pilot.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_admin_sync_pilot.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_jobexec.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_jobexec.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_cpu_normalization.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_cpu_normalization.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_queue_cpu_time.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_queue_cpu_time.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn_parameters.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_get_wn_parameters.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_match.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_match.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_pilot_job_info.py` & `DIRAC-8.1.0a9/src/DIRAC/WorkloadManagementSystem/scripts/dirac_wms_pilot_job_info.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/__init__.py` & `DIRAC-8.1.0a9/src/DIRAC/__init__.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Test_init.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Test_init.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/IntegrationTest.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/IntegrationTest.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/ProcessesCreator_withChildren.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/ProcessesCreator_withChildren.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/WMS.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/WMS.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/assertingUtils.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/assertingUtils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/mpTest-flexible.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/mpTest-flexible.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/mpTest.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/mpTest.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/plots.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/plots.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/testJobDefinitions.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/testJobDefinitions.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Utilities/utils.py` & `DIRAC-8.1.0a9/src/DIRAC/tests/Utilities/utils.py`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC/tests/Workflow/Regression/helloWorld.xml` & `DIRAC-8.1.0a9/src/DIRAC/tests/Workflow/Regression/helloWorld.xml`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC.egg-info/PKG-INFO` & `DIRAC-8.1.0a9/src/DIRAC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DIRAC
-Version: 8.1.0a8
+Version: 8.1.0a9
 Summary: DIRAC is an interware, meaning a software framework for distributed computing.
 Home-page: https://github.com/DIRACGrid/DIRAC/
 License: GPL-3.0-only
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC.egg-info/SOURCES.txt` & `DIRAC-8.1.0a9/src/DIRAC.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -372,14 +372,15 @@
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveFile.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/RemoveReplica.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/ReplicateAndRegister.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/StagingCallback.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/__init__.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ArchiveFiles.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_CheckMigration.py
+src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_ReplicateAndRegister.py
 src/DIRAC/DataManagementSystem/Agent/RequestOperations/test/Test_RequestOperations.py
 src/DIRAC/DataManagementSystem/Client/ConsistencyInspector.py
 src/DIRAC/DataManagementSystem/Client/DataIntegrityClient.py
 src/DIRAC/DataManagementSystem/Client/DataManager.py
 src/DIRAC/DataManagementSystem/Client/DirectoryListing.py
 src/DIRAC/DataManagementSystem/Client/FTS3Client.py
 src/DIRAC/DataManagementSystem/Client/FTS3File.py
@@ -538,15 +539,14 @@
 src/DIRAC/FrameworkSystem/Service/BundleDeliveryHandler.py
 src/DIRAC/FrameworkSystem/Service/ComponentMonitoringHandler.py
 src/DIRAC/FrameworkSystem/Service/NotificationHandler.py
 src/DIRAC/FrameworkSystem/Service/ProxyManagerHandler.py
 src/DIRAC/FrameworkSystem/Service/SecurityLoggingHandler.py
 src/DIRAC/FrameworkSystem/Service/SystemAdministratorHandler.py
 src/DIRAC/FrameworkSystem/Service/TokenManagerHandler.py
-src/DIRAC/FrameworkSystem/Service/TornadoBundleDeliveryHandler.py
 src/DIRAC/FrameworkSystem/Service/TornadoComponentMonitoringHandler.py
 src/DIRAC/FrameworkSystem/Service/TornadoNotificationHandler.py
 src/DIRAC/FrameworkSystem/Service/TornadoProxyManagerHandler.py
 src/DIRAC/FrameworkSystem/Service/TornadoUserProfileManagerHandler.py
 src/DIRAC/FrameworkSystem/Service/UserProfileManagerHandler.py
 src/DIRAC/FrameworkSystem/Service/__init__.py
 src/DIRAC/FrameworkSystem/Utilities/MonitoringUtilities.py
@@ -962,15 +962,14 @@
 src/DIRAC/Resources/Computing/test/Test_HTCondorCEComputingElement.py
 src/DIRAC/Resources/Computing/test/Test_InProcessComputingElement.py
 src/DIRAC/Resources/Computing/test/Test_PoolComputingElement.py
 src/DIRAC/Resources/Computing/test/Test_SSHComputingElement.py
 src/DIRAC/Resources/Computing/test/__init__.py
 src/DIRAC/Resources/IdProvider/CheckInIdProvider.py
 src/DIRAC/Resources/IdProvider/IAMIdProvider.py
-src/DIRAC/Resources/IdProvider/IdProvider.py
 src/DIRAC/Resources/IdProvider/IdProviderFactory.py
 src/DIRAC/Resources/IdProvider/OAuth2IdProvider.py
 src/DIRAC/Resources/IdProvider/Utilities.py
 src/DIRAC/Resources/IdProvider/__init__.py
 src/DIRAC/Resources/LogBackends/AbstractBackend.py
 src/DIRAC/Resources/LogBackends/ElasticSearchBackend.py
 src/DIRAC/Resources/LogBackends/FileBackend.py
```

### Comparing `DIRAC-8.1.0a8/src/DIRAC.egg-info/entry_points.txt` & `DIRAC-8.1.0a9/src/DIRAC.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `DIRAC-8.1.0a8/src/DIRAC.egg-info/requires.txt` & `DIRAC-8.1.0a9/src/DIRAC.egg-info/requires.txt`

 * *Files identical despite different names*

