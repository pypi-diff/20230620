# Comparing `tmp/grav-toolbox-0.1.9.tar.gz` & `tmp/grav-toolbox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grav-toolbox-0.1.9.tar", last modified: Fri Apr 21 17:58:22 2023, max compression
+gzip compressed data, was "grav-toolbox-0.2.0.tar", last modified: Tue Jun 20 14:25:09 2023, max compression
```

## Comparing `grav-toolbox-0.1.9.tar` & `grav-toolbox-0.2.0.tar`

### file list

```diff
@@ -1,76 +1,86 @@
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.253033 grav-toolbox-0.1.9/
--rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/LICENSE
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-21 17:58:22.253033 grav-toolbox-0.1.9/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.1.9/README.md
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.225033 grav-toolbox-0.1.9/bev_legacy/
--rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/__init__.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/adjust.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/adjust_reilly1970.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/command_line.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/const.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/drift_mlr.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/init.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/output.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/plots.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/schwaus.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.1.9/bev_legacy/settings.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/bev_legacy/utils.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.229033 grav-toolbox-0.1.9/grav_toolbox.egg-info/
--rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/PKG-INFO
--rw-rw-r--   0 heller    (1000) heller    (1000)     2021 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/SOURCES.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/dependency_links.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/entry_points.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/requires.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-04-21 17:58:22.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/top_level.txt
--rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.1.9/grav_toolbox.egg-info/zip-safe
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.229033 grav-toolbox-0.1.9/gravtools/
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.229033 grav-toolbox-0.1.9/gravtools/CG5_utils/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/CG5_utils/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.1.9/gravtools/CG5_utils/cg5_survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-04-21 17:58:03.000000 grav-toolbox-0.1.9/gravtools/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/const.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.241033 grav-toolbox-0.1.9/gravtools/gui/
--rw-rw-r--   0 heller    (1000) heller    (1000)    61145 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/gui/MainWindow.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/gui/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_about.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_autoselection_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9024 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_corrections.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_estimation_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_export_results.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_gis_export_settings.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-04-21 17:28:55.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_load_stations.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-04-21 17:28:55.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_new_campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_options.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1805 2023-04-21 17:28:56.000000 grav-toolbox-0.1.9/gravtools/gui/dialog_setup_data.py
--rw-rw-r--   0 heller    (1000) heller    (1000)   193329 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/gui/gui_main.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_observation_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_correlation_matrix_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_drift_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_obs_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_stat_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_results_vg_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_setup_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_station_table.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.1.9/gravtools/gui/gui_model_survey_table.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.245033 grav-toolbox-0.1.9/gravtools/models/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/models/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    48441 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/models/campaign.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/models/exceptions.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    37918 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/models/lsm.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    39571 2023-04-13 12:34:11.000000 grav-toolbox-0.1.9/gravtools/models/lsm_diff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    35903 2023-04-13 12:34:49.000000 grav-toolbox-0.1.9/gravtools/models/lsm_nondiff.py
--rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/models/misc.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    18647 2023-04-13 12:35:28.000000 grav-toolbox-0.1.9/gravtools/models/mlr_bev_legacy.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/models/station.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    86806 2023-04-04 07:26:18.000000 grav-toolbox-0.1.9/gravtools/models/survey.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    32345 2023-04-13 12:35:06.000000 grav-toolbox-0.1.9/gravtools/models/vg_lsm.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.249033 grav-toolbox-0.1.9/gravtools/scripts/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/scripts/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/scripts/run_gui.py
--rwxrwxr-x   0 heller    (1000) heller    (1000)     9521 2023-04-21 17:57:27.000000 grav-toolbox-0.1.9/gravtools/settings.py
-drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-04-21 17:58:22.249033 grav-toolbox-0.1.9/gravtools/tides/
--rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/tides/__init__.py
--rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/gravtools/tides/longman1959.py
--rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.1.9/pyproject.toml
--rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-04-21 17:58:22.253033 grav-toolbox-0.1.9/setup.cfg
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35148 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/LICENSE
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6900 2023-03-23 13:03:24.000000 grav-toolbox-0.2.0/README.md
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.691353 grav-toolbox-0.2.0/bev_legacy/
+-rw-rw-r--   0 heller    (1000) heller    (1000)        0 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/__init__.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    20574 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/adjust.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7276 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/adjust_reilly1970.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2736 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/command_line.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      139 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/const.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     3935 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/drift_mlr.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    11170 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/init.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     7718 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/output.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     2408 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/plots.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     9365 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/schwaus.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     4501 2022-11-14 22:19:26.000000 grav-toolbox-0.2.0/bev_legacy/settings.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)     1933 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/bev_legacy/utils.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.695353 grav-toolbox-0.2.0/grav_toolbox.egg-info/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7414 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/PKG-INFO
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2418 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/SOURCES.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/dependency_links.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       57 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/entry_points.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)      320 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/requires.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)       21 2023-06-20 14:25:09.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/top_level.txt
+-rw-rw-r--   0 heller    (1000) heller    (1000)        1 2022-11-14 12:57:52.000000 grav-toolbox-0.2.0/grav_toolbox.egg-info/zip-safe
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.695353 grav-toolbox-0.2.0/gravtools/
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.695353 grav-toolbox-0.2.0/gravtools/CG5_utils/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1122 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/CG5_utils/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32616 2023-03-22 14:22:41.000000 grav-toolbox-0.2.0/gravtools/CG5_utils/cg5_survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1303 2023-06-20 14:24:54.000000 grav-toolbox-0.2.0/gravtools/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      757 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/const.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.703353 grav-toolbox-0.2.0/gravtools/gui/
+-rw-rw-r--   0 heller    (1000) heller    (1000)    65835 2023-06-20 14:23:44.000000 grav-toolbox-0.2.0/gravtools/gui/MainWindow.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1324 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/gui/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42685 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_about.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12317 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_autoselection_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18526 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    11546 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    42384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_estimation_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18945 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_export_results.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10236 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_gis_export_settings.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2946 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_load_stations.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    12699 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     4384 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_new_campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3979 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_options.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9036 2023-06-15 09:16:03.000000 grav-toolbox-0.2.0/gravtools/gui/dialog_setup_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15540 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/gui/dlg_correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1784 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/gui/dlg_corrections.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2371 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/gui/dlg_load_tsf_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)   199744 2023-06-20 14:23:44.000000 grav-toolbox-0.2.0/gravtools/gui/gui_main.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1709 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    15119 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_observation_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6324 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_correlation_matrix_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     6311 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_drift_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    14448 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_obs_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     7427 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_stat_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     5454 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_results_vg_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9169 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_setup_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     9716 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_station_table.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    10357 2023-04-05 11:32:57.000000 grav-toolbox-0.2.0/gravtools/gui/gui_model_survey_table.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.707353 grav-toolbox-0.2.0/gravtools/models/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1166 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/models/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    49915 2023-06-13 16:10:17.000000 grav-toolbox-0.2.0/gravtools/models/campaign.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1695 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/models/exceptions.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    38608 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/lsm.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    38803 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/lsm_diff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    35256 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/lsm_nondiff.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     2328 2023-04-04 07:26:18.000000 grav-toolbox-0.2.0/gravtools/models/misc.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18698 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/mlr_bev_legacy.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    22918 2023-04-21 17:57:27.000000 grav-toolbox-0.2.0/gravtools/models/station.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    99692 2023-06-13 16:10:17.000000 grav-toolbox-0.2.0/gravtools/models/survey.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    32396 2023-05-14 14:10:01.000000 grav-toolbox-0.2.0/gravtools/models/vg_lsm.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/gravtools/scripts/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1064 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/scripts/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1893 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/scripts/create_correction_time_seriens_from_tsf.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1481 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/scripts/load_tfs_file.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)      884 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/scripts/run_gui.py
+-rwxrwxr-x   0 heller    (1000) heller    (1000)    12110 2023-06-20 14:23:44.000000 grav-toolbox-0.2.0/gravtools/settings.py
+drwxrwxr-x   0 heller    (1000) heller    (1000)        0 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/gravtools/tides/
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1090 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/tides/__init__.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16244 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/tides/correction_time_series.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    16006 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/gravtools/tides/longman1959.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)     3413 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/tides/tide_data.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)    18016 2023-06-07 17:28:21.000000 grav-toolbox-0.2.0/gravtools/tides/tide_data_tfs.py
+-rw-rw-r--   0 heller    (1000) heller    (1000)       89 2022-07-07 12:34:18.000000 grav-toolbox-0.2.0/pyproject.toml
+-rw-rw-r--   0 heller    (1000) heller    (1000)     1105 2023-06-20 14:25:09.711353 grav-toolbox-0.2.0/setup.cfg
```

### Comparing `grav-toolbox-0.1.9/LICENSE` & `grav-toolbox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/PKG-INFO` & `grav-toolbox-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.1.9
+Version: 0.2.0
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `grav-toolbox-0.1.9/README.md` & `grav-toolbox-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/adjust.py` & `grav-toolbox-0.2.0/bev_legacy/adjust.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/adjust_reilly1970.py` & `grav-toolbox-0.2.0/bev_legacy/adjust_reilly1970.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/command_line.py` & `grav-toolbox-0.2.0/bev_legacy/command_line.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/drift_mlr.py` & `grav-toolbox-0.2.0/bev_legacy/drift_mlr.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/init.py` & `grav-toolbox-0.2.0/bev_legacy/init.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/output.py` & `grav-toolbox-0.2.0/bev_legacy/output.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/plots.py` & `grav-toolbox-0.2.0/bev_legacy/plots.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/schwaus.py` & `grav-toolbox-0.2.0/bev_legacy/schwaus.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/settings.py` & `grav-toolbox-0.2.0/bev_legacy/settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/bev_legacy/utils.py` & `grav-toolbox-0.2.0/bev_legacy/utils.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/grav_toolbox.egg-info/PKG-INFO` & `grav-toolbox-0.2.0/grav_toolbox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grav-toolbox
-Version: 0.1.9
+Version: 0.2.0
 Summary: Gravity survey utility tools
 Home-page: https://github.com/ahellers/GravTools
 Author: Andreas Hellerschmied
 Author-email: andreas.hellerschmied@bev.gv.at
 License: GNU GPLv3
 Keywords: gravity,gravimeter,least squares adjustment,geodesy,geophysics
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
```

### Comparing `grav-toolbox-0.1.9/grav_toolbox.egg-info/SOURCES.txt` & `grav-toolbox-0.2.0/grav_toolbox.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -26,22 +26,27 @@
 gravtools/settings.py
 gravtools/CG5_utils/__init__.py
 gravtools/CG5_utils/cg5_survey.py
 gravtools/gui/MainWindow.py
 gravtools/gui/__init__.py
 gravtools/gui/dialog_about.py
 gravtools/gui/dialog_autoselection_settings.py
+gravtools/gui/dialog_correction_time_series.py
 gravtools/gui/dialog_corrections.py
 gravtools/gui/dialog_estimation_settings.py
 gravtools/gui/dialog_export_results.py
 gravtools/gui/dialog_gis_export_settings.py
 gravtools/gui/dialog_load_stations.py
+gravtools/gui/dialog_load_tsf_file.py
 gravtools/gui/dialog_new_campaign.py
 gravtools/gui/dialog_options.py
 gravtools/gui/dialog_setup_data.py
+gravtools/gui/dlg_correction_time_series.py
+gravtools/gui/dlg_corrections.py
+gravtools/gui/dlg_load_tsf_file.py
 gravtools/gui/gui_main.py
 gravtools/gui/gui_misc.py
 gravtools/gui/gui_model_observation_table.py
 gravtools/gui/gui_model_results_correlation_matrix_table.py
 gravtools/gui/gui_model_results_drift_table.py
 gravtools/gui/gui_model_results_obs_table.py
 gravtools/gui/gui_model_results_stat_table.py
@@ -57,10 +62,15 @@
 gravtools/models/lsm_nondiff.py
 gravtools/models/misc.py
 gravtools/models/mlr_bev_legacy.py
 gravtools/models/station.py
 gravtools/models/survey.py
 gravtools/models/vg_lsm.py
 gravtools/scripts/__init__.py
+gravtools/scripts/create_correction_time_seriens_from_tsf.py
+gravtools/scripts/load_tfs_file.py
 gravtools/scripts/run_gui.py
 gravtools/tides/__init__.py
-gravtools/tides/longman1959.py
+gravtools/tides/correction_time_series.py
+gravtools/tides/longman1959.py
+gravtools/tides/tide_data.py
+gravtools/tides/tide_data_tfs.py
```

### Comparing `grav-toolbox-0.1.9/gravtools/CG5_utils/__init__.py` & `grav-toolbox-0.2.0/gravtools/CG5_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/CG5_utils/cg5_survey.py` & `grav-toolbox-0.2.0/gravtools/CG5_utils/cg5_survey.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/__init__.py` & `grav-toolbox-0.2.0/gravtools/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,13 +22,13 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 :Authors:
     Andreas Hellerschmied (andreas.hellerschmied@bev.gv.at)
 """
 
-__version__ = '0.1.9'
+__version__ = '0.2.0'
 __author__ = 'Andreas Hellerschmied'
 __git_repo__ = 'https://github.com/ahellers/GravTools'
 __pypi_repo__ = 'https://pypi.org/project/grav-toolbox/'
 __email__ = 'andreas.hellerschmied@bev.gv.at'
 __copyright__ = '(c) 2022 Andreas Hellerschmied'
```

### Comparing `grav-toolbox-0.1.9/gravtools/const.py` & `grav-toolbox-0.2.0/gravtools/const.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/MainWindow.py` & `grav-toolbox-0.2.0/gravtools/gui/MainWindow.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_MainWindow(object):
     def setupUi(self, MainWindow):
         MainWindow.setObjectName("MainWindow")
         MainWindow.setEnabled(True)
-        MainWindow.resize(1337, 746)
+        MainWindow.resize(1337, 753)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout_28 = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout_28.setObjectName("verticalLayout_28")
         self.tabWidget_Main = QtWidgets.QTabWidget(self.centralwidget)
         self.tabWidget_Main.setTabPosition(QtWidgets.QTabWidget.East)
         self.tabWidget_Main.setMovable(True)
@@ -374,33 +374,71 @@
         self.verticalLayout_15.setObjectName("verticalLayout_15")
         self.tableView_results_observations = QtWidgets.QTableView(self.tab_results_obs_table)
         self.tableView_results_observations.setObjectName("tableView_results_observations")
         self.verticalLayout_15.addWidget(self.tableView_results_observations)
         self.tabWidget_results.addTab(self.tab_results_obs_table, "")
         self.tab_results_obs_plots = QtWidgets.QWidget()
         self.tab_results_obs_plots.setObjectName("tab_results_obs_plots")
-        self.verticalLayout_13 = QtWidgets.QVBoxLayout(self.tab_results_obs_plots)
-        self.verticalLayout_13.setObjectName("verticalLayout_13")
+        self.verticalLayout_38 = QtWidgets.QVBoxLayout(self.tab_results_obs_plots)
+        self.verticalLayout_38.setObjectName("verticalLayout_38")
         self.graphicsLayoutWidget_results_observations_plots = GraphicsLayoutWidget(self.tab_results_obs_plots)
         self.graphicsLayoutWidget_results_observations_plots.setObjectName("graphicsLayoutWidget_results_observations_plots")
-        self.verticalLayout_13.addWidget(self.graphicsLayoutWidget_results_observations_plots)
+        self.verticalLayout_38.addWidget(self.graphicsLayoutWidget_results_observations_plots)
+        self.horizontalLayout = QtWidgets.QHBoxLayout()
+        self.horizontalLayout.setObjectName("horizontalLayout")
         self.groupBox_plot_settings = QtWidgets.QGroupBox(self.tab_results_obs_plots)
         self.groupBox_plot_settings.setObjectName("groupBox_plot_settings")
         self.verticalLayout_25 = QtWidgets.QVBoxLayout(self.groupBox_plot_settings)
         self.verticalLayout_25.setObjectName("verticalLayout_25")
         self.formLayout_4 = QtWidgets.QFormLayout()
         self.formLayout_4.setObjectName("formLayout_4")
         self.label_results_obs_plot_selec_data_column = QtWidgets.QLabel(self.groupBox_plot_settings)
         self.label_results_obs_plot_selec_data_column.setObjectName("label_results_obs_plot_selec_data_column")
         self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_results_obs_plot_selec_data_column)
         self.comboBox_results_obs_plot_select_data_column = QtWidgets.QComboBox(self.groupBox_plot_settings)
         self.comboBox_results_obs_plot_select_data_column.setObjectName("comboBox_results_obs_plot_select_data_column")
         self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.comboBox_results_obs_plot_select_data_column)
         self.verticalLayout_25.addLayout(self.formLayout_4)
-        self.verticalLayout_13.addWidget(self.groupBox_plot_settings)
+        self.radioButton_results_obs_plot_timeseries = QtWidgets.QRadioButton(self.groupBox_plot_settings)
+        self.radioButton_results_obs_plot_timeseries.setChecked(True)
+        self.radioButton_results_obs_plot_timeseries.setObjectName("radioButton_results_obs_plot_timeseries")
+        self.verticalLayout_25.addWidget(self.radioButton_results_obs_plot_timeseries)
+        self.radioButton_results_obs_plot_histogram = QtWidgets.QRadioButton(self.groupBox_plot_settings)
+        self.radioButton_results_obs_plot_histogram.setObjectName("radioButton_results_obs_plot_histogram")
+        self.verticalLayout_25.addWidget(self.radioButton_results_obs_plot_histogram)
+        self.horizontalLayout.addWidget(self.groupBox_plot_settings)
+        self.groupBox_histogram_settings = QtWidgets.QGroupBox(self.tab_results_obs_plots)
+        self.groupBox_histogram_settings.setEnabled(False)
+        self.groupBox_histogram_settings.setObjectName("groupBox_histogram_settings")
+        self.verticalLayout_13 = QtWidgets.QVBoxLayout(self.groupBox_histogram_settings)
+        self.verticalLayout_13.setObjectName("verticalLayout_13")
+        self.formLayout_8 = QtWidgets.QFormLayout()
+        self.formLayout_8.setObjectName("formLayout_8")
+        self.label_11 = QtWidgets.QLabel(self.groupBox_histogram_settings)
+        self.label_11.setObjectName("label_11")
+        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_11)
+        self.comboBox_results_obs_plot_hist_method = QtWidgets.QComboBox(self.groupBox_histogram_settings)
+        self.comboBox_results_obs_plot_hist_method.setObjectName("comboBox_results_obs_plot_hist_method")
+        self.formLayout_8.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.comboBox_results_obs_plot_hist_method)
+        self.label_results_obs_plot_number_bins = QtWidgets.QLabel(self.groupBox_histogram_settings)
+        self.label_results_obs_plot_number_bins.setObjectName("label_results_obs_plot_number_bins")
+        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.LabelRole, self.label_results_obs_plot_number_bins)
+        self.spinBox_results_obs_plot_number_bins = QtWidgets.QSpinBox(self.groupBox_histogram_settings)
+        self.spinBox_results_obs_plot_number_bins.setMinimum(2)
+        self.spinBox_results_obs_plot_number_bins.setMaximum(1000)
+        self.spinBox_results_obs_plot_number_bins.setProperty("value", 10)
+        self.spinBox_results_obs_plot_number_bins.setObjectName("spinBox_results_obs_plot_number_bins")
+        self.formLayout_8.setWidget(1, QtWidgets.QFormLayout.FieldRole, self.spinBox_results_obs_plot_number_bins)
+        self.verticalLayout_13.addLayout(self.formLayout_8)
+        self.checkBox_results_obs_plot_show_outliers = QtWidgets.QCheckBox(self.groupBox_histogram_settings)
+        self.checkBox_results_obs_plot_show_outliers.setEnabled(False)
+        self.checkBox_results_obs_plot_show_outliers.setObjectName("checkBox_results_obs_plot_show_outliers")
+        self.verticalLayout_13.addWidget(self.checkBox_results_obs_plot_show_outliers)
+        self.horizontalLayout.addWidget(self.groupBox_histogram_settings)
+        self.verticalLayout_38.addLayout(self.horizontalLayout)
         self.tabWidget_results.addTab(self.tab_results_obs_plots, "")
         self.tab_results_drift = QtWidgets.QWidget()
         self.tab_results_drift.setObjectName("tab_results_drift")
         self.verticalLayout_18 = QtWidgets.QVBoxLayout(self.tab_results_drift)
         self.verticalLayout_18.setObjectName("verticalLayout_18")
         self.tableView_results_drift = QtWidgets.QTableView(self.tab_results_drift)
         self.tableView_results_drift.setObjectName("tableView_results_drift")
@@ -508,14 +546,16 @@
         self.menu_Observations.setTearOffEnabled(False)
         self.menu_Observations.setObjectName("menu_Observations")
         self.menuEstimation_settings = QtWidgets.QMenu(self.menubar)
         self.menuEstimation_settings.setEnabled(True)
         self.menuEstimation_settings.setObjectName("menuEstimation_settings")
         self.menuHelp = QtWidgets.QMenu(self.menubar)
         self.menuHelp.setObjectName("menuHelp")
+        self.menuCorrections = QtWidgets.QMenu(self.menubar)
+        self.menuCorrections.setObjectName("menuCorrections")
         MainWindow.setMenuBar(self.menubar)
         self.statusbar = QtWidgets.QStatusBar(MainWindow)
         self.statusbar.setInputMethodHints(QtCore.Qt.ImhNone)
         self.statusbar.setObjectName("statusbar")
         MainWindow.setStatusBar(self.statusbar)
         self.action_New_Campaign = QtWidgets.QAction(MainWindow)
         self.action_New_Campaign.setObjectName("action_New_Campaign")
@@ -578,14 +618,16 @@
         self.action_Gis_Export_settings = QtWidgets.QAction(MainWindow)
         self.action_Gis_Export_settings.setEnabled(False)
         self.action_Gis_Export_settings.setObjectName("action_Gis_Export_settings")
         self.action_from_oesgn_table = QtWidgets.QAction(MainWindow)
         self.action_from_oesgn_table.setObjectName("action_from_oesgn_table")
         self.action_from_csv_file = QtWidgets.QAction(MainWindow)
         self.action_from_csv_file.setObjectName("action_from_csv_file")
+        self.action_Correction_time_series = QtWidgets.QAction(MainWindow)
+        self.action_Correction_time_series.setObjectName("action_Correction_time_series")
         self.menuAdd_Survey.addAction(self.action_from_CG5_observation_file)
         self.menuAdd_Survey.addAction(self.action_from_BEV_observation_file)
         self.menu_Add_Stations.addAction(self.action_from_oesgn_table)
         self.menu_Add_Stations.addAction(self.action_from_csv_file)
         self.menu_File.addAction(self.action_New_Campaign)
         self.menu_File.addAction(self.action_Change_output_directory)
         self.menu_File.addAction(self.action_Change_Campaign_name)
@@ -598,32 +640,35 @@
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Export_Results)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Options)
         self.menu_File.addSeparator()
         self.menu_File.addAction(self.action_Exit)
         self.menu_Observations.addSeparator()
-        self.menu_Observations.addAction(self.action_Corrections)
         self.menu_Observations.addAction(self.action_Autoselection_settings)
         self.menu_Observations.addAction(self.actionEstimate_long_term_drift)
         self.menu_Observations.addAction(self.action_Setup_data_options)
         self.menu_Observations.addAction(self.action_Flag_observations)
         self.menuEstimation_settings.addAction(self.action_Estimation_settings)
         self.menuEstimation_settings.addAction(self.action_Gis_Export_settings)
         self.menuHelp.addAction(self.action_About)
+        self.menuCorrections.addAction(self.action_Corrections)
+        self.menuCorrections.addAction(self.action_Correction_time_series)
         self.menubar.addAction(self.menu_File.menuAction())
         self.menubar.addAction(self.menu_Observations.menuAction())
         self.menubar.addAction(self.menuEstimation_settings.menuAction())
+        self.menubar.addAction(self.menuCorrections.menuAction())
         self.menubar.addAction(self.menuHelp.menuAction())
 
         self.retranslateUi(MainWindow)
         self.tabWidget_Main.setCurrentIndex(1)
         self.tab_Widget_Stations.setCurrentIndex(0)
         self.tabWidget_observations.setCurrentIndex(0)
-        self.tabWidget_results.setCurrentIndex(3)
+        self.tabWidget_results.setCurrentIndex(0)
+        self.radioButton_results_obs_plot_histogram.toggled['bool'].connect(self.groupBox_histogram_settings.setEnabled) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
         MainWindow.setWindowTitle(_translate("MainWindow", "GravTools"))
         self.groupBox_filter_options.setToolTip(_translate("MainWindow", "Display options for stations"))
         self.groupBox_filter_options.setTitle(_translate("MainWindow", "Filter Options"))
@@ -693,14 +738,20 @@
         self.label_7.setToolTip(_translate("MainWindow", "Number of detected outliers."))
         self.label_7.setText(_translate("MainWindow", "Number of outliers:"))
         self.groupBox_results_lsm_run_log.setTitle(_translate("MainWindow", "LSM run log"))
         self.tabWidget_results.setTabText(self.tabWidget_results.indexOf(self.tab_results_info), _translate("MainWindow", "Info"))
         self.tabWidget_results.setTabText(self.tabWidget_results.indexOf(self.tab_results_obs_table), _translate("MainWindow", "Observations Table"))
         self.groupBox_plot_settings.setTitle(_translate("MainWindow", "Plot settings"))
         self.label_results_obs_plot_selec_data_column.setText(_translate("MainWindow", "Select data column:"))
+        self.radioButton_results_obs_plot_timeseries.setText(_translate("MainWindow", "Time series"))
+        self.radioButton_results_obs_plot_histogram.setText(_translate("MainWindow", "Histogram"))
+        self.groupBox_histogram_settings.setTitle(_translate("MainWindow", "Histogram settings"))
+        self.label_11.setText(_translate("MainWindow", "Method"))
+        self.label_results_obs_plot_number_bins.setText(_translate("MainWindow", "Number of bins"))
+        self.checkBox_results_obs_plot_show_outliers.setText(_translate("MainWindow", "Show outliers"))
         self.tabWidget_results.setTabText(self.tabWidget_results.indexOf(self.tab_results_obs_plots), _translate("MainWindow", "Observations Plots"))
         self.tabWidget_results.setTabText(self.tabWidget_results.indexOf(self.tab_results_drift), _translate("MainWindow", "Drift Table"))
         self.graphicsLayoutWidget_results_drift_plot.setToolTip(_translate("MainWindow", "<html><head/><body><p>This plot depicts setup observations and the the drift function (polynomial of degree n) fitted to these observations.</p></body></html>"))
         self.groupBox_results_drift_plot.setTitle(_translate("MainWindow", "Drift plot settings"))
         self.label_results_drift_plot_v_offset.setToolTip(_translate("MainWindow", "<html><head/><body><p>Add vertical offset to the drift function (polynomial) w.r.t. the setup observations. This is needed to when differential observations are used for prameter estimation. In this case the constant bias of the gravimeter reading cannot be estimated and is only determined approximately.</p></body></html>"))
         self.label_results_drift_plot_v_offset.setText(_translate("MainWindow", "Vertical offset of drift polynomial w.r.t. setup observations [µGal]"))
         self.spinBox_results_drift_plot_v_offset.setToolTip(_translate("MainWindow", "<html><head/><body><p>Add vertical offset to the drift function (polynomial) w.r.t. the setup observations. This is needed to when differential observations are used for prameter estimation. In this case the constant bias of the gravimeter reading cannot be estimated and is only determined approximately.</p></body></html>"))
@@ -722,25 +773,26 @@
         self.tabWidget_Main.setTabToolTip(self.tabWidget_Main.indexOf(self.tab_main_results), _translate("MainWindow", "Setup data: Corrected and reduces observation data accumulated for each instrument setup."))
         self.menu_File.setTitle(_translate("MainWindow", "File"))
         self.menuAdd_Survey.setTitle(_translate("MainWindow", "Add Survey"))
         self.menu_Add_Stations.setTitle(_translate("MainWindow", "Add Stations"))
         self.menu_Observations.setTitle(_translate("MainWindow", "Observations"))
         self.menuEstimation_settings.setTitle(_translate("MainWindow", "Settings"))
         self.menuHelp.setTitle(_translate("MainWindow", "Help"))
+        self.menuCorrections.setTitle(_translate("MainWindow", "Corrections"))
         self.action_New_Campaign.setText(_translate("MainWindow", "&New Campaign"))
         self.action_Save_Campaign.setText(_translate("MainWindow", "&Save Campaign"))
         self.action_Load_Campaign.setText(_translate("MainWindow", "&Load Campaign"))
         self.action_Load_Campaign.setToolTip(_translate("MainWindow", "Load campaign"))
         self.action_Add_Stations.setText(_translate("MainWindow", "Add Stations"))
         self.action_Exit.setText(_translate("MainWindow", "E&xit"))
         self.action_Exit.setToolTip(_translate("MainWindow", "Exit GravTools"))
         self.action_Edit_Observations.setText(_translate("MainWindow", "Edit Observations"))
         self.actionResiduals.setText(_translate("MainWindow", "Residuals"))
         self.actionEstimates.setText(_translate("MainWindow", "Estimates"))
-        self.action_Corrections.setText(_translate("MainWindow", "Corrections"))
+        self.action_Corrections.setText(_translate("MainWindow", "Correction settings"))
         self.actionShow_Stations.setText(_translate("MainWindow", "Show Stations"))
         self.action_from_CG5_observation_file.setText(_translate("MainWindow", "from CG5 observation file"))
         self.action_from_BEV_observation_file.setText(_translate("MainWindow", "from BEV observation file"))
         self.action_Autoselection_settings.setText(_translate("MainWindow", "Autoselection settings"))
         self.action_Estimation_settings.setText(_translate("MainWindow", "Estimation settings"))
         self.actionEstimate_long_term_drift.setText(_translate("MainWindow", "Estimate long-term drift"))
         self.action_Export_Results.setText(_translate("MainWindow", "Export Data"))
@@ -752,8 +804,10 @@
         self.action_Flag_observations.setToolTip(_translate("MainWindow", "Flag observations based ob observations file"))
         self.action_Change_Campaign_name.setText(_translate("MainWindow", "Change Campaign name"))
         self.action_About.setText(_translate("MainWindow", "About"))
         self.action_License.setText(_translate("MainWindow", "License"))
         self.action_Gis_Export_settings.setText(_translate("MainWindow", "GIS export settings"))
         self.action_from_oesgn_table.setText(_translate("MainWindow", "From OESGN file"))
         self.action_from_csv_file.setText(_translate("MainWindow", "From CSV file"))
+        self.action_Correction_time_series.setText(_translate("MainWindow", "Correction time series"))
+        self.action_Correction_time_series.setToolTip(_translate("MainWindow", "Manage correction time series data"))
 from pyqtgraph import GraphicsLayoutWidget
```

### Comparing `grav-toolbox-0.1.9/gravtools/gui/__init__.py` & `grav-toolbox-0.2.0/gravtools/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_about.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_about.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_autoselection_settings.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_autoselection_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_corrections.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_corrections.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 from PyQt5 import QtCore, QtGui, QtWidgets
 
 
 class Ui_Dialog_corrections(object):
     def setupUi(self, Dialog_corrections):
         Dialog_corrections.setObjectName("Dialog_corrections")
-        Dialog_corrections.resize(287, 340)
+        Dialog_corrections.resize(362, 419)
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(Dialog_corrections)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout()
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.groupBox_corrections_tides = QtWidgets.QGroupBox(Dialog_corrections)
         self.groupBox_corrections_tides.setObjectName("groupBox_corrections_tides")
         self.verticalLayout_3 = QtWidgets.QVBoxLayout(self.groupBox_corrections_tides)
@@ -36,15 +36,30 @@
         self.radioButton_corr_tides_cg5_model.setObjectName("radioButton_corr_tides_cg5_model")
         self.buttonGroup_corrections_tides.addButton(self.radioButton_corr_tides_cg5_model)
         self.verticalLayout.addWidget(self.radioButton_corr_tides_cg5_model)
         self.radioButton_corr_tides_longman1959 = QtWidgets.QRadioButton(self.groupBox_corrections_tides)
         self.radioButton_corr_tides_longman1959.setObjectName("radioButton_corr_tides_longman1959")
         self.buttonGroup_corrections_tides.addButton(self.radioButton_corr_tides_longman1959)
         self.verticalLayout.addWidget(self.radioButton_corr_tides_longman1959)
+        self.radioButton_corr_tides_time_series = QtWidgets.QRadioButton(self.groupBox_corrections_tides)
+        self.radioButton_corr_tides_time_series.setObjectName("radioButton_corr_tides_time_series")
+        self.buttonGroup_corrections_tides.addButton(self.radioButton_corr_tides_time_series)
+        self.verticalLayout.addWidget(self.radioButton_corr_tides_time_series)
         self.verticalLayout_3.addLayout(self.verticalLayout)
+        self.formLayout = QtWidgets.QFormLayout()
+        self.formLayout.setObjectName("formLayout")
+        self.label_tides_interpolation_method = QtWidgets.QLabel(self.groupBox_corrections_tides)
+        self.label_tides_interpolation_method.setEnabled(False)
+        self.label_tides_interpolation_method.setObjectName("label_tides_interpolation_method")
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.LabelRole, self.label_tides_interpolation_method)
+        self.comboBox_tides_interpolation_method = QtWidgets.QComboBox(self.groupBox_corrections_tides)
+        self.comboBox_tides_interpolation_method.setEnabled(False)
+        self.comboBox_tides_interpolation_method.setObjectName("comboBox_tides_interpolation_method")
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.FieldRole, self.comboBox_tides_interpolation_method)
+        self.verticalLayout_3.addLayout(self.formLayout)
         self.verticalLayout_5.addWidget(self.groupBox_corrections_tides)
         self.groupBox_corrections_ref_heights = QtWidgets.QGroupBox(Dialog_corrections)
         self.groupBox_corrections_ref_heights.setObjectName("groupBox_corrections_ref_heights")
         self.verticalLayout_4 = QtWidgets.QVBoxLayout(self.groupBox_corrections_ref_heights)
         self.verticalLayout_4.setObjectName("verticalLayout_4")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setObjectName("verticalLayout_2")
@@ -65,37 +80,46 @@
         self.radioButton_corr_ref_heights_control_point = QtWidgets.QRadioButton(self.groupBox_corrections_ref_heights)
         self.radioButton_corr_ref_heights_control_point.setChecked(True)
         self.radioButton_corr_ref_heights_control_point.setObjectName("radioButton_corr_ref_heights_control_point")
         self.buttonGroup_corrections_ref_heights.addButton(self.radioButton_corr_ref_heights_control_point)
         self.verticalLayout_2.addWidget(self.radioButton_corr_ref_heights_control_point)
         self.verticalLayout_4.addLayout(self.verticalLayout_2)
         self.verticalLayout_5.addWidget(self.groupBox_corrections_ref_heights)
+        spacerItem = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
+        self.verticalLayout_5.addItem(spacerItem)
         self.buttonBox = QtWidgets.QDialogButtonBox(Dialog_corrections)
         self.buttonBox.setOrientation(QtCore.Qt.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.Cancel|QtWidgets.QDialogButtonBox.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.verticalLayout_5.addWidget(self.buttonBox)
         self.verticalLayout_6.addLayout(self.verticalLayout_5)
 
         self.retranslateUi(Dialog_corrections)
         self.buttonBox.accepted.connect(Dialog_corrections.accept) # type: ignore
         self.buttonBox.rejected.connect(Dialog_corrections.reject) # type: ignore
+        self.radioButton_corr_tides_time_series.toggled['bool'].connect(self.comboBox_tides_interpolation_method.setEnabled) # type: ignore
+        self.radioButton_corr_tides_time_series.toggled['bool'].connect(self.label_tides_interpolation_method.setEnabled) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(Dialog_corrections)
 
     def retranslateUi(self, Dialog_corrections):
         _translate = QtCore.QCoreApplication.translate
         Dialog_corrections.setWindowTitle(_translate("Dialog_corrections", "Corrections"))
-        self.groupBox_corrections_tides.setToolTip(_translate("Dialog_corrections", "Different options are available to apply corrections for the tidal effects of sun and moon on the observed gravity."))
+        self.groupBox_corrections_tides.setToolTip(_translate("Dialog_corrections", "<html><head/><body><p>Options for tidal corretio of observation data.</p></body></html>"))
         self.groupBox_corrections_tides.setTitle(_translate("Dialog_corrections", "Tidal correction"))
         self.radioButton_corr_tides_no_correction.setToolTip(_translate("Dialog_corrections", "No tidal corrections applied."))
         self.radioButton_corr_tides_no_correction.setText(_translate("Dialog_corrections", "No correction"))
         self.radioButton_corr_tides_cg5_model.setToolTip(_translate("Dialog_corrections", "The tidal correction calculated by the CG-5 instrument (Longman, 1959) is applied."))
         self.radioButton_corr_tides_cg5_model.setText(_translate("Dialog_corrections", "CG-5 model (Longman, 1959)"))
         self.radioButton_corr_tides_longman1959.setToolTip(_translate("Dialog_corrections", "Tidal corrections are calculated ans applied in GravTools by evaluationg the model by Longman (1959). "))
         self.radioButton_corr_tides_longman1959.setText(_translate("Dialog_corrections", "Longman (1959)"))
+        self.radioButton_corr_tides_time_series.setToolTip(_translate("Dialog_corrections", "<html><head/><body><p>Interpolate corrections from time series data. The python module <span style=\" font-style:italic;\">scipy.interpolation.interp1</span> is used.</p></body></html>"))
+        self.radioButton_corr_tides_time_series.setText(_translate("Dialog_corrections", "Interpolate from time series"))
+        self.label_tides_interpolation_method.setToolTip(_translate("Dialog_corrections", "Method for the interpolation of correction time series."))
+        self.label_tides_interpolation_method.setText(_translate("Dialog_corrections", "Interpolation method"))
+        self.comboBox_tides_interpolation_method.setToolTip(_translate("Dialog_corrections", "Method for the interpolation of correction time series."))
         self.groupBox_corrections_ref_heights.setToolTip(_translate("Dialog_corrections", "The original gravity reading refer to the location (height) of the sensor within the instrument. By using the vertical differences \"dhb\" and \"dhf\" provided in the CG-5observation files along with the observation data and the vertical gravity gradients (standard value or provided in the station data), the observations can be reduced to different refernce heights."))
         self.groupBox_corrections_ref_heights.setTitle(_translate("Dialog_corrections", "Reference height"))
         self.radioButton_corr_ref_heights_sensor.setToolTip(_translate("Dialog_corrections", "Sensor heigt (measurement heugt => no correction applied)"))
         self.radioButton_corr_ref_heights_sensor.setText(_translate("Dialog_corrections", "Sensor"))
         self.radioButton_corr_ref_heights_instrument_top.setToolTip(_translate("Dialog_corrections", "Top of the gravimeter."))
         self.radioButton_corr_ref_heights_instrument_top.setText(_translate("Dialog_corrections", "Instrument top"))
         self.radioButton_corr_ref_heights_ground.setToolTip(_translate("Dialog_corrections", "Ground level at the station."))
```

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_estimation_settings.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_estimation_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_export_results.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_export_results.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_gis_export_settings.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_gis_export_settings.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_load_stations.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_load_stations.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_new_campaign.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_new_campaign.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/dialog_options.py` & `grav-toolbox-0.2.0/gravtools/gui/dialog_options.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_main.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 """
 
 import sys
 import os
 import warnings
 from PyQt5.QtWidgets import QApplication, QDialog, QMainWindow, QFileDialog, QMessageBox, QTreeWidgetItem, \
     QHeaderView, QInputDialog
-from PyQt5.QtCore import QDir, QAbstractTableModel, Qt, QSortFilterProxyModel, pyqtSlot, QRegExp, QModelIndex
+from PyQt5.QtCore import QDir, Qt, QSortFilterProxyModel, pyqtSlot, QRegExp
 from PyQt5 import QtGui
 import datetime as dt
 import pyqtgraph as pg
 import pyqtgraph.exporters
 import numpy as np
 import pandas as pd
 import pytz
@@ -44,15 +44,14 @@
                   ' will not be available.', UserWarning)
 else:
     _has_geopandas = True
 
 from gravtools.gui.MainWindow import Ui_MainWindow
 from gravtools.gui.dialog_new_campaign import Ui_Dialog_new_Campaign
 from gravtools.gui.dialog_load_stations import Ui_Dialog_load_stations
-from gravtools.gui.dialog_corrections import Ui_Dialog_corrections
 from gravtools.gui.dialog_autoselection_settings import Ui_Dialog_autoselection_settings
 from gravtools.gui.dialog_estimation_settings import Ui_Dialog_estimation_settings
 from gravtools.gui.dialog_setup_data import Ui_Dialog_setup_data
 from gravtools.gui.dialog_export_results import Ui_Dialog_export_results
 from gravtools.gui.dialog_options import Ui_Dialog_options
 from gravtools.gui.dialog_about import Ui_Dialog_about
 from gravtools.gui.dialog_gis_export_settings import Ui_Dialog_gis_settings
@@ -62,14 +61,16 @@
 from gravtools.gui.gui_model_results_stat_table import ResultsStationModel
 from gravtools.gui.gui_model_results_obs_table import ResultsObservationModel
 from gravtools.gui.gui_model_results_drift_table import ResultsDriftModel
 from gravtools.gui.gui_model_results_correlation_matrix_table import ResultsCorrelationMatrixModel
 from gravtools.gui.gui_model_results_vg_table import ResultsVGModel
 from gravtools.gui.gui_model_survey_table import SurveyTableModel
 from gravtools.gui.gui_misc import get_station_color_dict, checked_state_to_bool
+from gravtools.gui.dlg_correction_time_series import DialogCorrectionTimeSeries
+from gravtools.gui.dlg_corrections import DialogCorrections
 from gravtools import __version__, __author__, __git_repo__, __email__, __copyright__, __pypi_repo__
 
 from gravtools.models.survey import Survey
 from gravtools.models.campaign import Campaign
 from gravtools import settings
 
 DEFAULT_OUTPUT_DIR = os.path.abspath(os.getcwd())  # Current working directory
@@ -127,14 +128,15 @@
         self.pushButton_obs_comp_setup_data.pressed.connect(self.on_pushbutton_obs_comp_setup_data)
         self.pushButton_obs_run_estimation.pressed.connect(self.on_pushbutton_obs_run_estimation)
         self.pushButton_results_delete_lsm_run.pressed.connect(self.on_pushbutton_results_delete_lsm_run)
         self.pushButton_results_export_shapefile.pressed.connect(self.on_pushButton_results_export_shapefile)
         self.action_from_CG5_observation_file.triggered.connect(self.on_menu_file_load_survey_from_cg5_observation_file)
         self.action_from_oesgn_table.triggered.connect(self.on_menu_file_load_stations_from_oesgn_table)
         self.action_from_csv_file.triggered.connect(self.on_menu_file_load_stations_from_csv_file)
+        self.action_Correction_time_series.triggered.connect(self.action_correction_time_series_triggered)
         self.lineEdit_filter_stat_name.textChanged.connect(self.on_lineEdit_filter_stat_name_textChanged)
         self.checkBox_filter_observed_stat_only.stateChanged.connect(self.on_checkBox_filter_observed_stat_only_toggled)
         self.checkBox_obs_plot_setup_data.stateChanged.connect(self.on_checkBox_obs_plot_setup_data_state_changed)
         self.treeWidget_observations.itemSelectionChanged.connect(self.on_obs_tree_widget_item_selected)
         self.treeWidget_observations.itemChanged.connect(self.on_tree_widget_item_changed)
         self.checkBox_obs_plot_reduced_observations.clicked.connect(self.on_obs_tree_widget_item_selected)
         self.comboBox_results_lsm_run_selection.currentIndexChanged.connect(
@@ -151,34 +153,42 @@
             self.on_checkBox_stations_map_show_stat_name_labels_state_changed)
         self.radioButton_results_vg_plot_details.toggled.connect(self.on_results_vg_plot_type_radiobuttons_changed)
         self.radioButton_results_vg_plot_full_polynomial.toggled.connect(self.on_results_vg_plot_type_radiobuttons_changed)
         self.checkBox_stations_map_show_stat_name_labels.stateChanged.connect(
             self.on_checkBox_stations_map_show_stat_name_labels_state_changed)
         self.checkBox_results_vg_plot_show_residuals.stateChanged.connect(
             self.checkBox_results_vg_plot_show_residuals_state_changed)
+        self.radioButton_results_obs_plot_timeseries.toggled.connect(self.update_results_obs_plots)
+        self.radioButton_results_obs_plot_histogram.toggled.connect(self.update_results_obs_plots)
+        self.comboBox_results_obs_plot_hist_method.currentIndexChanged.connect(self.update_results_obs_plots)
+        self.comboBox_results_obs_plot_hist_method.currentIndexChanged.connect(
+            self.on_histogram_bin_method_currentIndexChanged)
+        self.spinBox_results_obs_plot_number_bins.valueChanged.connect(self.update_results_obs_plots)
         # self.action_Load_Campaign.triggered.connect(self.on_action_Load_Campaign_triggered)  # Not needed!?!
         # self.action_Change_output_directory.triggered.connect(self.on_action_Change_output_directory_triggered)  # Not needed!?!
 
         # Set up GUI items and widgets:
         self.set_up_survey_tree_widget()
         self.set_up_obseration_plots_widget()
         self.set_up_obseration_results_plots_widget()
+        self.set_up_obseration_results_plots_hist_method_comboBox()
         self.set_up_drift_plot_widget()
         self.set_up_stations_map()
         self.set_up_vg_plot_widget()
         # self.observations_splitter.setSizes([1000, 10])
 
         # Initialize dialogs if necessary at the start of the application:
-        self.dlg_corrections = DialogCorrections()
-        self.dlg_autoselect_settings = DialogAutoselectSettings()
-        self.dlg_estimation_settings = DialogEstimationSettings()
-        self.dlg_gis_export_settings = DialogGisExportSettings()
-        self.dlg_options = DialogOptions()
-        self.dlg_setup_data = DialogSetupData()
-        self.dlg_about = DialogAbout()
+        self.dlg_corrections = DialogCorrections(self)
+        self.dlg_autoselect_settings = DialogAutoselectSettings(self)
+        self.dlg_estimation_settings = DialogEstimationSettings(self)
+        self.dlg_gis_export_settings = DialogGisExportSettings(self)
+        self.dlg_options = DialogOptions(self)
+        self.dlg_setup_data = DialogSetupData(self)
+        self.dlg_about = DialogAbout(self)
+        self.dlg_correction_time_series = DialogCorrectionTimeSeries(self)
         # self.dlg_about.label_author.setText(__author__)
         self.dlg_about.label_version.setText(__version__)
         self.dlg_about.label_git_repo.setText(__git_repo__)
         self.dlg_about.label_pypi_repo.setText(__pypi_repo__)
         self.dlg_about.label_email.setText(__email__)
         self.dlg_about.label_copyright.setText(__copyright__)
 
@@ -217,14 +227,18 @@
 
         # Set fonts:
         self.plainTextEdit_results_log.setFont(self.system_default_fixed_width_font)  # Monospace font
 
         # Inits misc:
         self.station_colors_dict_results = {}  # set in self.update_results_tab()
 
+    def action_correction_time_series_triggered(self):
+        """Launch dialog for managing correction time series data."""
+        _ = self.dlg_correction_time_series.exec()
+
     @pyqtSlot()
     def on_pushButton_results_export_shapefile(self):
         """Invoked whenever pressing the button."""
         # Get the currently selected lsm run object:
         idx, time_str = self.get_selected_lsm_run()
         if idx == -1:  # invalid index
             self.statusBar().showMessage(f'No data selected for export to shapefiles...')
@@ -477,14 +491,19 @@
                 # - Results tab:
                 self.set_up_results_stations_view_model()
                 self.set_up_results_correlation_matrix_view_model()
                 self.set_up_results_observations_view_model()
                 self.set_up_results_drift_view_model()
                 self.set_up_results_vg_view_model()
                 self.update_results_tab(select_latest_item=True)
+                # - Corrections time series dialog:
+                self.dlg_correction_time_series.check_correction_time_series_object(parent=self)
+                self.dlg_correction_time_series.reset_update_gui()
+
+
 
                 self.statusBar().showMessage(
                     f"Previously saved campaign loaded rom pickle file (name: {self.campaign.campaign_name}, "
                     f"output directory: {self.campaign.output_directory})")
                 self.setWindowTitle('GravTools - Campaign: ' + self.campaign.campaign_name)
         else:
             self.statusBar().showMessage(f"No campaign data loaded.")
@@ -684,15 +703,14 @@
             #     selected_survey_names = [selected_survey_name]
 
             # Select lsm run:
             lsm_run = self.campaign.lsm_runs[lsm_run_idx]
 
             # Invoke plotting method according to the LSM method:
             if lsm_run.lsm_method == 'VG_LSM_nondiff':
-                # TODO: Get parameters from GUI!!
                 # Get plot settings from the GUI:
                 plot_residuals = self.checkBox_results_vg_plot_show_residuals.checkState() == Qt.Checked
                 if self.radioButton_results_vg_plot_details.isChecked() and not self.radioButton_results_vg_plot_full_polynomial.isChecked():
                     plot_type = 'detail'
                 elif not self.radioButton_results_vg_plot_details.isChecked() and self.radioButton_results_vg_plot_full_polynomial.isChecked():
                     plot_type = 'full'
                 else:
@@ -1051,18 +1069,25 @@
             # Prep data:
             drift_pol_df_short = drift_pol_df.loc[drift_pol_df['survey_name'] == survey_name]
             setup_df = setup_df_orig.copy(deep=True)  # Make hard copy to protect original data!
             # stat_obs_df_short = stat_obs_df.loc[:, ['station_name', 'g_est_mugal', 'sd_g_est_mugal']]
             # setup_df = pd.merge(setup_df, stat_obs_df_short, on='station_name')
             # setup_df['g_plot_mugal'] = setup_df['g_mugal'] - setup_df['g_est_mugal']
             setup_df.sort_values(by='delta_t_campaign_h', inplace=True)
-            setup_obs_df_short = lsm_run.setup_obs_df.loc[lsm_run.setup_obs_df['survey_name'] == survey_name, ['setup_id', 'v_obs_est_mugal']].copy(deep=True)
             # Merge df => Colum with post-fit residuals ("v_obs_est_mugal") added to "setup_df":
-            setup_df = pd.merge(setup_df, setup_obs_df_short, how='left', on='setup_id')
-
+            if setup_data['setup_calc_method'] != 'individual_obs':
+                setup_obs_df_short = lsm_run.setup_obs_df.loc[
+                    lsm_run.setup_obs_df['survey_name'] == survey_name, ['setup_id', 'v_obs_est_mugal']].copy(deep=True)
+                setup_df = pd.merge(setup_df, setup_obs_df_short, how='left', on='setup_id')  # WEG!
+            else:
+                setup_obs_df_short = lsm_run.setup_obs_df.loc[
+                    lsm_run.setup_obs_df['survey_name'] == survey_name, ['ref_epoch_dt', 'v_obs_est_mugal']].copy(
+                    deep=True)
+                setup_df = pd.merge(setup_df, setup_obs_df_short, how='left', left_on='epoch_dt',
+                                    right_on='ref_epoch_dt')
             # Evaluate drift polynomial:
             coeff_list = drift_pol_df_short['coefficient'].to_list()
             coeff_list.reverse()
             if lsm_run.drift_ref_epoch_type == 'survey':
                 delta_t_min_h = setup_df['delta_t_h'].min()  # = 0
                 delta_t_max_h = setup_df['delta_t_h'].max()
             elif lsm_run.drift_ref_epoch_type == 'campaign':
@@ -1340,49 +1365,130 @@
 
         # Adjust plot window:
         self.drift_plot.showGrid(x=True, y=True)
         self.drift_plot.setLabel(axis='left', text=f'g [µGal]')
         self.drift_plot.setTitle(f'Drift function w.r.t. setup observations')
         self.drift_plot.autoRange()
 
+    def set_up_obseration_results_plots_hist_method_comboBox(self):
+        """Set up the histogram method combo box."""
+        self.comboBox_results_obs_plot_hist_method.addItems(list(settings.NUMPY_HISTOGRAM_BIN_EDGES_OPTIONS.keys()))
+        # self.histogram_bin_method_selection(0)  # default: i. item in dict
+
     def set_up_obseration_results_plots_widget(self):
         """Set up `self.graphicsLayoutWidget_results_observations_plots`."""
         self.glw_obs_results = self.graphicsLayoutWidget_results_observations_plots
         self.glw_obs_results.setBackground('w')  # white background color
 
         # Create sub-plots:
+        # - Initialize time series or histogram:
+        if self.radioButton_results_obs_plot_timeseries.isChecked():
+            self.init_observation_results_plots_timerseries()
+        elif self.radioButton_results_obs_plot_histogram.isChecked():
+            self.init_observation_results_plots_histogram()
+        else:
+            pass
+
+    def init_observation_results_plots_timerseries(self):
+        """Initialize the time series plot for observation results."""
+        if self.glw_obs_results.getItem(0,0) is not None:
+            self.glw_obs_results.removeItem(self.glw_obs_results.getItem(0, 0))
         self.plot_obs_results = self.glw_obs_results.addPlot(0, 0, name='obs_results',
                                                              axisItems={'bottom': TimeAxisItem(orientation='bottom')})
         self.plot_obs_results.setLabel(axis='left', text='')
         self.plot_obs_results.addLegend()
 
-    def plot_observation_results(self, results_obs_df=None, column_name=''):
+    def init_observation_results_plots_histogram(self):
+        """Initialize the histogram plot for observation results."""
+        if self.glw_obs_results.getItem(0,0) is not None:
+            self.glw_obs_results.removeItem(self.glw_obs_results.getItem(0, 0))
+        self.plot_obs_results = self.glw_obs_results.addPlot(0, 0, name='obs_results')
+        self.plot_obs_results.setLabel(axis='left', text='')
+
+    def get_hist_bin_method(self):
+        """Get selected bin method from GUI."""
+        bins = self.comboBox_results_obs_plot_hist_method.currentText()
+        if bins == 'Num. of bins':
+            bins = self.spinBox_results_obs_plot_number_bins.value()
+        return bins
+
+    def on_histogram_bin_method_currentIndexChanged(self):
+        """Select bin determination method."""
+        hist_bin_method = self.comboBox_results_obs_plot_hist_method.currentText()
+        self.comboBox_results_obs_plot_hist_method.setToolTip(
+            settings.NUMPY_HISTOGRAM_BIN_EDGES_OPTIONS[hist_bin_method])
+        if hist_bin_method == 'Num. of bins':
+            self.label_results_obs_plot_number_bins.setEnabled(True)
+            self.spinBox_results_obs_plot_number_bins.setEnabled(True)
+        else:
+            self.label_results_obs_plot_number_bins.setEnabled(False)
+            self.spinBox_results_obs_plot_number_bins.setEnabled(False)
+
+    def plot_observation_results(self, results_obs_df=None, column_name='', type='timeseries'):
         """Plots observation data to the GraphicsLayoutWidget.
 
         Notes
         -----
-        If input parameters `` or/and `` is/are `None` or '', the plot content is deleted and the plot is resetted.
+        If input parameters `` or/and `` is/are `None` or '', the plot content is deleted and the plot is reseted.
         """
         # Clear plot in any case:
         self.plot_obs_results.clear()
+        # Plot time series:
+        if self.radioButton_results_obs_plot_timeseries.isChecked():
+            self.init_observation_results_plots_timerseries()
+            if results_obs_df is not None:  # Data available for plotting
+                # Get data:
+                data = results_obs_df[column_name].values
+                if isinstance(data, np.object):
+                    data = data.astype(float)
+                obs_epoch_timestamps = (results_obs_df['ref_epoch_dt'].values - np.datetime64(
+                    '1970-01-01T00:00:00')) / np.timedelta64(1, 's')
+                plot_name = self.results_observation_model.get_short_column_description(column_name)
+                self.plot_xy_data(self.plot_obs_results, obs_epoch_timestamps, data, plot_name=plot_name, color='b',
+                                  symbol='o', symbol_size=10)
+                self.plot_obs_results.showGrid(x=True, y=True)
+                column_description = self.results_observation_model.get_plotable_columns()[column_name]
+                self.plot_obs_results.setLabel(axis='left', text=column_description)
+                self.plot_obs_results.autoRange()
+
+        # Plot histogram:
+        elif self.radioButton_results_obs_plot_histogram.isChecked():
+            self.init_observation_results_plots_histogram()
+            if results_obs_df is not None:  # Data available for plotting
+                # Get bin method:
+                bins = self.get_hist_bin_method()
+                # Get data:
+                data = results_obs_df[column_name].values
+                if isinstance(data, np.object):
+                    data = data.astype(float)
+                y, x = np.histogram(data, bins=bins)
+                self.plot_obs_results.plot(x, y, stepMode=True, fillLevel=0, brush=(0, 0, 255, 80))
+                self.plot_obs_results.showGrid(x=True, y=True)
+
+                # Add legend with statistics:
+                mean = np.mean(data)
+                median = np.median(data)
+                std = np.std(data)
+                q25 = np.quantile(data, 0.25)
+                q75 = np.quantile(data, 0.75)
+                iqr = q75 - q25
+                legend = self.plot_obs_results.addLegend()
+                legend.setLabelTextColor('k')
+                style1 = pg.PlotDataItem(pen='w')
+                style2 = pg.PlotDataItem(pen='w')
+                style3 = pg.PlotDataItem(pen='w')
+                style4 = pg.PlotDataItem(pen='w')
+                legend.addItem(style1, f'Mean = {mean:0.3f}')
+                legend.addItem(style2, f'Std. = {std:0.3f}')
+                legend.addItem(style3, f'Median = {median:0.3f}')
+                legend.addItem(style4, f'IQR = {iqr:0.3f}')
 
-        if results_obs_df is not None:  # Data available for plotting
-            # Get data:
-            data = results_obs_df[column_name].values
-            if isinstance(data, np.object):
-                data = data.astype(float)
-            obs_epoch_timestamps = (results_obs_df['ref_epoch_dt'].values - np.datetime64(
-                '1970-01-01T00:00:00Z')) / np.timedelta64(1, 's')
-            plot_name = self.results_observation_model.get_short_column_description(column_name)
-            self.plot_xy_data(self.plot_obs_results, obs_epoch_timestamps, data, plot_name=plot_name, color='b',
-                              symbol='o', symbol_size=10)
-            self.plot_obs_results.showGrid(x=True, y=True)
-            column_description = self.results_observation_model.get_plotable_columns()[column_name]
-            self.plot_obs_results.setLabel(axis='left', text=column_description)
-            self.plot_obs_results.autoRange()
+                self.plot_obs_results.autoRange()
+        else:
+            pass
 
     def update_results_obs_plots(self):
         """Update the observation results plots in the results tab."""
         # Get data from selected column
         col_idx, column_name = self.get_selected_obs_data_column()
         if col_idx != -1:
             filtered_results_obs_df = self.results_observation_model.get_model_data_df
@@ -1593,15 +1699,15 @@
 
             # Update widgets:
             self.update_results_station_table_view(idx, station_name=station_name, survey_name=survey_name)
             self.update_results_correlation_matrix_table_view(idx)
             self.update_results_observation_table_view(idx, station_name=station_name, survey_name=survey_name)
             self.update_results_drift_table_view(idx, survey_name=survey_name)
             self.update_results_vg_table_view(idx)
-            self.update_results_obs_plots()  #TODO!! Error wegen dtype Änderung!!
+            self.update_results_obs_plots()
             self.update_drift_plot()
             self.update_vg_plot()
         else:  # invalid index => Reset results views
             self.station_colors_dict_results = {}
             self.label_results_comment.clear()
             self.label_results_adjustment_method.clear()
             self.label_results_number_of_iterations.clear()
@@ -1779,24 +1885,41 @@
                 self.label_obs_setups_tidal_corr.setText(f'{self.setup_model.get_tidal_corr_type} ({settings.TIDE_CORRECTION_TYPES[self.setup_model.get_tidal_corr_type]})')
             else:
                 self.label_obs_setups_tidal_corr.setText(f'{self.setup_model.get_tidal_corr_type}')
         except KeyError:
             self.label_obs_setups_ref_height.setText('')
             self.label_obs_setups_tidal_corr.setText('')
 
-
     def compute_setup_data_for_campaign(self):
         """Compute setup data for the campaign."""
 
         # Get GUI settings:
         active_obs_only_for_ref_epoch = self.dlg_setup_data.checkBox_drift_ref_epoch_active_obs_only.checkState() == Qt.Checked
+        if self.dlg_setup_data.radioButton_variance_weighted_mean.isChecked():
+            method = 'variance_weighted_mean'
+        elif self.dlg_setup_data.radioButton_individual_obs.isChecked():
+            method = 'individual_obs'
+        else:
+            method = 'variance_weighted_mean' # Use default
+        if self.dlg_setup_data.radioButton_sd_from_obsfile.isChecked():
+            method_sd = 'sd_from_obs_file'
+        elif self.dlg_setup_data.radioButton_sd_default_per_obs.isChecked():
+            method_sd = 'sd_default_per_obs'
+        elif self.dlg_setup_data.radioButton_sd_defaul_per_setup.isChecked():
+            method_sd = 'sd_default_per_setup'
+        else:
+            method_sd = 'sd_from_obs_file'
+        default_sd_mugal = self.dlg_setup_data.spinBox_sd_default.value()
 
         try:
             self.campaign.calculate_setup_data(obs_type='reduced',
                                                active_obs_only_for_ref_epoch=active_obs_only_for_ref_epoch,
+                                               method=method,
+                                               method_sd=method_sd,
+                                               default_sd_mugal=default_sd_mugal,
                                                verbose=IS_VERBOSE)
         except AssertionError as e:
             QMessageBox.critical(self, 'Error!', str(e))
             self.statusBar().showMessage(f"Error! No setup data computed")
         except Exception as e:
             QMessageBox.critical(self, 'Error!', str(e))
             self.statusBar().showMessage(f"Error! No setup data computed")
@@ -2262,15 +2385,14 @@
                                     try:
                                         filename_shp = os.path.join(gis_output_dir, filename + '_stat.shp')
                                         lsm_run.export_obs_results_shapefile(filename=filename_shp, epsg_code=epsg_code)
                                     except Exception as e:
                                         QMessageBox.critical(self, 'Error!', str(e))
                                         flag_export_successful = False
 
-
             if flag_export_successful:
                 self.statusBar().showMessage(f"Export to {output_path} successful!")
             else:
                 self.statusBar().showMessage(f"Problems at data export!")
         else:
             self.statusBar().showMessage(f"No exports.")
 
@@ -2323,15 +2445,15 @@
         self.plot_obs_sd_g.clear()
         self.plot_obs_corrections.clear()
         self.plot_obs_tilt.clear()
 
         if obs_df is not None and survey_name is not None:
             setup_df = self.observation_model.get_setup_data
             obs_epoch_timestamps = (obs_df['obs_epoch'].values - np.datetime64(
-                '1970-01-01T00:00:00Z')) / np.timedelta64(1,
+                '1970-01-01T00:00:00')) / np.timedelta64(1,
                                                           's')
             # Plot reduced or unreduced observations:
             flag_show_reduced_observations = False
             if self.checkBox_obs_plot_reduced_observations.checkState() == Qt.Checked and not any(
                     obs_df['g_red_mugal'].isnull()):
                 # Reduced observations are available and will be shown:
                 flag_show_reduced_observations = True
@@ -2343,14 +2465,21 @@
 
                 # Get data:
             if flag_show_reduced_observations:
                 g_mugal = obs_df['g_red_mugal'].astype(float).values
                 sd_g_mugal = obs_df['sd_g_red_mugal'].values
                 corr_tide = obs_df['corr_tide_red_mugal'].values
                 corr_tide_name = self.campaign.surveys[survey_name].red_tide_correction_type
+                try:
+                    corr_description_str = self.campaign.surveys[survey_name].red_tide_correction_description
+                except AttributeError:
+                    pass
+                else:
+                    if corr_description_str:
+                        corr_tide_name = corr_tide_name + ': ' + corr_description_str
                 ref_height_name = self.campaign.surveys[survey_name].red_reference_height_type
             else:
                 g_mugal = obs_df['g_obs_mugal'].values
                 sd_g_mugal = obs_df['sd_g_obs_mugal'].values
                 corr_tide = obs_df['corr_tide_mugal'].values
                 corr_tide_name = self.campaign.surveys[survey_name].obs_tide_correction_type
                 ref_height_name = self.campaign.surveys[survey_name].obs_reference_height_type
@@ -2736,30 +2865,32 @@
         """Launch the about dialog."""
         _ = self.dlg_about.exec()
 
     def on_menu_observations_corrections(self):
         """Launch diaglog to select and apply observation corrections."""
         return_value = self.dlg_corrections.exec()
         if return_value == QDialog.Accepted:
-            flag_corrections_ok, error_msg = self.apply_observation_corrections()
-            if flag_corrections_ok:
-                # Load survey from campaing data to observations vie model:
+            try:
+                self.apply_observation_corrections()
+            except Exception as e:
+                QMessageBox.critical(self, 'Error!', str(e))
+                self.statusBar().showMessage(f"Error: No observation corrections applied.")
+            else:
+                # Load survey from campaign data to observations vie model:
                 self.observation_model.load_surveys(self.campaign.surveys)
                 self.on_obs_tree_widget_item_selected()
                 self.statusBar().showMessage(f"Observation corrections applied.")
-            else:
-                QMessageBox.critical('Error!', error_msg)
-                self.statusBar().showMessage(f"Error: No observation corrections applied.")
         else:
             self.statusBar().showMessage(f"No observation corrections applied.")
 
     def apply_observation_corrections(self):
         """Apply observation corrections according to the selected settings."""
         flag_selection_ok = True
         error_msg = ''
+        tide_corr_timeseries_interpol_method = ''
         if self.dlg_corrections.radioButton_corr_ref_heights_ground.isChecked():
             target_ref_height = 'ground'
         elif self.dlg_corrections.radioButton_corr_ref_heights_control_point.isChecked():
             target_ref_height = 'control_point'
         elif self.dlg_corrections.radioButton_corr_ref_heights_sensor.isChecked():
             target_ref_height = 'sensor_height'
         elif self.dlg_corrections.radioButton_corr_ref_heights_instrument_top.isChecked():
@@ -2771,28 +2902,28 @@
 
         if self.dlg_corrections.radioButton_corr_tides_no_correction.isChecked():
             target_tide_corr = 'no_tide_corr'
         elif self.dlg_corrections.radioButton_corr_tides_cg5_model.isChecked():
             target_tide_corr = 'cg5_longman1959'
         elif self.dlg_corrections.radioButton_corr_tides_longman1959.isChecked():
             target_tide_corr = 'longman1959'
+        elif self.dlg_corrections.radioButton_corr_tides_time_series.isChecked():
+            target_tide_corr = 'from_time_series'
+            tide_corr_timeseries_interpol_method = self.dlg_corrections.comboBox_tides_interpolation_method.currentText()
         else:
             flag_selection_ok = False
             error_msg = f'Invalid selection of tidal correction in GUI (observation corrections dialog).'
             # QMessageBox.critical('Error!', error_msg)
 
         if flag_selection_ok:
-            flag_corrections_ok, error_msg = self.campaign.reduce_observations_in_all_surveys(
+            self.campaign.reduce_observations_in_all_surveys(
                 target_ref_height=target_ref_height,
                 target_tide_corr=target_tide_corr,
+                tide_corr_timeseries_interpol_method=tide_corr_timeseries_interpol_method,
                 verbose=IS_VERBOSE)
-        else:
-            flag_corrections_ok = False
-
-        return flag_corrections_ok, error_msg
 
     @pyqtSlot()
     def on_menu_file_new_campaign(self):
         """Launching dialog to create a new campaign."""
         dlg = DialogNewCampaign(old_campaign=self.campaign)
         return_value = dlg.exec()
         if return_value == QDialog.Accepted:
@@ -2827,14 +2958,16 @@
             # - Results tab:
             self.set_up_results_stations_view_model()
             self.set_up_results_correlation_matrix_view_model()
             self.set_up_results_observations_view_model()
             self.set_up_results_drift_view_model()
             self.set_up_results_vg_view_model()
             self.update_results_tab(select_latest_item=True)
+            # - Corrections time series dialog:
+            self.dlg_correction_time_series.reset_update_gui()
 
             self.statusBar().showMessage(f"New Campaign created (name: {self.campaign.campaign_name}, "
                                          f"output directory: {self.campaign.output_directory})")
             self.setWindowTitle('GravTools - Campaign: ' + self.campaign.campaign_name)
 
         elif return_value == QDialog.Rejected:
             self.statusBar().showMessage(f"Canceled creating new campaign.")
@@ -2927,23 +3060,28 @@
             self.on_checkBox_filter_observed_stat_only_toggled(self.checkBox_filter_observed_stat_only.checkState(),
                                                                auto_range_stations_plot=True)
             # self.update_stations_map() => Called in self.on_checkBox_filter_observed_stat_only_toggled() above!
             number_of_stations_added = self.campaign.stations.get_number_of_stations - number_of_stations_old
 
             # Re-calculate observation corrections, based on the new station data (VG is relevant for height
             # reduction!):
-            self.apply_observation_corrections()
-
-            # Update the observations table and plot (in case the reduced obs. changed):
-            survey_name, setup_id = self.get_obs_tree_widget_selected_item()
-            self.update_obs_table_view(survey_name, setup_id)
-            self.plot_observations(survey_name)
-
-            self.statusBar().showMessage(f"{number_of_stations_added} stations added.")
+            try:
+                self.apply_observation_corrections()
+            except Exception as e:
+                QMessageBox.critical(self, 'Error!', str(e))
+                self.statusBar().showMessage(f"Error: No observation corrections applied.")
+            else:
+                self.statusBar().showMessage(f"Observation corrections applied.")
+            finally:
+                # Update the observations table and plot (in case the reduced obs. changed):
+                survey_name, setup_id = self.get_obs_tree_widget_selected_item()
+                self.update_obs_table_view(survey_name, setup_id)
+                self.plot_observations(survey_name)
 
+                self.statusBar().showMessage(f"{number_of_stations_added} stations added.")
 
     def enable_station_view_options_based_on_model(self):
         """Enable or disable the station view options based on the number of stations in the model."""
         if len(self.station_model._data) > 0:
             self.groupBox_filter_options.setEnabled(True)
             self.groupBox_edit_options.setEnabled(True)
             self.groupBox_stations_map_view_options.setEnabled(True)
@@ -3014,80 +3152,79 @@
             self.tableView_surveys.resizeColumnsToContents()
 
     @pyqtSlot()
     def on_menu_file_load_survey_from_cg5_observation_file(self):
         """Launch file selection dialog to select a CG5 observation file and load the data to the campaign."""
         options = QFileDialog.Options()
         options |= QFileDialog.DontUseNativeDialog
-        cg5_obs_file_filename, _ = QFileDialog.getOpenFileName(self,
+        cg5_obs_file_filenames, _ = QFileDialog.getOpenFileNames(self,
                                                                'Select CG5 observation file',
                                                                self.campaign.output_directory,
                                                                "CG5 observation file (*.TXT)",
                                                                options=options)
-        if cg5_obs_file_filename:
-            # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
-            # operating system.
+        if not cg5_obs_file_filenames:
+            self.statusBar().showMessage(f"No survey data added.")
+            return
+
+        added_surveys_list = []
+        # Add surveys to the campaing:
+        for cg5_obs_file_filename in cg5_obs_file_filenames:
+            # Returns pathName with the '/' separators converted to separators that are appropriate for the
+            # underlying operating system.
             # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
             cg5_obs_file_filename = QDir.toNativeSeparators(cg5_obs_file_filename)
             # Add survey data to Campaign:
             try:
                 new_cg5_survey = Survey.from_cg5_obs_file(cg5_obs_file_filename)
-                flag_no_duplicate = self.campaign.add_survey(survey_add=new_cg5_survey, verbose=IS_VERBOSE)
+                if new_cg5_survey.obs_tide_correction_type == 'unknown':
+                    raise RuntimeError('Type of tidal correction is unknown!')
+                self.campaign.add_survey(survey_add=new_cg5_survey, verbose=IS_VERBOSE)
             except Exception as e:
-                QMessageBox.critical(self, 'Error!', str(e))
-                self.statusBar().showMessage(f"No survey data added.")
+                QMessageBox.critical(self, 'Error!', f'Error while loading {cg5_obs_file_filename}: ' + str(e))
+                # self.statusBar().showMessage(f"No survey data added.")
+                continue
             else:
-                if flag_no_duplicate:
-                    # No problems occurred:
-                    # Check if all expected information is available in the survey and raise warning:
-                    if new_cg5_survey.obs_tide_correction_type == 'unknown':
-                        QMessageBox.warning(self, 'Warning!',
-                                            'Type of tidal correction is unknown! '
-                                            'Check, if the "CG-5 OPTIONS" block in the input file is missing. '
-                                            ' => Reduced observations not calculated yet!')
-                    else:
-                        # Calculate reduced observation data:
-                        if settings.CALCULATE_REDUCED_OBS_WHEN_LOADING_DATA:
-                            flag_corrections_ok, error_msg = self.apply_observation_corrections()
-                            if flag_corrections_ok:
-                                # Load survey from campaing data to observations vie model:
-                                # self.observation_model.load_surveys(self.campaign.surveys)
-                                # self.on_obs_tree_widget_item_selected()
-                                self.statusBar().showMessage(f"Observation corrections applied.")
-                            else:
-                                QMessageBox.critical('Error!', error_msg)
-                                self.statusBar().showMessage(f"Error: No observation corrections applied.")
-                    self.connect_station_model_to_table_view()  # Disconnect sort & filter proxy model from station view.
-                    self.campaign.synchronize_stations_and_surveys(verbose=IS_VERBOSE)
-                    self.refresh_stations_table_model_and_view()
-                    self.populate_survey_tree_widget()
-                    # Select the added survey in the tree view:
-                    for tree_item_idx in range(self.treeWidget_observations.topLevelItemCount()):
-                        if self.treeWidget_observations.topLevelItem(tree_item_idx).text(0) == new_cg5_survey.name:
-                            self.treeWidget_observations.topLevelItem(tree_item_idx).setSelected(True)
-                    self.enable_menu_observations_based_on_campaign_data()
-                    self.statusBar().showMessage(f"Survey {new_cg5_survey.name} "
-                                                 f"({new_cg5_survey.get_number_of_observations()} observations) added.")
-                else:
-                    QMessageBox.warning(self,
-                                        'Warning!',
-                                        f'the current campaign already contains a survey named {new_cg5_survey.name}. '
-                                        f'Survey names have to be unique within a campaign.')
-                    self.statusBar().showMessage(f"No survey data added.")
-            finally:
-                self.set_up_proxy_station_model()  # Re-connect the sort & filter proxy model to the station view.
-                self.set_up_survey_view_model()
-                self.on_checkBox_filter_observed_stat_only_toggled(
-                    state=self.checkBox_filter_observed_stat_only.checkState())
-                self.enable_station_view_options_based_on_model()
-                # Show observed stations only based on Checkbox state:
-                self.on_checkBox_filter_observed_stat_only_toggled(self.checkBox_filter_observed_stat_only.checkState(),
-                                                                   auto_range_stations_plot=True)
-        else:
+                added_surveys_list.append(new_cg5_survey.name + f' ({new_cg5_survey.get_number_of_observations()} obs.)')
+
+        if  not added_surveys_list:
             self.statusBar().showMessage(f"No survey data added.")
+            return
+
+        # Calculate reduced observation data:
+        if settings.CALCULATE_REDUCED_OBS_WHEN_LOADING_DATA:
+            try:
+                self.apply_observation_corrections()
+            except Exception as e:
+                QMessageBox.critical(self, 'Error!', str(e))
+                self.statusBar().showMessage(f"Error: No observation corrections applied.")
+            else:
+                self.statusBar().showMessage(f"Observation corrections applied.")
+
+        self.connect_station_model_to_table_view()
+        self.campaign.synchronize_stations_and_surveys(verbose=IS_VERBOSE)
+        self.refresh_stations_table_model_and_view()
+        self.populate_survey_tree_widget()
+        # Select the added survey in the tree view:
+        for tree_item_idx in range(self.treeWidget_observations.topLevelItemCount()):
+            if self.treeWidget_observations.topLevelItem(tree_item_idx).text(0) == new_cg5_survey.name:
+                self.treeWidget_observations.topLevelItem(tree_item_idx).setSelected(True)
+        self.enable_menu_observations_based_on_campaign_data()
+
+        #
+        self.set_up_proxy_station_model()  # Re-connect the sort & filter proxy model to the station view.
+        self.set_up_survey_view_model()
+        self.on_checkBox_filter_observed_stat_only_toggled(
+            state=self.checkBox_filter_observed_stat_only.checkState())
+        self.enable_station_view_options_based_on_model()
+        # Show observed stations only based on Checkbox state:
+        self.on_checkBox_filter_observed_stat_only_toggled(self.checkBox_filter_observed_stat_only.checkState(),
+                                                           auto_range_stations_plot=True)
+        self.statusBar().showMessage(
+            f'{len(added_surveys_list)} survey added to campaign: ' + ','.join(added_surveys_list))
+
 
     @pyqtSlot()
     def on_manu_observations_flag_observations(self):
         """Load observation list file to flag observations in current campaign accordingly.
 
         The observation list file contains a list of gravity meter observations in CSV format with the following columns:
           - survey_name: Name of the survey
@@ -3243,26 +3380,14 @@
             # Returns pathName with the '/' separators converted to separators that are appropriate for the underlying
             # operating system.
             # On Windows, toNativeSeparators("c:/winnt/system32") returns "c:\winnt\system32".
             oesgn_filename = QDir.toNativeSeparators(oesgn_filename)
             self.lineEdit_oesgn_table_file_path.setText(oesgn_filename)
 
 
-class DialogCorrections(QDialog, Ui_Dialog_corrections):
-    """Dialog to select and apply observation corrections."""
-
-    def __init__(self, parent=None):
-        super().__init__(parent)
-
-        # Run the .setupUi() method to show the GUI
-        self.setupUi(self)
-        # connect signals and slots:
-        pass
-
-
 class DialogAutoselectSettings(QDialog, Ui_Dialog_autoselection_settings):
     """Dialog to define the autoselect settings."""
 
     def __init__(self, parent=None):
         super().__init__(parent)
 
         # Run the .setupUi() method to show the GUI
```

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_misc.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_observation_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_observation_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_correlation_matrix_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_correlation_matrix_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_drift_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_drift_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_obs_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_obs_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_stat_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_stat_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_results_vg_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_results_vg_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_setup_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_setup_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_station_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_station_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/gui/gui_model_survey_table.py` & `grav-toolbox-0.2.0/gravtools/gui/gui_model_survey_table.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/models/__init__.py` & `grav-toolbox-0.2.0/gravtools/models/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/models/campaign.py` & `grav-toolbox-0.2.0/gravtools/models/campaign.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 from gravtools.models.lsm import LSM
 from gravtools.models.lsm_diff import LSMDiff
 from gravtools.models.vg_lsm import VGLSM
 from gravtools.models.lsm_nondiff import LSMNonDiff
 from gravtools.models.mlr_bev_legacy import BEVLegacyProcessing
 from gravtools.models.survey import Survey
 from gravtools.models.station import Station
+from gravtools.tides.correction_time_series import CorrectionTimeSeries
 from gravtools.settings import ADDITIVE_CONST_ABS_GRTAVITY, GRAVIMETER_TYPES_KZG_LOOKUPTABLE, \
     GRAVIMETER_SERIAL_NUMBER_TO_ID_LOOKUPTABLE, GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m, EXPORT_OBS_LIST_COLUMNS, \
     MAX_SD_FOR_EXPORT_TO_NSB_FILE, WRITE_COMMENT_TO_NSB, PICKLE_PROTOCOL_VERSION
 from gravtools import __version__ as GRAVTOOLS_VERSION
 
 
 class Campaign:
@@ -44,14 +45,15 @@
 
     - Campaign name
     - One or more gravity surveys that belong together and
       - Each survey was observed with one gravimeter on a single day
     - Station data (datum and non-datum stations)
     - Reductions and corrections
       - All observations (from surveys) are corrected and reduced in the same way
+    - Time series data for the correction of gravity observations (optional)
 
     Attributes
     ----------
     campaign_name : str
         Name of the campaign.
     output_directory : str
         Path to output directory (all output files are stored there).
@@ -61,14 +63,17 @@
         Data of known stations (datum- and non-datum-stations).
     lsm_runs : list of objects inherited from :py:obj:`gravtools.models.lsm.LSM`
         Each item in the list contains one enclosed LSM object. Each LSM object reflects one dedicated run of an
         least-squares adjustment in order to estimate target parameters.
     ref_delta_t_dt : datetime object
         Reference epoch for relative times within the campaign, e.g. for the determination of the drift polynomials.
         This reference time is equalt to the first (active) observation in the campaign considering all surveys.
+    correction_time_series : :py:obj:`CorrectionTimeSeries`
+        Contains time series data for correcting gravity observations.
+
     gravtools_version : str
         Version of the gravtools software that was used to create the dataset.
     """
 
     def __init__(self,
                  campaign_name,
                  output_directory,
@@ -151,46 +156,51 @@
             if not isinstance(ref_delta_t_dt, dt.datetime):
                 raise TypeError('`ref_delta_t_dt` needs to be a datetime object.')
         self.ref_delta_t_dt = ref_delta_t_dt
 
         # Version of gravtools:
         self.gravtools_version = GRAVTOOLS_VERSION
 
+        # Correction time series object:
+        self.correction_time_series = CorrectionTimeSeries()
+
+    def add_empty_correction_time_series(self):
+        """Adds an empty `CorrectionTimeSeries` object to the campaign.
+
+        Notes
+        -----
+        This is required, e.g. if a campaign object os loaded into GravTools from a previous GRavTools version without
+        support of time series corrections.
+        """
+        self.correction_time_series = CorrectionTimeSeries()
+
     def add_survey(self, survey_add: Survey, verbose=False) -> bool:
         """Add a survey to campaign and specify whether to use it for ths analysis.
 
         Notes
         -----
         A survey can only be added, f the survey's name is unique within the campaign.
 
         Parameters
         ----------
         survey_add : :py:obj:`.Survey`
             Contains all information of s specific survey independent of the data source.
         verbose : bool, optional (default=False)
             If True, status messages are printed to the command line.
-
-        Returns
-        -------
-        bool
-            True, if the survey was successfully added; False, if not.
         """
         # Check if a survey with the dame name ("survey_add.name") already exists in this campaign:
         # - Raise warning:
         if survey_add.name in self.surveys.keys():
-            if verbose:
-                print(f'Warnung: the current campaign already contains a survey named {survey_add.name}.')
-                print(' - Survey names need to be unique within a campaign.')
-            return False
+            raise RuntimeError(f'The campaign already contains a survey named {survey_add.name}. Survey names need to '
+                               f'be unique within a campaign!')
         else:
             # Add survey:
             self.surveys[survey_add.name] = survey_add
             if verbose:
                 print(f"Survey {survey_add.name} added to the campaign.")
-            return True
 
     def remove_survey(self, survey_name: str, verbose=False) -> bool:
         """Remove survey with the specified name from the campaign
 
         Parameters
         ----------
         survey_name : str
@@ -318,15 +328,18 @@
         return len(self.surveys)
 
     @property
     def number_of_stations(self) -> int:
         """int : Returns the number of stations in this campaign."""
         return self.stations.get_number_of_stations
 
-    def reduce_observations_in_all_surveys(self, target_ref_height=None, target_tide_corr=None, verbose=False):
+    def reduce_observations_in_all_surveys(self, target_ref_height=None,
+                                           target_tide_corr=None,
+                                           tide_corr_timeseries_interpol_method='',
+                                           verbose=False):
         """Reduce the observed gravity by applying the specified corrections.
 
         Notes
         -----
         - For this reduction vertical gravity gradients are required. They are obtained from the `Station` object.
           Hence, a `Station` object has to be attached to the Campaign object beforehand.
 
@@ -337,48 +350,35 @@
         target_ref_height : string, specifying the target reference height type (default = `None`).
             The target reference height type has to be listed in :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`.
             Default is `None` indicating that the reference heights of the input data are not changed.
         target_tide_corr : str, specifying the tidal correction type to be applied (default = `None`).
             The target tidal correction type specifies what kind of tidal correction will be applied. Valid types have
             to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`. Default is `None` indicating that the
             tidal corrections are not considered here (tidal corrections are inherited from input data).
+        tide_corr_timeseries_interpol_method : str, optional (default='')
+            Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
+            obtained from other sources or models, this attribute is irrelevant and has to be empty!
         verbose : bool, optional (default=False)
             If True, status messages are printed to the command line.
-
-        Returns
-        -------
-        flag_corrections_applied_correctly : bool, default = True
-            `False` indicates that an error occurred when applying the observation corrections.
-        error_msg : str, default = ''
-            Message that describes the error in case an error occurred.
-
         """
-        flag_corrections_applied_correctly = True
-        error_msg = ''
         if verbose:
             print(f'## Reduce all observation in this campaign:')
         for survey_name, survey in self.surveys.items():
             if verbose:
                 print(f'Survey {survey_name}:')
             if target_ref_height is not None:
                 if verbose:
                     print(f' - Get vertical gradients')
                 survey.obs_df_populate_vg_from_stations(self.stations, verbose=verbose)
-            flag_corrections_applied_correctly, error_msg = survey.reduce_observations(
+            survey.reduce_observations(
                 target_ref_height=target_ref_height,
                 target_tide_corr=target_tide_corr,
+                tide_corr_timeseries_interpol_method=tide_corr_timeseries_interpol_method,
+                correction_time_series=self.correction_time_series,
                 verbose=verbose)
-            # Check, if corrections were applied correctly and return error message if an error occurred:
-            if not flag_corrections_applied_correctly:
-                error_msg = f'Survey: {survey_name}: ' + error_msg
-                if verbose:
-                    print(error_msg)
-                return flag_corrections_applied_correctly, error_msg
-                # raise AssertionError('Reduction to reference height failed!')
-        return flag_corrections_applied_correctly, error_msg
 
     def add_stations_from_oesgn_table_file(self, oesgn_filename, is_datum=False, verbose=False):
         """Add station from an OESGN table file.
 
         Parameters
         ----------
         oesgn_filename : string, specifying the path and filename of the OESGN file
@@ -447,14 +447,17 @@
             if verbose:
                 print(f' - Survey: {survey_name}')
             self.stations.add_stations_from_survey(survey, verbose)
 
     def calculate_setup_data(self,
                              obs_type='reduced',
                              active_obs_only_for_ref_epoch=True,
+                             method='variance_weighted_mean',
+                             method_sd='sd_from_obs_file',
+                             default_sd_mugal=100.0,
                              verbose=False):
         """Calculate accumulated pseudo observations for each active setup in all active surveys.
 
         Notes
         -----
         Two relative reference epochs are calculated for each setup: (a) w.r.t. the first (active) observation in the
         whole campaign and (b) w.r.t. the first (active) observation in each survey. Both reference time do not differ
@@ -462,21 +465,30 @@
         parameter `active_obs_only_for_ref_epoch`.
 
         Parameters
         ----------
         obs_type : str, 'observed' or 'reduced' (default)
             Defines whether the observed (as loaded from an observation file) or the reduced observations from
             `self.obs_df` are used to determine the weighted mean values per setup.
-        set_epoch_of_first_obs_as_reference: bool, optional (default=True)
-            If `True`, the epoch of the first observation in all surveys in the campaign is used as reference epoch
-            for all surveys. `False` implies that the reference epoch is based on the first (active, if
-            `active_obs_only_for_ref_epoch` is `True`) observation in each survey and determined individually for
-            each survey. Stored in `self.ref_delta_t_dt` (datetime object).
         active_obs_only_for_ref_epoch: bool, optional (default=True)
             `True` implies that the relative reference epochs are determined by considering active observations only.
+        method : str, optional (default=`variance_weighted_mean`)
+            Select method for the calculation of setup data. `variance_weighted_mean` implies that setup observations
+            (observed gravity, standard deviations and reference time) are calculated by variance weighted mean of the
+            individual observations. `individual_obs` implies that the original observations are used as setup data
+            without any aggregation.
+        method_sd : str, optional (default='sd_from_obs_file')
+            Method for the determination of standard deviations (SD) of setup observations. `sd_from_obs_file` implies that
+            SD are taken from the observation file. `sd_default_per_obs` and `sd_default_per_setup` imply that the
+            given default SD is used, where the default SD is applied the individual observations in the first case and
+            to setups in the second case. If applied to observations, the number of observations per setup still plays a
+            role for weighting the setup observations in the adjustment.
+        default_sd_mugal : float, optional (default=100.0)
+            Default standard deviation [µGal] that is used to determine the SD of setup observations when `method_sd` is
+            `sd_default_per_obs` or `sd_default_per_setup`
         verbose : bool, optional (default=False)
             If `True`, status messages are printed to the command line.
         """
         # Get reference epoch:
         self.ref_delta_t_dt = self.get_epoch_of_first_observation(active_obs_only_for_ref_epoch)
 
         # Loop over all surveys in the campaign:
@@ -485,14 +497,17 @@
         for survey_name, survey in self.surveys.items():
             if verbose:
                 print(f' - Survey: {survey_name}')
             if survey.is_active and survey.keep_survey:
                 survey.calculate_setup_data(obs_type=obs_type,
                                             ref_delta_t_campaign_dt=self.ref_delta_t_dt,
                                             active_obs_only_for_ref_epoch=active_obs_only_for_ref_epoch,
+                                            method=method,
+                                            method_sd=method_sd,
+                                            default_sd_mugal=default_sd_mugal,
                                             verbose=verbose)
             else:
                 survey.reset_setup_data(verbose)  # Remove setup data from previous calculations
 
     def get_epoch_of_first_observation(self, active_obs_only_for_ref_epoch=True):
         """Returns the epoch of the first (active) observation in this campaign.
```

### Comparing `grav-toolbox-0.1.9/gravtools/models/exceptions.py` & `grav-toolbox-0.2.0/gravtools/models/exceptions.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/models/lsm.py` & `grav-toolbox-0.2.0/gravtools/models/lsm.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,14 +241,15 @@
                                              f'differential observations!')
                     else:
                         setup_data_dict = {'ref_epoch_delta_t_h': survey.ref_delta_t_dt,
                                            'ref_epoch_delta_t_campaign_h': campaign.ref_delta_t_dt,
                                            'setup_df': survey.setup_df,
                                            'tide_correction_type': survey.setup_tide_correction_type,
                                            'reference_height_type': survey.setup_reference_height_type,
+                                           'setup_calc_method': survey.setup_calc_method,
                                            'setup_obs_list_df': survey.setup_obs_list_df}
                         setups[survey_name] = setup_data_dict
 
         # Check if setup data is available:
         if len(setups) == 0:
             raise AssertionError(f'Setup data of campaign "{campaign.campaign_name}" does not contain observations!')
 
@@ -573,14 +574,30 @@
     def get_results_vg_df(self):
         """Getter for the results of vertical gravity gradient estimation."""
         try:
             return self.vg_pol_df
         except AttributeError:  # If "self" has no attribute "vg_pol_df" (not initialized)
             return None
 
+    @property
+    def check_for_unique_setup_id(self):
+        """Indicates whether setup IDs should be unique based on the setup data calculation method.
+
+        Returns
+        -------
+        bool : `True`, if the setup IDs should be unique, otherwise `False`.
+
+        Notes
+        -----
+        If observations were not aggregated within at least one setup, checking for unique setup IDs makes no sense.
+        """
+        for survey_name, setup_data in self.setups.items():
+            if setup_data['setup_calc_method'] == 'individual_obs':
+                return False
+        return True
 
 def bin_redundacy_components(mat_r):
     """Bin redundancy components for easier interpretatzion.
 
     See: Skriptum AG2 (Navratil, TU Wien), p. 70.
     """
     number_obs_r_equal_0 = 0  # No error control: Errors cannot be detected
```

### Comparing `grav-toolbox-0.1.9/gravtools/models/lsm_diff.py` & `grav-toolbox-0.2.0/gravtools/models/lsm_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,33 +46,14 @@
         Pandas Dataframes for logging (differential or absolute) setup observations, the related metadata, estimation
         results and statistics. The columns of the dataframe are defined in `self._SETUP_DIFF_COLUMNS`.
     observed_stations : list of str
         Unique list of names of observed stations, defining the order of stations (station IDs) for all matrices and
         vectors used in the adjustment scheme.
     """
 
-    # Column names of self.setup_obs_df:
-    # - keys: Column names of the pandas dataframe
-    # - values: Short description for table headers, etc., in the GUI
-    # _SETUP_DIFF_COLUMNS_DICT = {
-    #     'survey_name': 'Survey',
-    #     'ref_epoch_dt': 'Epoch',
-    #     'diff_obs_id': 'Obs. ID',
-    #     'station_name_from': 'Station from',
-    #     'station_name_to': 'Station to',
-    #     'setup_id_from': 'Setup ID from',
-    #     'setup_id_to': 'Setup ID to',
-    #     'g_diff_mugal': 'g [µGal]',
-    #     'sd_g_diff_mugal': 'SD [µGal]',
-    #     'sd_g_diff_est_mugal': 'SD_est [µGal]',
-    #     'v_diff_mugal': 'Residuals [µGal]',  # Post fit residuals
-    #     'w_diff_mugal': 'Std. Residual []',
-    #     'r_diff_obs': 'Redundancy []',
-    #     'tau_test_result': 'Outlier Test',
-    # }
     _SETUP_DIFF_COLUMNS_DTYPES = {
         'survey_name': 'str',
         'ref_epoch_dt': 'datetime64[ns, UTC]',
         'diff_obs_id': 'int',
         'station_name_from': 'str',
         'station_name_to': 'str',
         'setup_id_from': 'int',
@@ -242,16 +223,17 @@
             self.observed_stations)  # Unique list of stations => order of stations in matrices!
         number_of_stations = len(self.observed_stations)
         number_of_surveys = len(self.setups)
         number_of_parameters = number_of_stations + drift_pol_degree * number_of_surveys  # Total number of parameters to be estimated
         number_of_diff_obs = number_of_observations - number_of_surveys
 
         # Check, if setup IDs are unique:
-        if len(set(setup_ids)) != len(setup_ids):
-            raise AssertionError('Setup IDs are not unique within the campaign!')
+        if self.check_for_unique_setup_id:
+            if len(set(setup_ids)) != len(setup_ids):
+                raise AssertionError('Setup IDs are not unique within the campaign!')
 
         # - Datum points for weighted constraints:
         # Get dataframe with subset of observed stations only:
         filter_tmp = self.stat_df['station_name'].isin(self.observed_stations)
         self.stat_obs_df = self.stat_df.loc[filter_tmp].copy(deep=True)  # All observed stations
         filter_tmp = self.stat_obs_df['is_datum'] == True
         stat_df_obs_datum = self.stat_obs_df.loc[filter_tmp]
```

### Comparing `grav-toolbox-0.1.9/gravtools/models/lsm_nondiff.py` & `grav-toolbox-0.2.0/gravtools/models/lsm_nondiff.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,31 +44,14 @@
         Pandas Dataframes for logging (differential or absolute) setup observations, the related metadata, estimation
         results and statistics. The columns of the dataframe are defined in `self._SETUP_OBS_COLUMNS`.
     observed_stations : list of str
         Unique list of names of observed stations, defining the order of stations (station IDs) for all matrices and
         vectors used in the adjustment scheme.
     """
 
-    # Column names of self.setup_obs_df:
-    # - keys: Column names of the pandas dataframe
-    # - values: Short description for table headers, etc., in the GUI
-    #_SETUP_OBS_COLUMNS_DICT = {
-    #    'survey_name': 'Survey',
-    #    'ref_epoch_dt': 'Epoch',
-    #    'obs_id': 'Obs. ID',
-    #    'station_name': 'Station',
-    #    'setup_id': 'Setup ID',
-    #    'g_obs_mugal': 'g [µGal]',
-    #    'sd_g_obs_mugal': 'SD [µGal]',
-    #    'sd_g_obs_est_mugal': 'SD_est [µGal]',
-    #    'v_obs_est_mugal': 'Residuals [µGal]',  # Post fit residuals
-    #    'w_obs_est_mugal': 'Std. Residual []',
-    #    'r_obs_est': 'Redundancy []',
-    #    'tau_test_result': 'Outlier Test',
-    #}
     _SETUP_OBS_COLUMNS_DTYPES = {
         'survey_name': 'str',
         'ref_epoch_dt': 'datetime64[ns, UTC]',
         'obs_id': 'int',
         'station_name': 'str',
         'setup_id': 'int',
         'g_obs_mugal': 'float',
@@ -230,16 +213,17 @@
         # - 1 g value per station
         # - Drift polynomial coeff. per survey: Polynomial degree * number of surveys
         # - 1 constant instrumental bias per survey
         number_of_parameters = number_of_stations + drift_pol_degree * number_of_surveys + number_of_surveys
         # number_of_diff_obs = number_of_observations - number_of_surveys
 
         # Check, if setup IDs are unique:
-        if len(set(setup_ids)) != len(setup_ids):
-            raise AssertionError('Setup IDs are not unique within the campaign!')
+        if self.check_for_unique_setup_id:
+            if len(set(setup_ids)) != len(setup_ids):
+                raise AssertionError('Setup IDs are not unique within the campaign!')
 
         # - Datum points for weighted constraints:
         # Get dataframe with subset of observed stations only:
         filter_tmp = self.stat_df['station_name'].isin(self.observed_stations)
         self.stat_obs_df = self.stat_df.loc[filter_tmp].copy(deep=True)  # All observed stations
         stat_df_obs_datum = self.stat_obs_df.loc[self.stat_obs_df['is_datum']]
         datum_stations = stat_df_obs_datum['station_name'].to_list()
```

### Comparing `grav-toolbox-0.1.9/gravtools/models/misc.py` & `grav-toolbox-0.2.0/gravtools/models/misc.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/models/mlr_bev_legacy.py` & `grav-toolbox-0.2.0/gravtools/models/mlr_bev_legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,16 +164,17 @@
 
         # Check if the drift polynomial reference epoch refers to the same time (campaign start) for all surveys:
         if len(set(ref_epoch_t0_dt_list)) > 1:
             raise AssertionError(f'The drift polynomial reference epochs do not match!')
         ref_epoch_t0_dt = ref_epoch_t0_dt_list[0]
 
         # Check, if setup IDs are unique:
-        if len(set(setup_ids)) != len(setup_ids):
-            raise AssertionError('Setup IDs are not unique within the campaign!')
+        if self.check_for_unique_setup_id:
+            if len(set(setup_ids)) != len(setup_ids):
+                raise AssertionError('Setup IDs are not unique within the campaign!')
 
         # Write log:
         if verbose or self.write_log:
             time_now_str = dt.datetime.now(tz=pytz.UTC).strftime('%Y-%m-%d, %H:%M:%S %Z')
             tmp_str = f'#### Adjustment log (MLR, BEV legacy) ####\n'
             tmp_str += f'Processed with GravTools {GRAVTOOLS_VERSION} ({time_now_str})\n'
             tmp_str += f'Comment: {self.comment}\n'
```

### Comparing `grav-toolbox-0.1.9/gravtools/models/station.py` & `grav-toolbox-0.2.0/gravtools/models/station.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/models/survey.py` & `grav-toolbox-0.2.0/gravtools/models/survey.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,18 +20,20 @@
 import datetime as dt
 import os
 
 import gravtools.models.lsm_diff
 import gravtools.tides.longman1959
 from gravtools.settings import SURVEY_DATA_SOURCE_TYPES, TIDE_CORRECTION_TYPES, DEFAULT_GRAVIMETER_TYPE_CG5_SURVEY, \
     REFERENCE_HEIGHT_TYPE, BEV_GRAVIMETER_TIDE_CORR_LOOKUP, GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m, \
-    GRAVIMETER_SERIAL_NUMBERS, GRAVIMETER_TYPES, GRAVIMETER_SERIAL_NUMBER_TO_ID_LOOKUPTABLE
+    GRAVIMETER_SERIAL_NUMBERS, GRAVIMETER_TYPES, GRAVIMETER_SERIAL_NUMBER_TO_ID_LOOKUPTABLE, SETUP_CALC_METHODS, \
+    UNIT_CONVERSION_TO_MUGAL, SETUP_SD_METHODS
 from gravtools.const import VG_DEFAULT
 from gravtools.CG5_utils.cg5_survey import CG5Survey
 from gravtools.models.misc import format_seconds_to_hhmmss
+from gravtools.tides.correction_time_series import convert_to_mugal
 
 
 class Survey:
     """Gravity survey (instrument-independent).
 
     A gravity survey object contains all data that belongs to a single field observation job, carried out under the
     same circumstances (same instrument, measurement area, drift- and datum-point planing, same observer, etc.). A
@@ -42,14 +44,15 @@
     corrections/reductions are supported:
 
     - Tidal corrections of observations
 
       - Corrections of the CG-5 instruments provided in the observation files (Longman, 1959)
       - No corrections
       - Longman (1959) model, evaluated in GravTools for the longitude, latitude , altitude and UTC time stamp of each observation. The correction is calculated for the middle of the readint time (obs_epoch + duration_sec/2)
+      - Interpolated from correction time series (e.g. loaded from Tsoft TSF files)
 
     - Reduction of the observed gravity to different reference height levels
 
       - Control point level
       - Ground level
       - Level of the gravimeter top
       - Sensor level
@@ -57,21 +60,21 @@
     Notes
     -----
     Basically it is possible to initialize an empty survey, by just defining the survey's name on the instantiation
     step. In this case all other (class and instance) attributes are initialized with the default values listed below
     in the Attributes section.
 
     The observation reference time in GravTools is equal to the start time of an instrument reading - in accordance with
-    the CG-5 observation files. This has to be taken into account when calcualting time dependent corrections, such as
+    the CG-5 observation files. This has to be taken into account when calculating time dependent corrections, such as
     tidal corrections.
 
     Attributes
     ----------
     name : str
-        Name of the survey. This parameter is mandatory!
+        Name of the survey
     date :
         Date of te survey.
     operator : str, optional (default='')
         Name of the responsible operator that carried out the observations of this survey.
     gravimeter_serial_number : str, optional (default='')
         Valid gravimeter types have to be listed in :py:obj:`gravtools.settings.GRAVIMETER_SERIAL_NUMBERS`.
     gravimeter_type: str, optional (default='')
@@ -93,22 +96,43 @@
         Type of the tidal corrections applied on the reduced observations (column `g_red_mugal` in `obs_df`). Valid
         entries have to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`. `Empty string`, if corrected
         observations are not available.
     red_reference_height_type : str, optional (default='')
         Reference level type of the reduced observations (column `g_red_mugal` in `obs_df`). Valid entries have to be
         listed in :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`. `Empty string`, if corrected observations are not
         available.
+    red_tide_correction_description : str, optional (default='')
+        Optional description of the tide correction e.g. obtained from time series data. The reduced observations are
+        stored in the column `g_red_mugal` and the corrections in column `corr_tide_red_mugal` in `obs_df`. Only
+    red_tide_corr_timeseries_interpol_method : str, optional (default='')
+        Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
+        obtained from other sources or models, this attribute is irrelevant and has to be empty!
+    red_tide_corr_timeseries_creation_dt : `datetime`, optional (default=`None`)
+        If tidal corrections are obtained from time series data, the time when the data was created, i.e. loaded into
+        GravTools, is stored here as `datetime` object. This is required to uniquely identify the applies tidal
+        corrections from time series data.
     setup_tide_correction_type : str, optional (default='')
         Type of the tidal corrections applied on the observations that are used to calculate the setup data in the
         `setup_df` dataframe. Valid entries have to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`.
         `Empty string`, if corrected setup data has not been calculated so far (`setup_df` = None).
     setup_reference_height_type : str, optional (default='')
         Reference height reduction type applied on the observations that are used to calculate the setup data in the
         `setup_df` dataframe. Valid entries have to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`.
         `Empty string`, if corrected setup data has not been calculated so far (`setup_df` = None).
+    setup_calc_method : str, optional (default='')
+        Method for the calculation of setup data. `variance_weighted_mean` implies that setup observations
+        (observed gravity, standard deviations and reference time) are calculated by variance weighted mean of the
+        individual observations. `individual_obs` implies that the original observations are used as setup data
+        without any aggregation.
+    setup_sd_method : str, optional (default='')
+        Method for the determination of standard deviations (SD) of setup observations. `sd_from_obs_file` implies that
+        SD are taken from the observation file. `sd_default_per_obs` and `sd_default_per_setup` imply that the
+        given default SD is used, where the default SD is applied the individual observations in the first case and
+        to setups in the second case. If applied to observations, the number of observations per setup still palys a
+        role for weighting the setup observations in the adjustment.
     keep_survey : bool (default=True)
         Flag that indicates whether this survey will be used to derive setup observations.`True` is the
         default and implies that this survey is considered. This flag is independent of the `keep_obs` flags
         in the `obs_df` dataframe (used to flag individual observations).
     obs_df : :py:obj:`pandas.core.frame.DataFrame`, optional (default=None)
         Contains all observation data that belongs to this survey. One observation per line. If `None`, no observations
         have been assigned to the survey. All Columns are listed in :py:obj:`.Survey._OBS_DF_COLUMNS`:
@@ -287,26 +311,28 @@
                  data_file_name='',
                  data_file_type='',
                  obs_df=None,
                  obs_tide_correction_type='',  # of "g_obs_mugal"
                  obs_reference_height_type='',  # of "g_obs_mugal"
                  red_tide_correction_type='',  # of "g_red_mugal"
                  red_reference_height_type='',  # of "g_red_mugal"
+                 red_tide_correction_description='',  # of "g_red_mugal"
+                 red_tide_corr_timeseries_interpol_method='',  # of "g_red_mugal"
+                 red_tide_corr_timeseries_creation_dt=None,  # of "g_red_mugal"
                  setup_tide_correction_type='',
                  setup_reference_height_type='',
+                 setup_calc_method='',
+                 setup_sd_method='',
                  keep_survey=True,  # Flag
                  setup_df=None,
                  ref_delta_t_dt=None,  # Datetime object (UTC)
                  setup_obs_list_df=None  #
                  ):
         """Default constructor of class Survey."""
 
-
-
-
         # Check input arguments:
         # name:
         if name is not None:
             if isinstance(name, str):
                 if len(name) > 0:
                     self.name = name
                 else:
@@ -442,14 +468,32 @@
                     raise ValueError('"red_reference_height_type" needs to be a key in REFERENCE_HEIGHT_TYPE '
                                      '({})'.format(', '.join(REFERENCE_HEIGHT_TYPE.keys())))
             else:
                 self.red_reference_height_type = red_reference_height_type  # None
         else:
             raise TypeError('"red_tide_correction_type" needs to be a string')
 
+        # red_tide_correction_description
+        if isinstance(red_tide_correction_description, str):
+            self.red_tide_correction_description = red_tide_correction_description
+        else:
+            raise TypeError('"red_tide_correction_description" needs to be a string')
+
+        # red_tide_corr_timeseries_interpol_method
+        if isinstance(red_tide_corr_timeseries_interpol_method, str):
+            self.red_tide_corr_timeseries_interpol_method = red_tide_corr_timeseries_interpol_method
+        else:
+            raise TypeError('"red_tide_corr_timeseries_interpol_method" needs to be a string')
+
+        # red_tide_corr_timeseries_creation_dt
+        if red_tide_corr_timeseries_creation_dt is not None:
+            if not isinstance(red_tide_corr_timeseries_creation_dt, dt.datetime):
+                raise TypeError('`red_tide_corr_timeseries_creation_dt` needs to be a datetime object.')
+        self.red_tide_corr_timeseries_creation_dt = red_tide_corr_timeseries_creation_dt
+
         # setup_tide_correction_type:
         if isinstance(setup_tide_correction_type, str):
             if setup_tide_correction_type:
                 if setup_tide_correction_type in REFERENCE_HEIGHT_TYPE.keys():
                     self.setup_tide_correction_type = setup_tide_correction_type
                 else:
                     raise ValueError('"setup_tide_correction_type" needs to be a key in REFERENCE_HEIGHT_TYPE '
@@ -468,14 +512,40 @@
                     raise ValueError('"setup_reference_height_type" needs to be a key in REFERENCE_HEIGHT_TYPE '
                                      '({})'.format(', '.join(REFERENCE_HEIGHT_TYPE.keys())))
             else:
                 self.setup_reference_height_type = setup_reference_height_type  # ''
         else:
             raise TypeError('"setup_reference_height_type" needs to be a string')
 
+        # setup_calc_method:
+        if isinstance(setup_calc_method, str):
+            if setup_calc_method:
+                if setup_calc_method in SETUP_CALC_METHODS.keys():
+                    self.setup_calc_method = setup_calc_method
+                else:
+                    raise ValueError('"setup_calc_method" needs to be a key in SETUP_CALC_METHODS '
+                                     '({})'.format(', '.join(SETUP_CALC_METHODS.keys())))
+            else:
+                self.setup_calc_method = setup_calc_method  # ''
+        else:
+            raise TypeError('"setup_calc_method" needs to be a string')
+
+        # setup_sd_method:
+        if isinstance(setup_sd_method, str):
+            if setup_sd_method:
+                if setup_sd_method in SETUP_SD_METHODS.keys():
+                    self.setup_sd_method = setup_sd_method
+                else:
+                    raise ValueError('"setup_sd_method" needs to be a key in SETUP_SD_METHODS '
+                                     '({})'.format(', '.join(SETUP_SD_METHODS.keys())))
+            else:
+                self.setup_sd_method = setup_sd_method  # ''
+        else:
+            raise TypeError('"setup_sd_method" needs to be a string')
+
         # keep_survey
         if isinstance(keep_survey, bool):
             self.keep_survey = keep_survey
         else:
             raise TypeError('"keep_survey" needs to be a bool type.')
 
         # setup_df:
@@ -959,16 +1029,21 @@
         self.obs_df.loc[self.obs_df['vg_mugalm'].isna(), 'vg_mugalm'] = VG_DEFAULT
 
         # Drop columns that are not required and check for validity:
         self.obs_df_drop_redundant_columns()
         if not self.is_valid_obs_df():
             raise AssertionError('The DataFrame "obs_df" is not valid.')
 
-    def reduce_observations(self, target_ref_height: str = None, target_tide_corr: str = None,
-                            verbose: bool = False) -> [bool, str]:
+    def reduce_observations(self,
+                            target_ref_height: str = None,
+                            target_tide_corr: str = None,
+                            tide_corr_timeseries_interpol_method = '',
+                            correction_time_series=None,
+                            verbose: bool = False,
+                            ) -> [bool, str]:
         """Reduce the observed gravity values by applying the selected corrections.
 
         The following corrections can be applied:
 
         - Reference height: Using the vertical gravity gradient at the measurement points (from station data file) and
           the vertical distances between instrument top, sensor height, ground and control point, the observations are
           reduced to the selected reference height. Information on the reference height of the input data (usually
@@ -987,27 +1062,26 @@
         target_ref_height : string, specifying the target reference height type (default = `None`).
             The target reference height type has to be listed in :py:obj:`gravtools.settings.REFERENCE_HEIGHT_TYPE`.
             Default is `None` indicating that the reference heights of the input data are not changed.
         target_tide_corr : str, specifying the tidal correction type to be applied (default = `None`).
             The target tidal correction type specifies what kind of tidal correction will be applied. Valid types have
             to be listed in :py:obj:`gravtools.settings.TIDE_CORRECTION_TYPES`. Default is `None` indicating that the
             tidal corrections are not considered here (tidal corrections are inherited from input data).
+        tide_corr_timeseries_interpol_method : str, optional (default='')
+            Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
+            obtained from other sources or models, this attribute is irrelevant and has to be empty!
+        correction_time_series : `CorrectionTimeSeries` object, optional (default=None)
+            Correction time series object that contains time series of tidal corrections for stations in surveys. This
+            argument is required, if tidal corrections should be derived from time series data, i.e. if
+            `self.target_tide_corr = from_time_series`.
         verbose : bool, optional (default=False)
             If `True`, status messages are printed to the command line.
-
-        Returns
-        -------
-        flag_corrections_applied_correctly : bool
-            `False` indicates that an error occurred when applying the observation corrections.
-        error_msg : str, default = ''
-            Message that describes the error in case an error occurred.
         """
         # Init.:
-        flag_corrections_applied = True
-        error_msg = ''
+        tide_corr_timeseries_interpol_method_out = ''
 
         # Create a copy auf obs_df in order prevent problems with manipulation assigned py reference variables:
         obs_df = self.obs_df.copy(deep=True)
 
         # Initialize pandas series for reduced data by copying the observation data as loaded from the input file:
         g_red_mugal = obs_df['g_obs_mugal']
         sd_g_red_mugal = obs_df['sd_g_obs_mugal']
@@ -1018,56 +1092,47 @@
                                       obs_df['corr_tide_red_mugal'].isna().all()
                                       ])
         flag_no_field_is_nan = all([
             all(~obs_df['g_red_mugal'].isna().values),
             all(~obs_df['sd_g_red_mugal'].isna().values),
             all(~obs_df['corr_tide_red_mugal'].isna().values)])
         if not (flag_all_field_are_nan or flag_no_field_is_nan):
-            # raise AssertionError('In "obs_df" the columns "g_red_mugal", "sd_g_red_mugal" and "corr_tide_red_mugal" '
-            #                      'are not initialized consistently!'
             error_msg = 'In "obs_df" the columns "g_red_mugal", "sd_g_red_mugal" and "corr_tide_red_mugal" are not ' \
                         'initialized consistently! '
-            flag_corrections_applied = False
-            if verbose:
-                print(error_msg)
-            return flag_corrections_applied, error_msg
+            raise RuntimeError(f'Survey "{self.name}":' + error_msg)
+
 
         if verbose:
             print(f'## Calculate reduced observations by applying the specified corrections:')
 
         # 1.) Check reference heights:
         if verbose:
             print(
                 f'Reduction of reference heights to "{target_ref_height}" ({REFERENCE_HEIGHT_TYPE[target_ref_height]}):')
 
         if target_ref_height is None:  # Do nothing
             if verbose:
                 print(f' - Reference heights are not changed!')
-            flag_corrections_applied = True
         else:
             # Check if the target reference height type is valid:
             if target_ref_height not in REFERENCE_HEIGHT_TYPE:
                 raise ValueError(f'"{target_ref_height}" is an unknown reference height type.')
 
             # Check if reduction is necessary:
             if self.obs_reference_height_type == target_ref_height:
                 if verbose:
                     print(f' - Observations are already referenced to: {target_ref_height}')
-                flag_corrections_applied = True
             else:
                 # Check, if VG are available in obs_df:
                 if obs_df.vg_mugalm.isna().any():
                     error_msg = f'For the following stations the vertical gravity gradient is not available: ' \
                                 f'{", ".join(obs_df[obs_df.vg_mugalm.isna()].station_name.unique())}. ' \
                                 f'Without vertical gradient the observed gravity cannot be reduced to another height ' \
                                 f'level! '
-                    flag_corrections_applied = False
-                    if verbose:
-                        print(error_msg)
-                    return flag_corrections_applied, error_msg
+                    raise RuntimeError(f'Survey "{self.name}":' + error_msg)
 
                 # Reduction:
                 # Distance between instrument top and sensor level:
                 dst_m = GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m[self.gravimeter_type]
                 if self.obs_reference_height_type == 'sensor_height':
                     if target_ref_height == 'control_point':
                         # + dst_m + dhf_m
@@ -1128,122 +1193,181 @@
                     elif target_ref_height == 'sensor_height':
                         # - dhf_m - dst_m
                         g_red_mugal = g_red_mugal - (obs_df['dhf_m'] + dst_m) * \
                                       obs_df['vg_mugalm']
                         # sd_g_red_mugal = sd_g_red_mugal  # Keep SD
                 if verbose:
                     print('...done!')
-                flag_corrections_applied = True
 
         # 2.) Check tidal corrections:
+        # Check if the target tidal correction type is valid:
+        if target_tide_corr not in TIDE_CORRECTION_TYPES:
+            error_msg = f'"{target_tide_corr}" is unknown ab invalid!'
+            raise RuntimeError(f'Survey "{self.name}":' + error_msg)
+        tide_correction_description = TIDE_CORRECTION_TYPES[target_tide_corr]
         if verbose:
-            print(f'Tidal corrections "{target_tide_corr}" ({TIDE_CORRECTION_TYPES[target_tide_corr]}):')
-
+            print(f'Tidal corrections "{target_tide_corr}" ({tide_correction_description}):')
         if target_tide_corr is None:  # Do nothing
             if verbose:
                 print(f' - Tidal corrections are not changed!')
-            corr_tide_red_mugal = obs_df['corr_tide_mugal']
-            flag_corrections_applied = True
         else:
-            # Check if the target tidal correction type is valid:
-            if target_tide_corr not in TIDE_CORRECTION_TYPES:
-                # raise ValueError(f'"{target_tide_corr}" is unknown ab invalid!')
-                error_msg = f'"{target_tide_corr}" is unknown ab invalid!'
-                flag_corrections_applied = False
-                if verbose:
-                    print(error_msg)
-                return flag_corrections_applied, error_msg
-
-            # Check if reduction is necessary or possible:
-            if self.obs_tide_correction_type == target_tide_corr:
+            # Check if reduction is necessary and/or possible:
+            # - If time series data is used, corrections have to be calculated anyway, because the time series
+            #   may have changed since their last determination!
+            if (self.obs_tide_correction_type == target_tide_corr) & (target_tide_corr != 'from_time_series'):
                 if verbose:
                     print(f' - Observations are already reduced by: {target_tide_corr}')
                 corr_tide_red_mugal = obs_df['corr_tide_mugal']
-                flag_corrections_applied = True
-
             elif self.obs_tide_correction_type == 'unknown':
                 error_msg = 'Unknown tidal corrections at input data!'
-                flag_corrections_applied = False
-                if verbose:
-                    print(error_msg)
-                return flag_corrections_applied, error_msg
+                raise RuntimeError(f'Survey "{self.name}":' + error_msg)
             else:
-                # Reduction:
-                if self.obs_tide_correction_type == 'no_tide_corr':  # status of unreduced observations
-                    if target_tide_corr == 'cg5_longman1959':  # Add instrumental corrections
+                if self.obs_tide_correction_type == 'no_tide_corr':
+                    if target_tide_corr == 'cg5_longman1959':
                         g_red_mugal = g_red_mugal + obs_df['corr_tide_mugal']
-                        # sd_g_red_mugal = sd_g_red_mugal # Keep SD
+                        # TODO: Was steht in der Spalte "TIDE", wenn im CG5 KEINE Korrektur angebracht wurde?
+                        # - Wenn die richtige Korretkur NICHT vorliegt => raise Error!
                         corr_tide_red_mugal = obs_df['corr_tide_mugal']
                     elif target_tide_corr == 'longman1959':
-                        # Calculate corrections:
-                        tmp_df = self.obs_df[['obs_epoch', 'duration_sec', 'lon_deg', 'lat_deg', 'alt_m']].copy(
-                            deep=True)
-                        # Shift obs reference epoch from start to the middle of the gravity reading
-                        # (= evaluation time for the tide model):
-                        tmp_df['obs_epoch'] = tmp_df['obs_epoch'] + pd.to_timedelta(tmp_df['duration_sec'], 'sec') / 2
-                        # Remove TZ info for longman evaluation:
-                        tmp_df['obs_epoch'] = tmp_df['obs_epoch'].dt.tz_localize(None)
-                        tmp_df['tmp_index'] = tmp_df.index
-                        tmp_df = tmp_df.set_index('obs_epoch')
-                        tmp_df = gravtools.tides.longman1959.solve_tide_df(tmp_df, lat='lat_deg', lon='lon_deg',
-                                                                           alt='alt_m')
-                        tmp_df['longman_tide_corr_mugal'] = tmp_df['g0'] * 1e3  # Convert from mGal to µGal
-                        tmp_df = tmp_df.set_index('tmp_index')  # Restore numerical index
-                        # Apply correction:
-                        g_red_mugal = g_red_mugal - tmp_df['longman_tide_corr_mugal']
-                        # sd_g_red_mugal = sd_g_red_mugal # Keep SD
-                        corr_tide_red_mugal = tmp_df['longman_tide_corr_mugal']
-                    # elif target_tide_corr == '......':
+                        corr_tide_red_mugal = self.get_tidal_corrections_from_longman1959()
+                        g_red_mugal = g_red_mugal + corr_tide_red_mugal
+                    elif target_tide_corr == 'from_time_series':
+                        corr_tide_red_mugal = self.get_tidal_corrections_from_timeseries(
+                            correction_time_series=correction_time_series,
+                            interpolation_method=tide_corr_timeseries_interpol_method)
+                        g_red_mugal = g_red_mugal + corr_tide_red_mugal
+                        tide_corr_timeseries_interpol_method_out = tide_corr_timeseries_interpol_method
+
                 elif self.obs_tide_correction_type == 'cg5_longman1959':
-                    if target_tide_corr == 'no_tide_corr':  # Subtract instrumental corrections
-                        g_red_mugal = g_red_mugal - obs_df['corr_tide_mugal']
-                        # sd_g_red_mugal = sd_g_red_mugal # Keep SD
-                        corr_tide_red_mugal = obs_df['corr_tide_mugal']
+                    g_red_mugal = g_red_mugal - obs_df['corr_tide_mugal']  # Undo instrumental corrections => No tide corr!
+                    if target_tide_corr == 'no_tide_corr':
+                        corr_tide_red_mugal = obs_df['corr_tide_mugal'].copy(deep=True)
                         corr_tide_red_mugal.values[:] = 0
                     elif target_tide_corr == 'longman1959':
-                        # Calculate corrections:
-                        tmp_df = self.obs_df[['obs_epoch', 'duration_sec', 'lon_deg', 'lat_deg', 'alt_m']].copy(
-                            deep=True)
-                        # Shift obs reference epoch from start to the middle of the gravity reading
-                        # (= evaluation time for the tide model):
-                        tmp_df['obs_epoch'] = tmp_df['obs_epoch'] + pd.to_timedelta(tmp_df['duration_sec'], 'sec') / 2
-                        # Remove TZ info for longman evaluation:
-                        tmp_df['obs_epoch'] = tmp_df['obs_epoch'].dt.tz_localize(None)
-                        tmp_df['tmp_index'] = tmp_df.index
-                        tmp_df = tmp_df.set_index('obs_epoch')
-                        tmp_df = gravtools.tides.longman1959.solve_tide_df(tmp_df, lat='lat_deg', lon='lon_deg', alt='alt_m')
-                        tmp_df['longman_tide_corr_mugal'] = tmp_df['g0']*1e3  # Convert from mGal to µGal
-                        tmp_df = tmp_df.set_index('tmp_index')  # Restore numerical index
-                        # Apply correction:
-                        g_red_mugal = g_red_mugal - tmp_df['longman_tide_corr_mugal']
-                        # sd_g_red_mugal = sd_g_red_mugal # Keep SD
-                        corr_tide_red_mugal = tmp_df['longman_tide_corr_mugal']
-                    # elif target_tide_corr == '......':
+                        corr_tide_red_mugal = self.get_tidal_corrections_from_longman1959()
+                        g_red_mugal = g_red_mugal + corr_tide_red_mugal
+                    elif target_tide_corr == 'from_time_series':
+                        corr_tide_red_mugal = self.get_tidal_corrections_from_timeseries(
+                            correction_time_series=correction_time_series,
+                            interpolation_method=tide_corr_timeseries_interpol_method)
+                        g_red_mugal = g_red_mugal + corr_tide_red_mugal
+                        tide_corr_timeseries_interpol_method_out = tide_corr_timeseries_interpol_method
+
                 elif self.obs_tide_correction_type == 'longman1959':
-                    if target_tide_corr == 'no_tide_corr':  # Subtract instrumental corrections
-                        g_red_mugal = g_red_mugal - obs_df['corr_tide_mugal']
-                        # sd_g_red_mugal = sd_g_red_mugal # Keep SD
-                        corr_tide_red_mugal = obs_df['corr_tide_mugal']
+                    # This should never be the case!
+                    g_red_mugal = g_red_mugal - obs_df[
+                        'corr_tide_red_mugal']  # Undo corrections => No tide corr!
+                    if target_tide_corr == 'no_tide_corr':
+                        corr_tide_red_mugal = obs_df['corr_tide_mugal'].copy(deep=True)
                         corr_tide_red_mugal.values[:] = 0
-                    elif target_tide_corr == 'cg5_longman1959':  # Add instrumental corrections
+                    elif target_tide_corr == 'cg5_longman1959':
                         g_red_mugal = g_red_mugal + obs_df['corr_tide_mugal']
-                        # sd_g_red_mugal = sd_g_red_mugal # Keep SD
                         corr_tide_red_mugal = obs_df['corr_tide_mugal']
+                    elif target_tide_corr == 'from_time_series':
+                        corr_tide_red_mugal = self.get_tidal_corrections_from_timeseries(correction_time_series=correction_time_series,
+                                                                                         interpolation_method=tide_corr_timeseries_interpol_method)
+                        g_red_mugal = g_red_mugal + corr_tide_red_mugal
+                        tide_corr_timeseries_interpol_method_out = tide_corr_timeseries_interpol_method
+                else:
+                    raise RuntimeError(f'Tidal corrections of observation data ("{self.obs_tide_correction_type}") not '
+                                       f'supported!')
                 if verbose:
                     print('...done!')
-                flag_corrections_applied = True
 
-        # Apply changes, if everything worked out in here:
-        if flag_corrections_applied:
+            # Apply changes, if no exceptions were raised:
             self.red_tide_correction_type = target_tide_corr
             self.red_reference_height_type = target_ref_height
+            self.red_tide_correction_description = tide_correction_description
+            self.red_tide_corr_timeseries_interpol_method = tide_corr_timeseries_interpol_method_out
             self.obs_df['g_red_mugal'] = g_red_mugal
             self.obs_df['sd_g_red_mugal'] = sd_g_red_mugal
             self.obs_df['corr_tide_red_mugal'] = corr_tide_red_mugal
-        return flag_corrections_applied, error_msg
+
+    def get_tidal_corrections_from_timeseries(self, correction_time_series, interpolation_method : str) -> np.ndarray  :
+        """Derives tidal corrections for observations from time series data.
+
+        Notes
+        -----
+        The derived corrections have to be ADDED to the observations in order to reduce tidal effects!
+
+        Parameters
+        ----------
+        correction_time_series : `CorrectionTimeSeries` object, optional (default=None)
+            Correction time series object that contains time series of tidal corrections for stations in surveys. This
+            argument is required, if tidal corrections should be derived from time series data, i.e. if
+            `self.target_tide_corr = from_time_series`.
+        interpolation_method : str, optional (default='')
+            Interpolation method used to calculate tidal corrections from time series data. If tidal corrections are
+            obtained from other sources or models, this attribute is irrelevant and has to be empty!
+
+        Returns
+        -------
+        `pandas.Series`: Interpolated value for the given interpolation times.
+        """
+        # Check, if time series data is available for all stations in the survey:
+        # - Survey:
+        if self.name not in correction_time_series.surveys:
+            raise RuntimeError(f'No correction time series data available for survey "{self.name}".')
+        # - Stations in Survey:
+        missing_stations = list(set(correction_time_series.surveys[self.name].station_names) - set(self.observed_stations))
+        if len(missing_stations) > 0:
+            raise RuntimeError(f'No correction time series data available for the stations: ' + ', '.join(missing_stations))
+
+        # Prep input obervation dataframe: Keep required columns only:
+        tmp_df = self.obs_df[['station_name', 'obs_epoch', 'duration_sec']].copy(deep=True)
+        # Shift obs reference epoch from start to the middle of the gravity reading
+        # (= evaluation time for the tide model):
+        tmp_df['obs_epoch'] = tmp_df['obs_epoch'] + pd.to_timedelta(tmp_df['duration_sec'], 'sec') / 2
+        tmp_df.drop(columns=['duration_sec'], inplace=True)
+        tmp_df['ts_tide_corr_mugal'] = np.nan
+
+        # Loop over stations, interpolate corrections and add them to tmp_df:
+        # - Check temporal data availability (scipy.interpolate.interp1 raises an error anyway)
+        # - consider interpolation_method
+        # - consider the model type (correction or effect)
+        # - consider the units => µGal
+        for station in self.observed_stations:
+            tmp_filter = tmp_df['station_name'] == station
+            obs_epochs_dt64 = tmp_df.loc[tmp_filter, 'obs_epoch'].to_numpy()
+            interp = correction_time_series.surveys[self.name].stations[station].tidal_correction.interpolate(interp_times=obs_epochs_dt64,
+                                                                                                              kind=interpolation_method,
+                                                                                                              return_correction=True)
+            interp_mugal = convert_to_mugal(interp,
+                                      correction_time_series.surveys[self.name].stations[station].tidal_correction.unit)
+            tmp_df.loc[tmp_filter, 'ts_tide_corr_mugal'] = interp_mugal
+        tide_corr_timeseries_mugal = tmp_df['ts_tide_corr_mugal'].to_numpy()
+        return tide_corr_timeseries_mugal
+
+    def get_tidal_corrections_from_longman1959(self) -> np.ndarray  :
+        """Derives tidal corrections for observations from the Longman (1959) model.
+
+        Notes
+        -----
+        The derived corrections have to be ADDED to the observations in order to reduce tidal effects!
+
+        Parameters
+        ----------
+
+        Returns
+        -------
+        `pandas.Series`: Tidal corrections.
+        """
+        tmp_df = self.obs_df[['obs_epoch', 'duration_sec', 'lon_deg', 'lat_deg', 'alt_m']].copy(
+            deep=True)
+        # Shift obs reference epoch from start to the middle of the gravity reading
+        # (= evaluation time for the tide model):
+        tmp_df['obs_epoch'] = tmp_df['obs_epoch'] + pd.to_timedelta(tmp_df['duration_sec'], 'sec') / 2
+        # Remove TZ info for longman evaluation:
+        tmp_df['obs_epoch'] = tmp_df['obs_epoch'].dt.tz_localize(None)
+        tmp_df['tmp_index'] = tmp_df.index
+        tmp_df = tmp_df.set_index('obs_epoch')
+        tmp_df = gravtools.tides.longman1959.solve_tide_df(tmp_df, lat='lat_deg', lon='lon_deg', alt='alt_m')
+        tmp_df['longman_tide_corr_mugal'] = tmp_df['g0'] * 1e3  # Convert from mGal to µGal
+        tmp_df = tmp_df.set_index('tmp_index')  # Restore numerical index
+        return tmp_df['longman_tide_corr_mugal']
 
     def autselect_tilt(self, threshold_arcsec: int, setup_id: int = None, verbose: bool = False):
         """Deactivate all observations of the survey or of a setup with a tilt larger than the defined threshold.
 
         Parameters
         ----------
         threshold_arcsec : int
@@ -1426,32 +1550,50 @@
                 print('Nothing to delete. Setup data is empty.')
         else:
             if verbose:
                 print('Setup data deleted.')
             self.setup_df = None
             self.setup_reference_height_type = ''
             self.setup_tide_correction_type = ''
+            self.setup_calc_method = ''
             self.setup_obs_list_df = None
 
     def calculate_setup_data(self, obs_type='reduced',
                              ref_delta_t_campaign_dt=None,
                              active_obs_only_for_ref_epoch=True,
+                             method='variance_weighted_mean',
+                             method_sd='sd_from_obs_file',
+                             default_sd_mugal=100.0,
                              verbose=False):
         """Accumulate all active observation within each setup and calculate a single representative pseudo observation.
 
         Parameters
         ----------
         obs_type : str, 'observed' or 'reduced' (default)
             Defines whether the observed (as loaded from an observation file) or the reduced observations from
             `self.obs_df` are used to determine the weighted mean values per setup.
         ref_delta_t_campaign_dt : datetime object, optional (default = None)
             Reference time for calculation of `delta_t_campaign_h`. `None` implies that the reference epoch is not
             available/defined. In the latter case `delta_t_campaign_h` is `None` for all setup observations.
         active_obs_only_for_ref_epoch: bool, optional (default=True)
             `True` implies that the relative reference epochs are determined by considering active observations only.
+        method : str, optional (default=`variance_weighted_mean`)
+            Select method for the calculation of setup data. `variance_weighted_mean` implies that setup observations
+            (observed gravity, standard deviations and reference time) are calculated by variance weighted mean of the
+            individual observations. `individual_obs` implies that the original observations are used as setup data
+            without any aggregation.
+        method_sd : str, optional (default='sd_from_obs_file')
+            Method for the determination of standard deviations (SD) of setup observations. `sd_from_obs_file` implies that
+            SD are taken from the observation file. `sd_default_per_obs` and `sd_default_per_setup` imply that the
+            given default SD is used, where the default SD is applied the individual observations in the first case and
+            to setups in the second case. If applied to observations, the number of observations per setup still plays a
+            role for weighting the setup observations in the adjustment.
+        default_sd_mugal : float, optional (default=100.0)
+            Default standard deviation [µGal] that is used to determine the SD of setup observations when `method_sd` is
+            `sd_default_per_obs` or `sd_default_per_setup`
         verbose : bool, optional (default=False)
             If `True`, status messages are printed to the command line.
         """
 
         if verbose:
             print(f'Calculate setup data for survey {self.name}')
 
@@ -1459,21 +1601,33 @@
         flag_calculate_delta_t_campaign_h = False
 
         self.reset_setup_data(verbose)
 
         # Initial checks:
         if obs_type not in _VALID_OBS_TYPES:
             raise AssertionError(f'Invalid observation type: {obs_type} (valid: "reduced" or "observed").')
+        if method not in SETUP_CALC_METHODS:
+            raise AssertionError(f'Invalid method: {method} (valid: "variance_weighted_mean" or "individual_obs").')
         if self.obs_df is None:
             raise AssertionError('Observation dataframe is empty!')
 
         # Get all active observations:
         tmp_filter = self.obs_df['keep_obs']
         active_obs_df = self.obs_df[tmp_filter].copy(deep=True)
 
+        # Modify SD according to input options:
+        if method_sd == 'sd_from_obs_file':
+            pass  # keep SD
+        elif method_sd == 'sd_default_per_obs':
+            if verbose:
+                print(f'Use default SD of {default_sd_mugal} µGal for weighting observations instead of SD from '
+                      f'observation files.')
+            active_obs_df['sd_g_red_mugal'] = default_sd_mugal
+            active_obs_df['sd_g_obs_mugal'] = default_sd_mugal
+
         # Check, if at least one observation is active:
         if len(active_obs_df) == 0:
             # raise AssertionError(f'No active observations in survey {self.name}')
             if verbose:
                 print(f'No active observations in survey {self.name}')
         else:
 
@@ -1489,99 +1643,129 @@
                 flag_calculate_delta_t_campaign_h = True
             else:
                 raise TypeError('`ref_delta_t_campaign_dt` needs to be a datetime object!')
             # - SD == 0? => This would create a divided by zero error!
             if obs_type == 'reduced':
                 tmp_filter = active_obs_df['sd_g_red_mugal'] <= 0.0
             elif obs_type == 'observed':
-                tmp_filter = active_obs_df['sd_g_red_mugal'] <= 0.0
+                tmp_filter = active_obs_df['sd_g_obs_mugal'] <= 0.0
             if tmp_filter.any():
                 error_str = active_obs_df.loc[tmp_filter, ['station_name', 'obs_epoch']].to_string()
                 raise AssertionError(f'The SD of the following observations ({obs_type}) in the survey {self.name}'
                                      f' is <= 0.0 µGal (invalid!):\n{error_str}')
 
             # Determine reference time for the survey:
             if active_obs_only_for_ref_epoch:
                 ref_delta_t_dt = active_obs_df['obs_epoch'].min()  # First observation epoch in survey (active only)
             else:
                 ref_delta_t_dt = self.obs_df['obs_epoch'].min()  # First observation epoch (also inactive obs)
 
-            # Initialize columns lists for creating dataframe:
-            station_name_list = []
-            setup_id_list = []
-            g_mugal_list = []
-            sd_g_red_mugal_list = []
-            obs_epoch_list_unix = []
-            obs_epoch_list_dt = []
-            delta_t_h_list = []
-            delta_t_campaign_h_list = []
-            sd_setup_mugal_list = []
-            number_obs_list = []
-            dhf_sensor_m_list = []
-
             # Loop over setups:
-            setup_ids = active_obs_df['setup_id'].unique()
-            for setup_id in setup_ids:
-                tmp_filter = active_obs_df['setup_id'] == setup_id
+            if method == 'variance_weighted_mean':
+                # Initialize columns lists for creating dataframe:
+                station_name_list = []
+                setup_id_list = []
+                g_mugal_list = []
+                sd_g_red_mugal_list = []
+                obs_epoch_list_unix = []
+                obs_epoch_list_dt = []
+                delta_t_h_list = []
+                delta_t_campaign_h_list = []
+                sd_setup_mugal_list = []
+                number_obs_list = []
+                dhf_sensor_m_list = []
+
+                setup_ids = active_obs_df['setup_id'].unique()
+                for setup_id in setup_ids:
+                    tmp_filter = active_obs_df['setup_id'] == setup_id
+                    if obs_type == 'observed':
+                        g_mugal = active_obs_df.loc[tmp_filter, 'g_obs_mugal'].to_numpy()
+                        sd_g_mugal = active_obs_df.loc[tmp_filter, 'sd_g_obs_mugal'].to_numpy()
+                    elif obs_type == 'reduced':
+                        g_mugal = active_obs_df.loc[tmp_filter, 'g_red_mugal'].to_numpy()
+                        sd_g_mugal = active_obs_df.loc[tmp_filter, 'sd_g_red_mugal'].to_numpy()
+                    weights = 1 / sd_g_mugal ** 2
+                    g_setup_mugal = np.sum(g_mugal * weights) / np.sum(weights)
+                    sd_g_setup_mugal = np.sqrt(1 / np.sum(weights))
+                    if len(active_obs_df.loc[tmp_filter, 'station_name'].unique()) > 1:
+                        raise AssertionError(
+                            f'Setup with ID "{setup_id}" in survey "{self.name}" contains '
+                            f'{len(active_obs_df.loc[tmp_filter, "station_name"].unique())} stations (only 1 allowed)!'
+                        )
+
+                    # Standard deviation of active observations within setup:
+                    # - If less than 2 active observations in setup => Calculation not possible => NaN
+                    if len(g_mugal) >= 2:
+                        sd_setup_mugal_list.append(g_mugal.std(ddof=1))  # degree of freedom = (len(g_mugal) - 1)
+                    else:
+                        sd_setup_mugal_list.append(np.nan)
+
+                    number_obs_list.append(len(g_mugal))  # Number of observations
+
+                    # Get vertical distance between sensor height and control point:
+                    dhf_sensor_m_list.append(active_obs_df.loc[tmp_filter, 'dhf_m'].values[0] + GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m[self.gravimeter_type])
+
+                    # observation epoch (UNIX timestamps in full seconds):
+                    obs_epochs_series = active_obs_df.loc[tmp_filter, 'obs_epoch']
+                    unix_obs_epochs = obs_epochs_series.values.astype(np.int64) / 10 ** 9
+                    unix_setup_epoch = np.sum(unix_obs_epochs * weights) / np.sum(weights)
+
+                    # Reference epoch as datetime object (TZ=<UTC>):
+                    dt_setup_epoch = dt.datetime.utcfromtimestamp(unix_setup_epoch)
+                    dt_setup_epoch = dt_setup_epoch.replace(tzinfo=dt.timezone.utc)  # TZ = <UTC>
+
+                    station_name_list.append(active_obs_df.loc[tmp_filter, 'station_name'].unique()[0])
+                    setup_id_list.append(setup_id)
+                    g_mugal_list.append(g_setup_mugal)
+                    sd_g_red_mugal_list.append(sd_g_setup_mugal)
+                    obs_epoch_list_unix.append(unix_setup_epoch)
+                    obs_epoch_list_dt.append(dt_setup_epoch)
+                    delta_t_h_list.append((unix_setup_epoch - (ref_delta_t_dt.value / 10 ** 9)) / 3600.0)
+                    if flag_calculate_delta_t_campaign_h:
+                        delta_t_campaign_h_list.append((unix_setup_epoch - (ref_delta_t_campaign_dt.value / 10 ** 9)) / 3600.0)
+                    else:
+                        delta_t_campaign_h_list.append(None)
+            elif method == 'individual_obs':
+                station_name_list = active_obs_df['station_name'].to_list()
+                setup_id_list = active_obs_df['setup_id'].to_list()
                 if obs_type == 'observed':
-                    g_mugal = active_obs_df.loc[tmp_filter, 'g_obs_mugal'].to_numpy()
-                    sd_g_mugal = active_obs_df.loc[tmp_filter, 'sd_g_obs_mugal'].to_numpy()
+                    g_mugal_list = active_obs_df['g_obs_mugal'].to_list()
+                    sd_g_red_mugal_list = active_obs_df['sd_g_obs_mugal'].to_list()
                 elif obs_type == 'reduced':
-                    g_mugal = active_obs_df.loc[tmp_filter, 'g_red_mugal'].to_numpy()
-                    sd_g_mugal = active_obs_df.loc[tmp_filter, 'sd_g_red_mugal'].to_numpy()
-                weights = 1 / sd_g_mugal ** 2
-                g_setup_mugal = np.sum(g_mugal * weights) / np.sum(weights)
-                sd_g_setup_mugal = np.sqrt(1 / np.sum(weights))
-                if len(active_obs_df.loc[tmp_filter, 'station_name'].unique()) > 1:
-                    raise AssertionError(
-                        f'Setup with ID "{setup_id}" in survey "{self.name}" contains '
-                        f'{len(active_obs_df.loc[tmp_filter, "station_name"].unique())} stations (only 1 allowed)!'
-                    )
-
-                # Standard deviation of active observations within setup:
-                # - If less than 2 active observations in setup => Calculation not possible => NaN
-                if len(g_mugal) >= 2:
-                    sd_setup_mugal_list.append(g_mugal.std(ddof=1))  # degree of freedom = (len(g_mugal) - 1)
-                else:
-                    sd_setup_mugal_list.append(np.nan)
-
-                number_obs_list.append(len(g_mugal))  # Number of observations
+                    g_mugal_list = active_obs_df['g_red_mugal'].to_list()
+                    sd_g_red_mugal_list = active_obs_df['sd_g_red_mugal'].to_list()
 
-                # Get vertical distance between sensor height and control point:
-                dhf_sensor_m_list.append(active_obs_df.loc[tmp_filter, 'dhf_m'].values[0] + GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m[self.gravimeter_type])
+                obs_epoch_unix_array = active_obs_df['obs_epoch'].values.astype(np.int64) / 10 ** 9
+                obs_epoch_list_unix = list(obs_epoch_unix_array)
+                obs_epoch_list_dt = pd.to_datetime(obs_epoch_unix_array, unit='s').tz_localize('utc').to_list()
 
-                # observation epoch (UNIX timestamps in full seconds):
-                obs_epochs_series = active_obs_df.loc[tmp_filter, 'obs_epoch']
-                unix_obs_epochs = obs_epochs_series.values.astype(np.int64) / 10 ** 9
-                unix_setup_epoch = np.sum(unix_obs_epochs * weights) / np.sum(weights)
-
-                # Reference epoch as datetime object (TZ=<UTC>):
-                dt_setup_epoch = dt.datetime.utcfromtimestamp(unix_setup_epoch)
-                dt_setup_epoch = dt_setup_epoch.replace(tzinfo=dt.timezone.utc)  # TZ = <UTC>
-
-                station_name_list.append(active_obs_df.loc[tmp_filter, 'station_name'].unique()[0])
-                setup_id_list.append(setup_id)
-                g_mugal_list.append(g_setup_mugal)
-                sd_g_red_mugal_list.append(sd_g_setup_mugal)
-                obs_epoch_list_unix.append(unix_setup_epoch)
-                obs_epoch_list_dt.append(dt_setup_epoch)
-                delta_t_h_list.append((unix_setup_epoch - (ref_delta_t_dt.value / 10 ** 9)) / 3600.0)
+                delta_t_h_list = list((obs_epoch_unix_array - (ref_delta_t_dt.value / 10 ** 9)) / 3600.0)
                 if flag_calculate_delta_t_campaign_h:
-                    delta_t_campaign_h_list.append((unix_setup_epoch - (ref_delta_t_campaign_dt.value / 10 ** 9)) / 3600.0)
+                    delta_t_campaign_h_list = list((obs_epoch_unix_array - (ref_delta_t_campaign_dt.value / 10 ** 9)) / 3600.0)
                 else:
-                    delta_t_campaign_h_list.append(None)
+                    delta_t_campaign_h_list = [None] * len(g_mugal_list)
+                sd_setup_mugal_list = [np.nan] * len(g_mugal_list)
+                number_obs_list = [1] * len(g_mugal_list)
+                dhf_sensor_m_list = active_obs_df['dhf_m'] + GRAVIMETER_REFERENCE_HEIGHT_CORRECTIONS_m[self.gravimeter_type]
 
             if obs_type == 'observed':
                 self.setup_tide_correction_type = self.obs_tide_correction_type
                 self.setup_reference_height_type = self.obs_reference_height_type
             elif obs_type == 'reduced':
                 self.setup_tide_correction_type = self.red_tide_correction_type
                 self.setup_reference_height_type = self.red_reference_height_type
+            self.setup_calc_method = method
+            self.setup_sd_method = method_sd
             self.create_setup_obs_list()
 
+            if method_sd == 'sd_default_per_setup':
+                if verbose:
+                    print(f'Use a default SD of {default_sd_mugal} µGal for all setup observations.')
+                sd_g_red_mugal_list = [default_sd_mugal for item in sd_g_red_mugal_list]
+
             # convert to pd dataframe:
             self.setup_df = pd.DataFrame(list(zip(station_name_list,
                                                   setup_id_list,
                                                   g_mugal_list,
                                                   sd_g_red_mugal_list,
                                                   obs_epoch_list_unix,
                                                   obs_epoch_list_dt,
@@ -1592,15 +1776,15 @@
                                                   dhf_sensor_m_list)),
                                          columns=self._SETUP_DF_COLUMNS)
             self.set_reference_time(ref_delta_t_dt)  # Save reference time for `delta_t_h`, i.e. for the survey.
 
     def create_setup_obs_list(self):
         """Create list of all observations that contribute to the calculation of setup data in this Survey object.
 
-        The list is created as pabdas dataframe. It holds information whether an observation in the `obs_df` is
+        The list is created as pandas dataframe. It holds information whether an observation in the `obs_df` is
         active or inactive (`keep_obs` flag).
         """
         self.setup_obs_list_df = self.obs_df.loc[:, self._SETUP_OBS_LIST_DF_COLUMNS].copy(deep=True)
 
     @property
     def number_of_setups(self):
         """Returns the number of setups in the survey"""
@@ -1658,15 +1842,18 @@
             return ''
 
     @property
     def duration_hhmmss_str(self):
         """Returns the timespan (Timedalta) between first and last observation in the survey in hh:mm:ss format."""
         if self.obs_df is not None:
             duration = self.obs_df['obs_epoch'].max() - self.obs_df['obs_epoch'].min()
-            return format_seconds_to_hhmmss(duration.seconds)
+            if duration.days == 0:
+                return format_seconds_to_hhmmss(duration.seconds)
+            else:
+                return f'{duration.days}d ' + format_seconds_to_hhmmss(duration.seconds)
         else:
             return ''
 
     @property
     def is_active(self):
         """`True` indicates that the survey contains at least one active observation."""
         if self.obs_df is not None:
```

### Comparing `grav-toolbox-0.1.9/gravtools/models/vg_lsm.py` & `grav-toolbox-0.2.0/gravtools/models/vg_lsm.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,16 +264,17 @@
         # Total number of parameters to be estimated:
         # - Drift polynomial coeff.: Polynomial degree * number of surveys
         # - 1 constant instrumental bias per survey
         # - VG polynomial coeff.: Polynomial degree * number of surveys
         number_of_parameters = drift_pol_degree + vg_polynomial_degree + 1
 
         # Check, if setup IDs are unique:
-        if len(set(setup_ids)) != len(setup_ids):
-            raise AssertionError('Setup IDs are not unique within the campaign!')
+        if self.check_for_unique_setup_id:
+            if len(set(setup_ids)) != len(setup_ids):
+                raise AssertionError('Setup IDs are not unique within the campaign!')
 
         if verbose or self.write_log:
             time_now_str = dt.datetime.now(tz=pytz.UTC).strftime('%Y-%m-%d, %H:%M:%S %Z')
             tmp_str = f'#### Adjustment log (VG LGM estimation based on non-differential observations) ####\n'
             tmp_str += f'Processed with GravTools {GRAVTOOLS_VERSION} ({time_now_str})\n'
             tmp_str += f'Comment: {self.comment}\n'
             tmp_str += f'\n'
```

### Comparing `grav-toolbox-0.1.9/gravtools/scripts/__init__.py` & `grav-toolbox-0.2.0/gravtools/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/scripts/run_gui.py` & `grav-toolbox-0.2.0/gravtools/scripts/run_gui.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/settings.py` & `grav-toolbox-0.2.0/gravtools/settings.py`

 * *Files 23% similar despite different names*

```diff
@@ -30,17 +30,41 @@
     'obs_file': 'From an observation file',
 }
 
 TIDE_CORRECTION_TYPES = {
     'cg5_longman1959': 'Instrument-implemented tidal correction of the Scintrex CG-5',
     'longman1959': 'Tidal corrections by the model of Longman (1959)',
     'no_tide_corr': 'No tide correction applied',
+    'from_time_series': 'Interpolated from correction time series',
     'unknown': 'Unknown whether a tide correction was applied',
 }
 
+# Conversion factors of different units of gravity to µGal:
+# - Keys: Units as used e.g. in TSF files by Tsoft
+# - Values: Multiplicative conversion factors to µGal
+UNIT_CONVERSION_TO_MUGAL = {
+    'nm/s^2': 1e-1  # 1 nm/s^2 * 0.1 = 1 µGal
+}
+
+# Interpolation methods provided by scipy.interpolation.interp1, e.g. used for the interpolation of correction time
+# series data.
+SCIPY_INTERP1_INTERPOLATION_METHODS = {
+    'linear': 'Linear interpolation.',
+    'nearest': '"Snaps" to the nearest data point. Rounds down at half-integers (e.g. 0.5, 1.5)',
+    'nearest-up': '"Snaps" to the nearest data point. Rounds up at half-integers (e.g. 0.5, 1.5)',
+    'zero': 'Zero order spline. It`s value at any point is the last raw value seen.',
+    'slinear': 'First order spline interpolation (similar to "linear").',
+    'quadratic': 'Second order spline interpolation.',
+    'cubic': 'Third order spline interpolation.',
+    'previous': 'Return previous value.',
+    'next': 'Return next value.',
+}
+# Default interpolation method:
+SCIPY_INTERP1_INTERPOLATION_DEFAULT_METHOD = 'quadratic'
+
 REFERENCE_HEIGHT_TYPE = {
     'sensor_height': 'The gravity values refer to the sensor height',
     'instrument_top': 'The gravity values refers to the instrument top',
     'ground': 'The gravity values refers to the ground point of the station',
     'control_point': 'The gravity values refers to the control point of the station',
 }
 
@@ -79,14 +103,27 @@
 
 #  Lookup table for matching gravimeter IDs and the tidal corrections that are applied per default in the BEV legacy
 #  observation files:
 BEV_GRAVIMETER_TIDE_CORR_LOOKUP = {
     '5': 'cg5_longman1959'
 }
 
+# Methods for calculation of setup observations:
+SETUP_CALC_METHODS = {
+    'variance_weighted_mean': 'Variance weighted mean of observations within a setup.',
+    'individual_obs': 'Each observation is treated as setup.'
+}
+
+# Methods for calculation of standard deviations (SD) of setup observations:
+SETUP_SD_METHODS = {
+    'sd_from_obs_file': 'Apply the standard deviations from observation files.',
+    'sd_default_per_obs': 'Apply the default standard deviation to all individual observations.',
+    'sd_default_per_setup': 'Apply the default standard deviation to setup obsertvations.'
+}
+
 # Available adjustment methods:
 ADJUSTMENT_METHODS = {
     'LSM_diff': 'LSM (differential observations)',  # Least-squares adjustment of differential observations
     'LSM_non_diff': 'LSM (non-differential observations)',  # Least-squares adjustment of non-differential observations
     'MLR_BEV': 'MLR (BEV legacy processing)',  # Least-squares adjustment of differential observations
     'VG_LSM_nondiff': 'VG LSM (non-differential observations)',  # Vertical Gravity Gradient estimation based on Least-squares adjustment of non-differential observations
 }
@@ -127,14 +164,26 @@
 # GUI and Program options:
 CALCULATE_REDUCED_OBS_WHEN_LOADING_DATA = True  # Calculate reduced observations when loading observation data.
 INIT_OESGN_STATION_AS_DATUM = False  # Initialize OESGN stations as datum stations when loading rom an OESGN file?
 
 
 # ----- GUI appearance and plot settings -----
 
+# Methods for the determination of histogram bin edges:
+NUMPY_HISTOGRAM_BIN_EDGES_OPTIONS = {
+    'auto': 'Maximum of the ‘sturges’ and ‘fd’ estimators. Provides good all around performance.',
+    'fd': 'Freedman Diaconis Estimator: Robust (resilient to outliers) estimator that takes into account data variability and data size.',
+    'doane': 'An improved version of Sturges’ estimator that works better with non-normal datasets.',
+    'scott': 'Estimator based on leave-one-out cross-validation estimate of the integrated squared error. Can be regarded as a generalization of Scott’s rule.',
+    'rice': 'Estimator does not take variability into account, only data size. Commonly overestimates number of bins required.',
+    'sturges': 'R’s default method, only accounts for data size. Only optimal for gaussian data and underestimates number of bins for large non-gaussian datasets.',
+    'sqrt': 'Square root (of data size) estimator, used by Excel and other programs for its speed and simplicity.',
+    'Num. of bins': 'User defined number of bins (min. = 2, max. = 1000).'
+}
+
 # --- Gerneral color settings ---
 DATUM_STATION_COLOR = (255, 204, 204)
 
 # --- Drift plots in the results tab: ---
 # Number of plot items for plotting the drift function (polynomial):
 DRIFT_PLOT_NUM_ITEMS_IN_DRIFT_FUNCTION = 100
 # Options for the observation data points in the drift plot:
@@ -231,19 +280,12 @@
 
 # ÖSGN Table:
 PATH_OESGN_TABLE = '/home/heller/pyProjects/GravTools/data/'
 NAME_OESGN_TABLE = 'OESGN.TAB'
 
 # BEV observation files:
 PATH_OBS_FILE_BEV = '/home/heller/pyProjects/GravTools/data/BEV/'
-# NAME_OBS_FILE_BEV = '20200527_tideCorr'
-# NAME_OBS_FILE_BEV = '20200527_sd'
-# NAME_OBS_FILE_BEV = '20200527_2'
-# NAME_OBS_FILE_BEV = '20200527'
-# NAME_OBS_FILE_BEV = 'n20200701_1'
 NAME_OBS_FILE_BEV = 'f200701_1'
-# NAME_OBS_FILE_BEV = 'e201001'
 
 # CG-5 observation files (text)
 PATH_OBS_FILE_CG5 = '/home/heller/pyProjects/GravTools/data/CG5/'
-# NAME_OBS_FILE_CG5 = '2020-06-18_DACH.TXT'
 NAME_OBS_FILE_CG5 = '20200907_test.TXT'
```

### Comparing `grav-toolbox-0.1.9/gravtools/tides/__init__.py` & `grav-toolbox-0.2.0/gravtools/tides/__init__.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/gravtools/tides/longman1959.py` & `grav-toolbox-0.2.0/gravtools/tides/longman1959.py`

 * *Files identical despite different names*

### Comparing `grav-toolbox-0.1.9/setup.cfg` & `grav-toolbox-0.2.0/setup.cfg`

 * *Files identical despite different names*

