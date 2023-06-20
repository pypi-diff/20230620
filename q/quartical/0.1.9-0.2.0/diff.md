# Comparing `tmp/quartical-0.1.9.tar.gz` & `tmp/quartical-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quartical-0.1.9.tar", last modified: Thu Nov 24 10:13:17 2022, max compression
+gzip compressed data, was "quartical-0.2.0.tar", max compression
```

## Comparing `quartical-0.1.9.tar` & `quartical-0.2.0.tar`

### file list

```diff
@@ -1,118 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.096158 quartical-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (122)     1078 2022-11-24 10:13:16.000000 quartical-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       41 2022-11-24 10:13:16.000000 quartical-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2022-11-24 10:13:17.096158 quartical-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      674 2022-11-24 10:13:16.000000 quartical-0.1.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/
--rw-r--r--   0 runner    (1001) docker     (122)       24 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/apps/backup.py
--rw-r--r--   0 runner    (1001) docker     (122)    10511 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/apps/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/calibration/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11975 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)    10814 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/constructor.py
--rw-r--r--   0 runner    (1001) docker     (122)     7043 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/mapping.py
--rw-r--r--   0 runner    (1001) docker     (122)     5932 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/calibration/solver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical/config/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2206 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)     8808 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/external.py
--rw-r--r--   0 runner    (1001) docker     (122)     4407 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/helper.py
--rw-r--r--   0 runner    (1001) docker     (122)    12372 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/helpstrings.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     1797 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/internal.py
--rw-r--r--   0 runner    (1001) docker     (122)     4410 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/parser.py
--rw-r--r--   0 runner    (1001) docker     (122)     3275 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/config/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/data_handling/
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11452 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/angles.py
--rw-r--r--   0 runner    (1001) docker     (122)     9049 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/bda.py
--rw-r--r--   0 runner    (1001) docker     (122)     8269 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/chunking.py
--rw-r--r--   0 runner    (1001) docker     (122)     6021 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    16419 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/ms_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)    17299 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      411 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/selection.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/data_handling/wisdom.py
--rw-r--r--   0 runner    (1001) docker     (122)     7000 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/flagging/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/flagging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8950 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/flagging/flagging.py
--rw-r--r--   0 runner    (1001) docker     (122)     4157 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/flagging/flagging_kernels.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/
--rw-r--r--   0 runner    (1001) docker     (122)      644 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/amplitude/
--rw-r--r--   0 runner    (1001) docker     (122)     2420 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/amplitude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19879 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/amplitude/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/complex/
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/complex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    18923 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/complex/diag_kernel.py
--rw-r--r--   0 runner    (1001) docker     (122)    18881 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/complex/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/crosshand_phase/
--rw-r--r--   0 runner    (1001) docker     (122)     2156 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/crosshand_phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19270 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/crosshand_phase/kernel.py
--rw-r--r--   0 runner    (1001) docker     (122)    16182 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/delay/
--rw-r--r--   0 runner    (1001) docker     (122)     6636 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/delay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24050 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/delay/kernel.py
--rw-r--r--   0 runner    (1001) docker     (122)     6517 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/gain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/general/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3453 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)    23088 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/factories.py
--rw-r--r--   0 runner    (1001) docker     (122)    12700 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/flagging.py
--rw-r--r--   0 runner    (1001) docker     (122)    16519 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/generics.py
--rw-r--r--   0 runner    (1001) docker     (122)     3550 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/general/inversion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.088158 quartical-0.1.9/quartical/gains/phase/
--rw-r--r--   0 runner    (1001) docker     (122)     2045 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/phase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21754 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/phase/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/gains/rotation_measure/
--rw-r--r--   0 runner    (1001) docker     (122)     2580 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/rotation_measure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    20628 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/rotation_measure/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/gains/tec/
--rw-r--r--   0 runner    (1001) docker     (122)     2862 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/tec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6669 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/gains/tec/kernel.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/interpolation/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/interpolation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6648 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/interpolation/interpolants.py
--rw-r--r--   0 runner    (1001) docker     (122)    10963 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/interpolation/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/logging/
--rw-r--r--   0 runner    (1001) docker     (122)     2070 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/scheduling/
--rw-r--r--   0 runner    (1001) docker     (122)     5754 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/scheduling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/statistics/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5641 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/logging.py
--rw-r--r--   0 runner    (1001) docker     (122)     1609 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/stat_kernels.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/statistics/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/collections.py
--rw-r--r--   0 runner    (1001) docker     (122)    12149 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/dask.py
--rw-r--r--   0 runner    (1001) docker     (122)     7373 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/intervals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1539 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/maths.py
--rw-r--r--   0 runner    (1001) docker     (122)      318 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/numba.py
--rw-r--r--   0 runner    (1001) docker     (122)      226 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/utils/timings.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/quartical/weights/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/weights/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7974 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/weights/robust.py
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2022-11-24 10:13:16.000000 quartical-0.1.9/quartical/weights/weights.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.084158 quartical-0.1.9/quartical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1453 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2854 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      278 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      234 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-24 10:13:17.000000 quartical-0.1.9/quartical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-24 10:13:17.096158 quartical-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1897 2022-11-24 10:13:16.000000 quartical-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/testing/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3921 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:17.092158 quartical-0.1.9/testing/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2793 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/calibration.py
--rw-r--r--   0 runner    (1001) docker     (122)      802 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/config.py
--rw-r--r--   0 runner    (1001) docker     (122)     1473 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (122)      699 2022-11-24 10:13:16.000000 quartical-0.1.9/testing/fixtures/gains.py
+-rw-r--r--   0        0        0     1078 2023-06-20 08:06:41.280731 quartical-0.2.0/LICENSE
+-rw-r--r--   0        0        0      674 2023-06-20 08:06:41.280731 quartical-0.2.0/README.md
+-rw-r--r--   0        0        0     1771 2023-06-20 08:06:41.280731 quartical-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       24 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/apps/__init__.py
+-rw-r--r--   0        0        0     4407 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/apps/backup.py
+-rw-r--r--   0        0        0    10511 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/apps/summary.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/calibration/__init__.py
+-rw-r--r--   0        0        0    12197 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/calibration/calibrate.py
+-rw-r--r--   0        0        0    11411 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/calibration/constructor.py
+-rw-r--r--   0        0        0     3676 2023-06-20 08:06:41.280731 quartical-0.2.0/quartical/calibration/mapping.py
+-rw-r--r--   0        0        0     9227 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/calibration/solver.py
+-rw-r--r--   0        0        0     1292 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/__init__.py
+-rw-r--r--   0        0        0    14136 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/argument_schema.yaml
+-rw-r--r--   0        0        0     6396 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/config_classes.py
+-rw-r--r--   0        0        0     2206 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/converters.py
+-rw-r--r--   0        0        0     1390 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/external.py
+-rw-r--r--   0        0        0     2533 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/gain_schema.yaml
+-rw-r--r--   0        0        0     3062 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/helper.py
+-rw-r--r--   0        0        0     1360 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/internal.py
+-rw-r--r--   0        0        0     4928 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/parser.py
+-rw-r--r--   0        0        0     3531 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/config/preprocess.py
+-rw-r--r--   0        0        0      108 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/__init__.py
+-rw-r--r--   0        0        0    11246 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/angles.py
+-rw-r--r--   0        0        0     9044 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/bda.py
+-rw-r--r--   0        0        0     8179 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/chunking.py
+-rw-r--r--   0        0        0     8014 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/model_handler.py
+-rw-r--r--   0        0        0    16417 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/ms_handler.py
+-rw-r--r--   0        0        0    17375 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/predict.py
+-rw-r--r--   0        0        0      411 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/selection.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/data_handling/wisdom.py
+-rw-r--r--   0        0        0     6765 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/executor.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/flagging/__init__.py
+-rw-r--r--   0        0        0     8551 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/flagging/flagging.py
+-rw-r--r--   0        0        0     5753 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/flagging/flagging_kernels.py
+-rw-r--r--   0        0        0      860 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/__init__.py
+-rw-r--r--   0        0        0     1681 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/amplitude/__init__.py
+-rw-r--r--   0        0        0    21180 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/amplitude/kernel.py
+-rw-r--r--   0        0        0     9734 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/baseline.py
+-rw-r--r--   0        0        0     1027 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/complex/__init__.py
+-rw-r--r--   0        0        0    21671 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/complex/diag_kernel.py
+-rw-r--r--   0        0        0    19731 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/complex/kernel.py
+-rw-r--r--   0        0        0     2782 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/conversion.py
+-rw-r--r--   0        0        0     1634 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/crosshand_phase/__init__.py
+-rw-r--r--   0        0        0    20489 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/crosshand_phase/kernel.py
+-rw-r--r--   0        0        0    15445 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/datasets.py
+-rw-r--r--   0        0        0     5632 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/delay/__init__.py
+-rw-r--r--   0        0        0    26272 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/delay/kernel.py
+-rw-r--r--   0        0        0     5814 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/delay_and_offset/__init__.py
+-rw-r--r--   0        0        0    28011 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/delay_and_offset/kernel.py
+-rw-r--r--   0        0        0     9357 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/gain.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/general/__init__.py
+-rw-r--r--   0        0        0     3704 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/general/convenience.py
+-rw-r--r--   0        0        0    23050 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/general/factories.py
+-rw-r--r--   0        0        0    13340 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/general/flagging.py
+-rw-r--r--   0        0        0    18704 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/general/generics.py
+-rw-r--r--   0        0        0     3550 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/general/inversion.py
+-rw-r--r--   0        0        0      593 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/leakage/__init__.py
+-rw-r--r--   0        0        0     7398 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/leakage/kernel.py
+-rw-r--r--   0        0        0     5185 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/parameterized_gain.py
+-rw-r--r--   0        0        0     1589 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/phase/__init__.py
+-rw-r--r--   0        0        0    24290 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/phase/kernel.py
+-rw-r--r--   0        0        0     1395 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/rotation/__init__.py
+-rw-r--r--   0        0        0    21632 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/rotation/kernel.py
+-rw-r--r--   0        0        0     2820 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/rotation_measure/__init__.py
+-rw-r--r--   0        0        0    22350 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/rotation_measure/kernel.py
+-rw-r--r--   0        0        0     2341 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/tec_and_offset/__init__.py
+-rw-r--r--   0        0        0    28214 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/gains/tec_and_offset/kernel.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/interpolation/__init__.py
+-rw-r--r--   0        0        0    12802 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/interpolation/interpolants.py
+-rw-r--r--   0        0        0     9068 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/interpolation/interpolate.py
+-rw-r--r--   0        0        0     2070 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/logging/__init__.py
+-rw-r--r--   0        0        0     5754 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/scheduling/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/statistics/__init__.py
+-rw-r--r--   0        0        0     5220 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/statistics/logging.py
+-rw-r--r--   0        0        0     5744 2023-06-20 08:06:41.284731 quartical-0.2.0/quartical/statistics/stat_kernels.py
+-rw-r--r--   0        0        0      667 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/statistics/statistics.py
+-rw-r--r--   0        0        0      249 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/stimela_cabs.yaml
+-rw-r--r--   0        0        0      156 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/__init__.py
+-rw-r--r--   0        0        0     1226 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/array.py
+-rw-r--r--   0        0        0      315 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/callables.py
+-rw-r--r--   0        0        0      266 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/collections.py
+-rw-r--r--   0        0        0    12149 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/dask.py
+-rw-r--r--   0        0        0     7218 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/intervals.py
+-rw-r--r--   0        0        0     1520 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/maths.py
+-rw-r--r--   0        0        0      469 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/numba.py
+-rw-r--r--   0        0        0      226 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/utils/timings.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/weights/__init__.py
+-rw-r--r--   0        0        0     9108 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/weights/robust.py
+-rw-r--r--   0        0        0     1625 2023-06-20 08:06:41.288731 quartical-0.2.0/quartical/weights/weights.py
+-rw-r--r--   0        0        0     2285 1970-01-01 00:00:00.000000 quartical-0.2.0/PKG-INFO
```

### Comparing `quartical-0.1.9/LICENSE` & `quartical-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/README.md` & `quartical-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/apps/backup.py` & `quartical-0.2.0/quartical/apps/backup.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/apps/summary.py` & `quartical-0.2.0/quartical/apps/summary.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/calibration/calibrate.py` & `quartical-0.2.0/quartical/calibration/calibrate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,69 +1,125 @@
 # -*- coding: utf-8 -*-
+import numpy as np
 import dask.array as da
+from quartical.calibration.mapping import make_mapping_datasets
 from quartical.gains.general.generics import (compute_residual,
                                               compute_corrected_residual,
                                               compute_corrected_weights)
 from quartical.calibration.constructor import construct_solver
-from quartical.calibration.mapping import make_t_maps, make_f_maps, make_d_maps
 from quartical.gains.datasets import (make_gain_xds_lod,
-                                      compute_dataset_coords,
-                                      compute_interval_chunking,
-                                      make_net_xds_list,
+                                      make_net_xds_lod,
                                       populate_net_xds_list)
 from quartical.interpolation.interpolate import load_and_interpolate_gains
+from quartical.gains.baseline import (compute_baseline_corrections,
+                                      apply_baseline_corrections)
 from loguru import logger  # noqa
-from collections import namedtuple
 
 
-# The following supresses the egregious numba pending deprecation warnings.
-# TODO: Make sure that the code doesn't break when they finally decprecate
-# reflected lists.
-from numba.core.errors import NumbaDeprecationWarning
-from numba.core.errors import NumbaPendingDeprecationWarning
-import warnings
-
-warnings.simplefilter('ignore', category=NumbaDeprecationWarning)
-warnings.simplefilter('ignore', category=NumbaPendingDeprecationWarning)
-
-
-dstat_dims_tup = namedtuple("dstat_dims_tup",
-                            "n_utime n_chan n_ant n_t_chunk n_f_chunk")
-
-
-def dask_residual(data, model, a1, a2, t_map_arr, f_map_arr, d_map_arr,
-                  sub_dirs, row_map, row_weights, corr_mode, *gains):
+def dask_residual(
+    data,
+    model,
+    a1,
+    a2,
+    sub_dirs,
+    row_map,
+    row_weights,
+    corr_mode,
+    *args
+):
     """Thin wrapper to handle an unknown number of input gains."""
 
-    return compute_residual(data, model, gains, a1, a2, t_map_arr[0],
-                            f_map_arr[0], d_map_arr, row_map, row_weights,
-                            corr_mode, sub_dirs=sub_dirs)
+    gains = tuple(args[::4])
+    time_maps = tuple(args[1::4])
+    freq_maps = tuple(args[2::4])
+    dir_maps = tuple(args[3::4])
+
+    return compute_residual(
+        data,
+        model,
+        gains,
+        a1,
+        a2,
+        time_maps,
+        freq_maps,
+        dir_maps,
+        row_map,
+        row_weights,
+        corr_mode,
+        sub_dirs=sub_dirs
+    )
 
 
-def dask_corrected_residual(residual, a1, a2, t_map_arr, f_map_arr,
-                            d_map_arr, row_map, row_weights, corr_mode,
-                            *gains):
+def dask_corrected_residual(
+    residual,
+    a1,
+    a2,
+    row_map,
+    row_weights,
+    corr_mode,
+    *args
+):
     """Thin wrapper to handle an unknown number of input gains."""
 
-    return compute_corrected_residual(residual, gains, a1, a2, t_map_arr[0],
-                                      f_map_arr[0], d_map_arr, row_map,
-                                      row_weights, corr_mode)
+    gains = tuple(args[::4])
+    time_maps = tuple(args[1::4])
+    freq_maps = tuple(args[2::4])
+    dir_maps = tuple(args[3::4])
+
+    return compute_corrected_residual(
+        residual,
+        gains,
+        a1,
+        a2,
+        time_maps,
+        freq_maps,
+        dir_maps,
+        row_map,
+        row_weights,
+        corr_mode
+    )
 
 
-def dask_corrected_weights(weights, a1, a2, t_map_arr, f_map_arr,
-                           d_map_arr, row_map, row_weights, corr_mode,
-                           *gains):
+def dask_corrected_weights(
+    weights,
+    a1,
+    a2,
+    row_map,
+    row_weights,
+    corr_mode,
+    *args
+):
     """Thin wrapper to handle an unknown number of input gains."""
 
-    return compute_corrected_weights(weights, gains, a1, a2, t_map_arr[0],
-                                     f_map_arr[0], d_map_arr, row_map,
-                                     row_weights, corr_mode)
+    gains = tuple(args[::4])
+    time_maps = tuple(args[1::4])
+    freq_maps = tuple(args[2::4])
+    dir_maps = tuple(args[3::4])
+
+    return compute_corrected_weights(
+        weights,
+        gains,
+        a1,
+        a2,
+        time_maps,
+        freq_maps,
+        dir_maps,
+        row_map,
+        row_weights,
+        corr_mode
+    )
 
 
-def add_calibration_graph(data_xds_list, solver_opts, chain_opts, output_opts):
+def add_calibration_graph(
+    data_xds_list,
+    stats_xds_list,
+    solver_opts,
+    chain,
+    output_opts
+):
     """Given data graph and options, adds the steps necessary for calibration.
 
     Extends the data graph with the steps necessary to perform gain
     calibration and in accordance with the options Namespace.
 
     Args:
         data_xds_list: A list of xarray data sets/graphs providing input data.
@@ -72,98 +128,112 @@
     Returns:
         gain_xds_lod: A list of dicts containing xarray.Datasets housing the
             solved gains.
         net_xds_list: A list of xarray.Datasets containing the effective gains.
         data_xds_list: A list of xarra.Datasets containing the MS data with
             added visibility outputs.
     """
-    # Figure out all mappings between data and solution intervals.
-    t_bin_list, t_map_list = make_t_maps(data_xds_list, chain_opts)
-    f_map_list = make_f_maps(data_xds_list, chain_opts)
-    d_map_list = make_d_maps(data_xds_list, chain_opts)
 
-    # Early compute to figure out solution intervals per data chunk.
-    tipc_list, fipc_list = compute_interval_chunking(
-        data_xds_list,
-        t_map_list,
-        f_map_list
-    )
-
-    # Early compute to figure out coordinates of gain datasets.
-    coords_per_xds = compute_dataset_coords(
-        data_xds_list,
-        t_bin_list,
-        f_map_list,
-        tipc_list,
-        fipc_list,
-        solver_opts.terms
-    )
+    # TODO: Does this check belong here or elsewhere?
+    have_dd_model = any(xds.dims['dir'] > 1 for xds in data_xds_list)
+    have_dd_chain = any(term.direction_dependent for term in chain)
+
+    if have_dd_model and not have_dd_chain:
+        logger.warning(
+            "User has specified a direction-dependent model but no gain term "
+            "has term.direction_dependent enabled. This is supported but may "
+            "indicate user error."
+        )
 
     # Create a list of dicts of xarray.Dataset objects which will describe the
     # gains per data xarray.Dataset.
-    gain_xds_lod = make_gain_xds_lod(
-        data_xds_list,
-        tipc_list,
-        fipc_list,
-        coords_per_xds,
-        chain_opts
-    )
+    gain_xds_lod = make_gain_xds_lod(data_xds_list, chain)
+
+    # Create a list of datasets containing mappings. TODO: Is this the best
+    # place to do this?
+    mapping_xds_list = make_mapping_datasets(data_xds_list, chain)
 
     # If there are gains to be loaded from disk, this will load an interpolate
-    # them to be consistent with this calibration run.
-    gain_xds_lod = load_and_interpolate_gains(gain_xds_lod, chain_opts)
+    # them to be consistent with this calibration run. TODO: This needs to
+    # be substantially improved to handle term specific behaviour/utilize
+    # mappings.
+    gain_xds_lod = load_and_interpolate_gains(
+        gain_xds_lod,
+        chain,
+        output_opts.gain_directory
+    )
 
     # Poplulate the gain xarray.Datasets with solutions and convergence info.
-    gain_xds_lod, data_xds_list = construct_solver(
+    gain_xds_lod, data_xds_list, stats_xds_list = construct_solver(
         data_xds_list,
+        mapping_xds_list,
+        stats_xds_list,
         gain_xds_lod,
-        t_bin_list,
-        t_map_list,
-        f_map_list,
-        d_map_list,
         solver_opts,
-        chain_opts
+        chain
     )
 
     if output_opts.net_gains:
         # Construct an effective gain per data_xds. This is always at the full
-        # time and frequency resolution of the data.
-        net_xds_lod = make_net_xds_list(
+        # time and frequency resolution of the data. Triggers an early compute.
+        net_xds_lod = make_net_xds_lod(
             data_xds_list,
-            coords_per_xds,
+            chain,
             output_opts
         )
 
         net_xds_lod = populate_net_xds_list(
             net_xds_lod,
             gain_xds_lod,
-            t_bin_list,
-            f_map_list,
-            d_map_list,
+            mapping_xds_list,
             output_opts
         )
     else:
         net_xds_lod = []
 
+    # TODO: This is a very hacky implementation that needs work.
+    if output_opts.compute_baseline_corrections:
+        bl_corr_xds_list = compute_baseline_corrections(
+            data_xds_list,
+            gain_xds_lod,
+            mapping_xds_list
+        )
+    else:
+        bl_corr_xds_list = None
+
     # Update the data xarray.Datasets with visibility outputs.
     data_xds_list = make_visibility_output(
         data_xds_list,
         gain_xds_lod,
-        t_map_list,
-        f_map_list,
-        d_map_list,
+        mapping_xds_list,
         output_opts
     )
 
+    if output_opts.apply_baseline_corrections:
+        data_xds_list = apply_baseline_corrections(
+            data_xds_list,
+            bl_corr_xds_list
+        )
+
     # Return the resulting graphs for the gains and updated xds.
-    return gain_xds_lod, net_xds_lod, data_xds_list
+    return (
+        gain_xds_lod,
+        net_xds_lod,
+        data_xds_list,
+        stats_xds_list,
+        bl_corr_xds_list
+    )
 
 
-def make_visibility_output(data_xds_list, solved_gain_xds_lod, t_map_list,
-                           f_map_list, d_map_list, output_opts):
+def make_visibility_output(
+    data_xds_list,
+    solved_gain_xds_lod,
+    mapping_xds_list,
+    output_opts
+):
     """Creates dask arrays for possible visibility outputs.
 
     Given and xds containing data and its assosciated gains, produces
     dask.Array objects containing the possible visibility outputs.
 
     Args:
         data_xds_list: A list of xarray.Dataset objects containing MS data.
@@ -177,110 +247,111 @@
         A dictionary of lists containing graphs which prodcuce a gain array
         per gain term per xarray dataset.
 
     """
 
     post_solve_data_xds_list = []
 
-    for xds_ind, data_xds in enumerate(data_xds_list):
+    itr = enumerate(zip(data_xds_list, mapping_xds_list))
+
+    for xds_ind, (data_xds, mapping_xds) in itr:
         data_col = data_xds.DATA.data
         model_col = data_xds.MODEL_DATA.data
         weight_col = data_xds._WEIGHT.data  # The weights exiting the solver.
         ant1_col = data_xds.ANTENNA1.data
         ant2_col = data_xds.ANTENNA2.data
         gain_terms = solved_gain_xds_lod[xds_ind]
-        t_map_arr = t_map_list[xds_ind]
-        f_map_arr = f_map_list[xds_ind]
-        d_map_arr = d_map_list[xds_ind]
+
+        time_maps = tuple(
+            [mapping_xds.get(f"{k}_time_map").data for k in gain_terms.keys()]
+        )
+        freq_maps = tuple(
+            [mapping_xds.get(f"{k}_freq_map").data for k in gain_terms.keys()]
+        )
+        dir_maps = tuple(
+            [mapping_xds.get(f"{k}_dir_map").data for k in gain_terms.keys()]
+        )
+
         corr_mode = data_xds.dims["corr"]
 
         is_bda = hasattr(data_xds, "ROW_MAP")  # We are dealing with BDA.
         row_map = data_xds.ROW_MAP.data if is_bda else None
         row_weights = data_xds.ROW_WEIGHTS.data if is_bda else None
 
         gain_schema = ("rowlike", "chan", "ant", "dir", "corr")
 
-        # TODO: For gains with n_dir > 1, we can select out the gains we
-        # actually want to correct for.
-        gain_list = [x for gxds in gain_terms.values()
-                     for x in (gxds.gains.data, gain_schema)]
+        term_args = []
+
+        for gain_idx, gain_xds in enumerate(gain_terms.values()):
+            term_args.extend([gain_xds.gains.data, gain_schema])
+            term_args.extend([time_maps[gain_idx], ("rowlike",)])
+            term_args.extend([freq_maps[gain_idx], ("chan",)])
+            term_args.extend([dir_maps[gain_idx], ("dir",)])
 
         residual = da.blockwise(
             dask_residual, ("rowlike", "chan", "corr"),
             data_col, ("rowlike", "chan", "corr"),
             model_col, ("rowlike", "chan", "dir", "corr"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
-            t_map_arr, ("gp", "rowlike", "term"),
-            f_map_arr, ("gp", "chan", "term"),
-            d_map_arr, None,
             output_opts.subtract_directions, None,
             *((row_map, ("rowlike",)) if is_bda else (None, None)),
             *((row_weights, ("rowlike",)) if is_bda else (None, None)),
             corr_mode, None,
-            *gain_list,
-            dtype=data_col.dtype,
+            *term_args,
+            meta=np.empty((0, 0, 0), dtype=data_col.dtype),
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": data_col.chunks[0],
                            "chan": data_col.chunks[1]})
 
         corrected_residual = da.blockwise(
             dask_corrected_residual, ("rowlike", "chan", "corr"),
             residual, ("rowlike", "chan", "corr"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
-            t_map_arr, ("gp", "rowlike", "term"),
-            f_map_arr, ("gp", "chan", "term"),
-            d_map_arr, None,
             *((row_map, ("rowlike",)) if is_bda else (None, None)),
             *((row_weights, ("rowlike",)) if is_bda else (None, None)),
             corr_mode, None,
-            *gain_list,
-            dtype=residual.dtype,
+            *term_args,
+            meta=np.empty((0, 0, 0), dtype=residual.dtype),
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": data_col.chunks[0],
                            "chan": data_col.chunks[1]})
 
         # We can cheat and reuse the corrected residual code - the only
         # difference is whether we supply the residuals or the data.
         corrected_data = da.blockwise(
             dask_corrected_residual, ("rowlike", "chan", "corr"),
             data_col, ("rowlike", "chan", "corr"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
-            t_map_arr, ("gp", "rowlike", "term"),
-            f_map_arr, ("gp", "chan", "term"),
-            d_map_arr, None,
             *((row_map, ("rowlike",)) if is_bda else (None, None)),
             *((row_weights, ("rowlike",)) if is_bda else (None, None)),
             corr_mode, None,
-            *gain_list,
-            dtype=residual.dtype,
+            *term_args,
+            meta=np.empty((0, 0, 0), dtype=data_col.dtype),
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": data_col.chunks[0],
                            "chan": data_col.chunks[1]})
 
         # We may also want to form corrected weights. Not technicallay a
         # visibility output but close enough. TODO: Change calling function.
         corrected_weight = da.blockwise(
             dask_corrected_weights, ("rowlike", "chan", "corr"),
             weight_col, ("rowlike", "chan", "corr"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
-            t_map_arr, ("gp", "rowlike", "term"),
-            f_map_arr, ("gp", "chan", "term"),
-            d_map_arr, None,
             *((row_map, ("rowlike",)) if is_bda else (None, None)),
             *((row_weights, ("rowlike",)) if is_bda else (None, None)),
             corr_mode, None,
-            *gain_list,
-            dtype=weight_col.dtype,
+            *term_args,
+            meta=np.empty((0, 0, 0), dtype=weight_col.dtype),
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": data_col.chunks[0],
                            "chan": data_col.chunks[1]}
         )
 
         # QuartiCal will assign these to the xarray.Datasets as the following
```

### Comparing `quartical-0.1.9/quartical/calibration/constructor.py` & `quartical-0.2.0/quartical/calibration/constructor.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,59 +4,56 @@
 from collections import namedtuple
 
 
 term_spec_tup = namedtuple("term_spec_tup", "name type shape pshape")
 aux_info_fields = ("SCAN_NUMBER", "FIELD_ID", "DATA_DESC_ID")
 
 
-def construct_solver(data_xds_list,
-                     gain_xds_lod,
-                     t_bin_list,
-                     t_map_list,
-                     f_map_list,
-                     d_map_list,
-                     solver_opts,
-                     chain_opts):
+def construct_solver(
+    data_xds_list,
+    mapping_xds_list,
+    stats_xds_list,
+    gain_xds_lod,
+    solver_opts,
+    chain
+):
     """Constructs the dask graph for the solver layer.
 
     This constructs a custom dask graph for the solver layer given the slew
     of solver inputs. This is arguably the most important function in V2 and
     should not be tampered with without a certain level of expertise with dask.
 
     Args:
         data_xds_list: A list of xarray.Dataset objects containing MS data.
         gain_xds_lod: A list of dicts containing xarray.Dataset objects
             describing the gain terms.
         t_map_list: List of dask.Array objects containing time mappings.
         f_map_list: List of dask.Array objects containing frequency mappings.
         d_map_list: List of dask.Array objects containing direction mappings.
         solver_opts: A Solver config object.
-        chain_opts: A Chain config object.
+        chain: A list of Gain objects.
 
     Returns:
         solved_gain_xds_lod: A list of dicts containing xarray.Datasets
             describing the solved gains.
     """
 
     solved_gain_xds_lod = []
     output_data_xds_list = []
+    output_stats_xds_list = []
 
-    for xds_ind, data_xds in enumerate(data_xds_list):
+    required_fields = {fld for term in chain for fld in term.ms_inputs._fields}
+
+    itr = enumerate(zip(data_xds_list, mapping_xds_list, stats_xds_list))
+
+    for xds_ind, (data_xds, mapping_xds, stats_xds) in itr:
 
-        model_col = data_xds.MODEL_DATA.data
         data_col = data_xds.DATA.data
-        ant1_col = data_xds.ANTENNA1.data
-        ant2_col = data_xds.ANTENNA2.data
         weight_col = data_xds.WEIGHT.data
         flag_col = data_xds.FLAG.data
-        chan_freqs = data_xds.CHAN_FREQ.data
-        t_bin_arr = t_bin_list[xds_ind]
-        t_map_arr = t_map_list[xds_ind]
-        f_map_arr = f_map_list[xds_ind]
-        d_map_arr = d_map_list[xds_ind]
         gain_terms = gain_xds_lod[xds_ind]
         corr_mode = data_xds.dims["corr"]
 
         block_id_arr = get_block_id_arr(data_col)
         aux_block_info = {
             k: data_xds.attrs.get(k, "?") for k in aux_info_fields
         }
@@ -65,165 +62,222 @@
         # safe.
         n_t_chunks, n_f_chunks, _ = data_col.numblocks
 
         # Take the compact chunking info on the gain xdss and expand it.
         spec_list = expand_specs(gain_terms)
 
         # Create a blocker object.
-        blocker = Blocker(solver_wrapper, "rf")
+        blocker = Blocker(solver_wrapper, ("row", "chan"))
 
-        # Add relevant inputs to the blocker object. TODO: Only pass in values
-        # required by the specific terms in use.
-        blocker.add_input("model", model_col, "rfdc")
-        blocker.add_input("data", data_col, "rfc")
-        blocker.add_input("a1", ant1_col, "r")
-        blocker.add_input("a2", ant2_col, "r")
-        blocker.add_input("weights", weight_col, "rfc")
-        blocker.add_input("flags", flag_col, "rf")
-        blocker.add_input("t_bin_arr", t_bin_arr, "prj")  # Not always needed.
-        blocker.add_input("t_map_arr", t_map_arr, "prj")
-        blocker.add_input("f_map_arr", f_map_arr, "pfj")
-        blocker.add_input("d_map_arr", d_map_arr)
+        for v in data_xds.data_vars.values():
+            if v.name in required_fields:
+                blocker.add_input(v.name, v.data, v.dims)
+
+        # NOTE: We need to treat time as a rowlike dimension here.
+        for v in mapping_xds.data_vars.values():
+            blocker.add_input(
+                v.name,
+                v.data,
+                ("row",) if v.dims == ("time",) else v.dims
+            )
+
+        blocker.add_input(
+            "block_id_arr",
+            block_id_arr,
+            ("row", "chan", "corr")
+        )
+        blocker.add_input("term_spec_list", spec_list, ("row", "chan"))
         blocker.add_input("corr_mode", corr_mode)
-        blocker.add_input("term_spec_list", spec_list, "rf")
-        blocker.add_input("chan_freqs", chan_freqs, "f")  # Not always needed.
-        blocker.add_input("block_id_arr", block_id_arr, "rfc")
         blocker.add_input("aux_block_info", aux_block_info)
         blocker.add_input("solver_opts", solver_opts)
-        blocker.add_input("chain_opts", chain_opts)
+        blocker.add_input("chain", chain)
 
         # If the gain dataset already has a gain variable, we want to pass
         # it in to initialize the solver.
         for term_name, term_xds in gain_terms.items():
             if "gains" in term_xds.data_vars:
-                blocker.add_input(f"{term_name}_initial_gain",
-                                  term_xds.gains.data,
-                                  "rfadc")
-
-        if hasattr(data_xds, "ROW_MAP"):  # We are dealing with BDA.
-            blocker.add_input("row_map", data_xds.ROW_MAP.data, "r")
-            blocker.add_input("row_weights", data_xds.ROW_WEIGHTS.data, "r")
-        else:
-            blocker.add_input("row_map", None)
-            blocker.add_input("row_weights", None)
+                blocker.add_input(
+                    f"{term_name}_initial_gain",
+                    term_xds.gains.data,
+                    ("row", "chan", "ant", "dir", "corr")
+                )
+            if "params" in term_xds.data_vars:
+                blocker.add_input(
+                    f"{term_name}_initial_params",
+                    term_xds.params.data,
+                    ("row", "chan", "ant", "dir", "param")
+                )
 
         # Add relevant outputs to blocker object.
-        blocker.add_output("weights",
-                           "rfc",
-                           weight_col.chunks,
-                           weight_col.dtype)
-
-        blocker.add_output("flags",
-                           "rf",
-                           flag_col.chunks,
-                           flag_col.dtype)
+        blocker.add_output(
+            "weights",
+            ("row", "chan", "corr"),
+            weight_col.chunks,
+            weight_col.dtype
+        )
+
+        blocker.add_output(
+            "flags",
+            ("row", "chan"),
+            flag_col.chunks,
+            flag_col.dtype
+        )
+
+        blocker.add_output(
+            "presolve_chisq",
+            ("row", "chan"),
+            ((1,)*n_t_chunks, (1,)*n_f_chunks),
+            np.float64
+        )
+
+        blocker.add_output(
+            "postsolve_chisq",
+            ("row", "chan"),
+            ((1,)*n_t_chunks, (1,)*n_f_chunks),
+            np.float64
+        )
 
         for term_name, term_xds in gain_terms.items():
 
-            blocker.add_output(f"{term_name}-gain",
-                               "rfadc",
-                               term_xds.GAIN_SPEC,
-                               np.complex128)
-
-            blocker.add_output(f"{term_name}-gain_flags",
-                               "rfad",
-                               term_xds.GAIN_SPEC[:-1],
-                               np.int8)
+            blocker.add_output(
+                f"{term_name}_gains",
+                ("row", "chan", "ant", "dir", "corr"),
+                term_xds.GAIN_SPEC,
+                np.complex128
+            )
+
+            blocker.add_output(
+                f"{term_name}_gain_flags",
+                ("row", "chan", "ant", "dir"),
+                term_xds.GAIN_SPEC[:-1],
+                np.int8
+            )
 
             # If there is a PARAM_SPEC on the gain xds, it is also an output.
             if hasattr(term_xds, "PARAM_SPEC"):
-                blocker.add_output(f"{term_name}-param",
-                                   "rfadp",
-                                   term_xds.PARAM_SPEC,
-                                   np.float64)
-
-                blocker.add_output(f"{term_name}-param_flags",
-                                   "rfad",
-                                   term_xds.PARAM_SPEC[:-1],
-                                   np.int8)
+                blocker.add_output(
+                    f"{term_name}_params",
+                    ("row", "chan", "ant", "dir", "param"),
+                    term_xds.PARAM_SPEC,
+                    np.float64
+                )
+
+                blocker.add_output(
+                    f"{term_name}_param_flags",
+                    ("row", "chan", "ant", "dir"),
+                    term_xds.PARAM_SPEC[:-1],
+                    np.int8
+                )
+
+                blocker.add_output(
+                    f"{term_name}_jhj",
+                    ("row", "chan", "ant", "dir", "param"),
+                    term_xds.PARAM_SPEC,
+                    np.float64
+                )
 
             else:  # Only non-parameterised gains return a jhj (for now).
-                blocker.add_output(f"{term_name}-jhj",
-                                   "rfadc",
-                                   term_xds.GAIN_SPEC,
-                                   np.complex128)
+                blocker.add_output(
+                    f"{term_name}_jhj",
+                    ("row", "chan", "ant", "dir", "corr"),
+                    term_xds.GAIN_SPEC,
+                    np.complex128
+                )
 
             chunks = ((1,)*n_t_chunks, (1,)*n_f_chunks)
-            blocker.add_output(f"{term_name}-conviter",
-                               "rf",
-                               chunks,
-                               np.int64)
-            blocker.add_output(f"{term_name}-convperc",
-                               "rf",
-                               chunks,
-                               np.float64)
+            blocker.add_output(
+                f"{term_name}_conviter",
+                ("row", "chan"),
+                chunks,
+                np.int64
+            )
+            blocker.add_output(
+                f"{term_name}_convperc",
+                ("row", "chan"),
+                chunks,
+                np.float64
+            )
 
         # Apply function to inputs to produce dask array outputs (as dict).
         output_dict = blocker.get_dask_outputs()
 
         # Assign column results to the relevant data xarray.Dataset object.
         # NOTE: Only update FLAG if we are honouring solver flags.
         flag_field = "FLAG" if solver_opts.propagate_flags else "_FLAG"
 
         output_data_xds = data_xds.assign(
             {"_WEIGHT": (data_xds.WEIGHT.dims, output_dict["weights"]),
              flag_field: (data_xds.FLAG.dims, output_dict["flags"])}
         )
         output_data_xds_list.append(output_data_xds)
 
+        presolve_chisq = output_dict["presolve_chisq"]
+        postsolve_chisq = output_dict["postsolve_chisq"]
+
+        stats_xds = stats_xds.assign(
+            {
+                "PRESOLVE_CHISQ": (("t_chunk", "f_chunk"), presolve_chisq),
+                "POSTSOLVE_CHISQ": (("t_chunk", "f_chunk"), postsolve_chisq)
+            }
+        )
+        output_stats_xds_list.append(stats_xds)
+
         # Assign results to the relevant gain xarray.Dataset object.
         solved_gain_dict = {}
 
         for term_name, term_xds in gain_terms.items():
 
             result_vars = {}
 
-            gain = output_dict[f"{term_name}-gain"]
+            gain = output_dict[f"{term_name}_gains"]
             result_vars["gains"] = (term_xds.GAIN_AXES, gain)
 
-            flags = output_dict[f"{term_name}-gain_flags"]
+            flags = output_dict[f"{term_name}_gain_flags"]
             result_vars["gain_flags"] = (term_xds.GAIN_AXES[:-1], flags)
 
-            convperc = output_dict[f"{term_name}-convperc"]
-            result_vars["conv_perc"] = (("t_chunk", "f_chunk"), convperc)
+            convperc = output_dict[f"{term_name}_convperc"]
+            result_vars["conv_perc"] = (("time_chunk", "freq_chunk"), convperc)
 
-            conviter = output_dict[f"{term_name}-conviter"]
-            result_vars["conv_iter"] = (("t_chunk", "f_chunk"), conviter)
+            conviter = output_dict[f"{term_name}_conviter"]
+            result_vars["conv_iter"] = (("time_chunk", "freq_chunk"), conviter)
 
             if hasattr(term_xds, "PARAM_SPEC"):
-                params = output_dict[f"{term_name}-param"]
+                params = output_dict[f"{term_name}_params"]
                 result_vars["params"] = (term_xds.PARAM_AXES, params)
 
-                param_flags = output_dict[f"{term_name}-param_flags"]
+                param_flags = output_dict[f"{term_name}_param_flags"]
                 result_vars["param_flags"] = \
                     (term_xds.PARAM_AXES[:-1], param_flags)
+
+                jhj = output_dict[f"{term_name}_jhj"]
+                result_vars["jhj"] = (term_xds.PARAM_AXES, jhj)
             else:
-                jhj = output_dict[f"{term_name}-jhj"]
+                jhj = output_dict[f"{term_name}_jhj"]
                 result_vars["jhj"] = (term_xds.GAIN_AXES, jhj)
 
             solved_xds = term_xds.assign(result_vars)
 
             solved_gain_dict[term_name] = solved_xds
 
         solved_gain_xds_lod.append(solved_gain_dict)
 
-    return solved_gain_xds_lod, output_data_xds_list
+    return solved_gain_xds_lod, output_data_xds_list, output_stats_xds_list
 
 
 def expand_specs(gain_terms):
     """Convert compact spec to a per-term list per-chunk."""
 
     # TODO: This was rejiggered to work with the updated Blocker. Could stand
     # to be made a little neater/smarter, but works for now. Assembles nested
     # list where the outer list represnts time chunks, the middle list
     # represents frequency chunks and the inner-most list contains the
     # specs per term. Might be possible to do this with arrays instead.
 
-    n_t_chunks = set(xds.dims["t_chunk"] for xds in gain_terms.values())
-    n_f_chunks = set(xds.dims["f_chunk"] for xds in gain_terms.values())
+    n_t_chunks = set(xds.dims["time_chunk"] for xds in gain_terms.values())
+    n_f_chunks = set(xds.dims["freq_chunk"] for xds in gain_terms.values())
 
     assert len(n_t_chunks) == 1, "Chunking in time is inconsistent."
     assert len(n_f_chunks) == 1, "Chunking in freq is inconsistent."
 
     n_t_chunks = n_t_chunks.pop()
     n_f_chunks = n_f_chunks.pop()
```

### Comparing `quartical-0.1.9/quartical/config/converters.py` & `quartical-0.2.0/quartical/config/converters.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/config/helpstrings.yaml` & `quartical-0.2.0/quartical/config/argument_schema.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,248 +1,409 @@
 input_ms:
   path:
-    Path to input measurement set.
+    required: true
+    dtype: str
+    info:
+      Path to input measurement set.
+
   data_column:
-    Name of column to use as data.
+    dtype: str
+    default: DATA
+    info:
+      Name of column to use as data.
+
   sigma_column:
-    When given, the weights will be reinitialized as 1/sigma_column**2. This
-    should be preferred over input_ms.weight_column to ensure that the correct
-    data weights are used and not those from a previous calibration run.
-    Mutually exclusive with input_ms.weight_column.
+    dtype: Optional[str]
+    info:
+      When given, the weights will be reinitialized as 1/sigma_column**2. This
+      should be preferred over weight_column to ensure that the correct
+      data weights are used and not those from a previous calibration run.
+      Mutually exclusive with input_ms.weight_column.
+
   weight_column:
-    Column to read weights from. An empty string will result in all weights
-    being treated as unity if input_ms.sigma_column is not set. Mutually
-    exclusive with input_ms.sigma_column (which is preferred).
+    dtype: Optional[str]
+    info:
+      Column to read weights from. An empty string will result in all weights
+      being treated as unity if sigma_column is not set. Mutually
+      exclusive with input_ms.sigma_column (which is preferred).
+
   time_chunk:
-    Chunk data up by this number of timeslots. This limits the amount of data
-    processed at once. Smaller chunks allow for a smaller RAM footprint and
-    greater parallelism, but this sets an upper limit on the solution
-    intervals that may be employed. Specify as an integer number of timeslots,
-    or a value with a unit (e.g. '300s'). 0 means use full time axis.
+    dtype: str
+    default: '0'
+    info:
+      Chunk data up by this number of timeslots. This limits the amount of
+      data processed at once. Smaller chunks allow for a smaller RAM footprint
+      and greater parallelism, but this sets an upper limit on the solution
+      intervals that may be employed. Specify as an integer number of
+      timeslots, or a value with a unit (e.g. '300s'). 0 means use full time
+      axis.
+
   freq_chunk:
-    Chunk data by this number of channels. See time_chunk for info. Specify as
-    an integer number of channels, or a value with a unit (e.g. '128MHz').
-    0 means use full frequency axis.
+    dtype: str
+    default: '0'
+    info:
+      Chunk data by this number of channels. See time_chunk for info. Specify
+      as an integer number of channels, or a value with a unit (e.g. '128MHz').
+      0 means use full frequency axis.
+
   is_bda:
-    If set True, the input measurement set is assumed to have been averaged in
-    a baseline dependent fashion.
+    dtype: bool
+    default: False
+    info:
+      If set True, the input measurement set is assumed to have been averaged
+      in a baseline dependent fashion.
+
   group_by:
-    Input data will be partitioned into separate xarray datasets based on the
-    values of the specified columns. Multiple column names may be given as a
-    list, e.g. [SCAN_NUMBER, FIELD_ID, DATA_DESC_ID].
+    dtype: Optional[List[str]]
+    default: ["SCAN_NUMBER", "FIELD_ID", "DATA_DESC_ID"]
+    element_choices: ["SCAN_NUMBER", "FIELD_ID", "DATA_DESC_ID"]
+    info:
+      Input data will be partitioned into separate xarray datasets based on the
+      values of the specified columns. Multiple column names may be given as a
+      list, e.g. [SCAN_NUMBER, FIELD_ID, DATA_DESC_ID].
+
   select_corr:
-    Select correlations from the input data. These are specified as integer
-    values and must be given as a list e.g. to select the first and last
-    correlations in a measurement set with four correlations, use [0, 3].
+    dtype: Optional[List[int]]
+    element_choices: [0,1,2,3]
+    info:
+      Select correlations from the input data. These are specified as integer
+      values and must be given as a list e.g. to select the first and last
+      correlations in a measurement set with four correlations, use [0, 3].
+
   select_fields:
-    Select fields from the input data. These are specified as integer
-    values and must be given as a list e.g. to select fields 2 and 6
-    use [2, 6].
+    dtype: List[int]
+    default: []
+    info:
+      Select fields from the input data. These are specified as integer
+      values and must be given as a list e.g. to select fields 2 and 6
+      use [2, 6].
+
   select_ddids:
-    Select data descriptor IDs (spectral windows) from the input data. These
-    are specified as integer values and must be given as a list e.g. to select
-    ddids/SPWs 0 and 2, use [0, 2].
-  select_uv_range:
-    Select a range of uv values to include when calibrating. Practically, this
-    treats points outside the range as having zero weight. Use zero to
-    indicate an open interval, e.g. [100, 0] would select all values greater
-    than 100, [0, 10000] would select all values less than 10000 and
-    [100, 10000] would select values greater than 100 but less than 10000.
+    dtype: List[int]
+    default: []
+    info:
+      Select data descriptor IDs (spectral windows) from the input data. These
+      are specified as integer values and must be given as a list e.g. to
+      select ddids/SPWs 0 and 2, use [0, 2].
 
+  select_uv_range:
+    dtype: List[float]
+    default: [0, 0]
+    info:
+      Select a range of uv values to include when calibrating. Practically,
+      this treats points outside the range as having zero weight. Use zero to
+      indicate an open interval, e.g. [100, 0] would select all values greater
+      than 100, [0, 10000] would select all values less than 10000 and
+      [100, 10000] would select values greater than 100 but less than 10000.
 
 input_model:
   recipe:
-    Input model recipe. This is a string which describes how the model data
-    should be constructed. Currently, measurement set columns and Tigger lsms
-    are supported. Multiple columns and lsms can be specified and combined
-    using colons (:), addition (+) and negation (~). As an example consider
-    COL1, COL2 and LSM1. "COL1" will simply use a single MS column as input.
-    "COL1:COL2" will create a direction dependent model with COL1 as the
-    first direction and COL2 as the second. "COL1~COL2" will create a model
-    with a single direction by subtracting COL2 from COL1. "COL1+COL2" will
-    create a model with a single direction by adding COL1 and COL2. Tigger
-    lsms can be used interchangeably with columns (using the same syntax) but
-    also support the use of tagged directions. "LSM1" will create a model with
-    a single direction from the sky model. "LSM1@dE" will create a model with
-    multiple directions, one for each cluster tagged with dE in the lsm.
-    Combining all of the above it is possible to do things like
-    "COL1~LSM1:LSM1@dE" which will create a model with multiple
-    directions, the first given by COL1 minus LSM1 and the remainder given
-    given by the dE tagged clusters in LSM1.
+    dtype: Optional[str]
+    info:
+      Input model recipe. This is a string which describes how the model
+      data should be constructed. Currently, measurement set columns and
+      Tigger lsms are supported. Multiple columns and lsms can be specified
+      and combined using colons (:), addition (+) and negation (~). As an
+      example consider COL1, COL2 and LSM1. "COL1" will simply use a single
+      MS column as input. "COL1:COL2" will create a direction dependent
+      model with COL1 as the first direction and COL2 as the second.
+      "COL1~COL2" will create a model with a single direction by subtracting
+      COL2 from COL1. "COL1+COL2" will create a model with a single
+      direction by adding COL1 and COL2. Tigger lsms can be used
+      interchangeably with columns (using the same syntax) but also support
+      the use of tagged directions. "LSM1" will create a model with a single
+      direction from the sky model. "LSM1@dE" will create a model with
+      multiple directions, one for each cluster tagged with dE in the lsm.
+      Combining all of the above it is possible to do things like
+      "COL1~LSM1:LSM1@dE" which will create a model with multiple
+      directions, the first given by COL1 minus LSM1 and the remainder given
+      given by the dE tagged clusters in LSM1. Leaving this value unset
+      (the default) will use an identity model.
+
   beam:
-    Path to beams. Apply beams during predict if specified eg.
-    'beam_$(corr)_$(reim).fits' or 'beam_$(CORR)_$(REIM).fits'.
+    dtype: Optional[str]
+    info:
+      Path to beams. Apply beams during predict if specified eg.
+      'beam_$(corr)_$(reim).fits' or 'beam_$(CORR)_$(REIM).fits'.
+
   beam_l_axis:
-    Determines the orientation of the beam l-axis. Note that ~ indicates
-    flipping the orientation of the axis.
+    default: X
+    choices: ["X", "~X", "Y", "~Y", "L", "~L", "M", "~M"]
+    info:
+      Determines the orientation of the beam l-axis. Note that ~ indicates
+      flipping the orientation of the axis.
+
   beam_m_axis:
-    Determines the orientation of the beam m-axis. See beam_l_axis.
+    default: Y
+    choices: ["X", "~X", "Y", "~Y", "L", "~L", "M", "~M"]
+    info:
+      Determines the orientation of the beam m-axis. See beam_l_axis.
+
   invert_uvw:
-    The UVW coordinates will be negated if this option is specified. Enabled
-    by default to match the Casa convention.
+    dtype: bool
+    default: true
+    info:
+      The UVW coordinates will be negated if this option is specified.
+      Enabled by default to match the Casa convention.
+
   source_chunks:
-    The number of sources to predict simultaneously. Has a large impact on
-    memory footprint.
-  apply_p_jones:
-    Determines whether P-Jones (parallactic angle rotation) is applied to the
-    model. This affects both measurement set columns and predicted components.
-    Care must taken when using this option and output.apply_p_jones_inv.
+    dtype: int
+    default: 500
+    info:
+      The number of sources to predict simultaneously. Has a large impact on
+      memory footprint.
 
+  apply_p_jones:
+    dtype: bool
+    default: false
+    info:
+      Determines whether P-Jones (parallactic angle rotation) is applied to
+      the model. This affects both measurement set columns and predicted
+      components. Care must taken when using this option and
+      output.apply_p_jones_inv.
 
 output:
   gain_directory:
-    Name of directory in which QuartiCal gain outputs will be stored. Accepts
-    both local and s3 paths. QuartiCal will always produce gain outputs.
+    default: gains.qc
+    dtype: str
+    info:
+      Name of directory in which QuartiCal gain outputs will be stored.
+      Accepts both local and s3 paths. QuartiCal will always produce gain
+      outputs.
+
   log_directory:
-    Name of directory in which QuartiCal logging outputs will be stored. s3
-    is not currently supported for these outputs.
+    default: logs.qc
+    dtype: str
+    info:
+      Name of directory in which QuartiCal logging outputs will be stored.
+      s3 is not currently supported for these outputs.
+
   log_to_terminal:
-    Enable or disable logging to terminal.
+    default: true
+    dtype: bool
+    info:
+      Enable or disable logging to terminal.
+
   overwrite:
-    Whether or not the contents of the output directory may be overwritten.
-    Will trigger an error when False and output.directory already exists.
+    dtype: bool
+    default: False
+    info:
+      Whether or not the contents of the output directory may be overwritten.
+      Will trigger an error when False and output.directory already exists.
+
   products:
-    The desired output data products. Multiple data products can be specified
-    as a list e.g. [residual, corrected_residual]. Any required measurement
-    set outputs should be specified here. Note that the output names of the
-    desired products should be specified via output.columns.
+    dtype: Optional[List[str]]
+    element_choices:
+      - corrected_data
+      - corrected_residual
+      - residual
+      - weight
+      - corrected_weight
+      - model_data
+    info:
+      The desired output data products. Multiple data products can be
+      specified as a list e.g. [residual, corrected_residual]. Any required
+      measurement set outputs should be specified here. Note that the output
+      names of the desired products should be specified via output.columns.
+
   columns:
-    Output MS column names for visibility outputs (if applicable).
-    Column names will be used in order, matching the order of output.products.
-    Multiple columns can be specified as a list e.g. [COL1, COL2, COL3].
+    dtype: Optional[List[str]]
+    info:
+      Output MS column names for visibility outputs (if applicable).
+      Column names will be used in order, matching the order of
+      output.products. Multiple columns can be specified as a list e.g.
+      [COL1, COL2, COL3].
+
   flags:
-    If True, write out flags to FLAG and FLAG_ROW. This can be disabled if
-    you want QuartiCal to leave the measurement set flags unaltered.
+    dtype: bool
+    default: True
+    info:
+      If True, write out flags to FLAG and FLAG_ROW. This can be disabled if
+      you want QuartiCal to leave the measurement set flags unaltered.
+
   apply_p_jones_inv:
-    Determines whether the inverse of P-Jones (parallactic angle rotation) is
-    applied to the output visibilitites. This has the effect of derotating
-    the output visibilities into the sky frame. Care must taken when using
-    this option and input_model.apply_p_jones.
-  net_gains:
-    Merge subsets of gains into an effective/net gain per antenna per time per
-    channel. This is formed by multiplying all the specified gains together.
-    This can be used to reduce the computational load of solution transfer by
-    transferring merged gains rather than each individual term. Accepts a list
-    or a list of lists e.g. ["K", "G", "X", "B"] or [["K", "G"], ["X", "B"]].
-    Results will be written to outputs.gain_directory as e.g. KGXB-net.
+    dtype: bool
+    default: false
+    info:
+      Determines whether the inverse of P-Jones (parallactic angle rotation)
+      is applied to the output visibilitites. This has the effect of
+      derotating the output visibilities into the sky frame. Care must taken
+      when using this option and input_model.apply_p_jones.
+
   subtract_directions:
-    Which model directions to subtract when generating residuals. Must be
-    specified as a list of integers e.g. [0, 5, 7]. The default will subtract
-    all directions.
+    dtype: Optional[List[int]]
+    info:
+      Which model directions to subtract when generating residuals. Must be
+      specified as a list of integers e.g. [0, 5, 7]. The default will
+      subtract all directions.
+
+  net_gains:
+    dtype: Optional[List[Any]]
+    info:
+      Merge subsets of gains into an effective/net gain per antenna per time
+      per channel. This is formed by multiplying all the specified gains
+      together. This can be used to reduce the computational load of
+      solution transfer by transferring net/effective gains rather than each
+      individual term. Accepts a list or a list of lists e.g.
+      ["K", "G", "X", "B"] or [["K", "G"], ["X", "B"]]. Results will be
+      written to outputs.gain_directory as e.g. KGXB-net.
+
+  compute_baseline_corrections:
+    dtype: bool
+    default: false
+    info:
+      Enable or disable computation of baseline-based corrections.
+      Functionality is currently limited to a solution per-channel, per-chunk.
+      These solutions are useful for analysis and are stored in
+      output.gain_directory.
 
+  apply_baseline_corrections:
+    dtype: bool
+    default: false
+    info:
+      Enable or disable application of baseline-based corrections. Extreme
+      caution advised - this can and will lead to overfitting.
 
 mad_flags:
   enable:
-    Enables the MAD flagging routines.
+    dtype: bool
+    default: False
+    info:
+      Enables the MAD flagging routines.
+
   whitening:
-    Determines whether and how the residuals are whitened (multiplied by the
-    square root of the weights) prior to performing MAD flagging. "native"
-    whitening will use the original weights (specified in the input_ms
-    section). "robust" will use the weights produced when solver.robust=True.
-    "disabled" will result in the MAD estimate being performed on the
-    unwhitened residuals.
+    dtype: str
+    default: disabled
+    info:
+      Determines whether and how the residuals are whitened (multiplied by
+      the square root of the weights) prior to performing MAD flagging.
+      "native" whitening will use the original weights (specified in the
+      input_ms section). "robust" will use the weights produced when
+      solver.robust=True. "disabled" will result in the MAD estimate being
+      performed on the unwhitened residuals.
+
   threshold_bl:
-    Multiplicative factor which determines whether or not a chi-squared value
-    is considered to deviate significantly from the median of a given baseline.
-    Values greater than MAD_bl*threshold_bl will be flagged.
+    dtype: float
+    default: 5
+    info:
+      Multiplicative factor which determines whether or not a chi-squared
+      value is considered to deviate significantly from the median of a
+      given baseline. Values greater than MAD_bl*threshold_bl will be
+      flagged.
+
   threshold_global:
-    Multiplicative factor which determines whether or not a chi-squared value
-    is considered to deviate significantly from the median of a given data
-    chunk. Values greater than MAD*threshold_global will be flagged.
-  max_deviation:
-    Multiplicative factor which determines whether or not the MAD estimate
-    on a given baseline is considered to deviate too much from the global
-    MAD estimate. If the MAD estimate over all baselines is X, and the MAD
-    estimate on a specific baseline is X_bl, baselines for which
-    X_bl > max_deviation*X will be flagged.
+    dtype: float
+    default: 5
+    info:
+      Multiplicative factor which determines whether or not a chi-squared
+      value is considered to deviate significantly from the median of a
+      given data chunk. Values greater than MAD*threshold_global will be
+      flagged.
 
+  max_deviation:
+    dtype: float
+    default: 5
+    info:
+      Multiplicative factor which determines whether or not the MAD estimate
+      on a given baseline is considered to deviate too much from the global
+      MAD estimate. If the MAD estimate over all baselines is X, and the MAD
+      estimate on a specific baseline is X_bl, baselines for which
+      X_bl > max_deviation*X will be flagged.
 
 solver:
   terms:
-    Gain terms for which we are solving. Multiple terms can be specified as
-    a list e.g. [G,B,dE]. Each term specified here has its own set of
-    arguments which can be specified as (gain).(option). e.g. G.time_interval.
+    dtype: List[str]
+    default: [G]
+    info:
+      Gain terms for which we are solving. Multiple terms can be specified
+      as a list e.g. [G,B,dE]. Each term specified here has its own set of
+      arguments which can be specified as (gain).(option). e.g.
+      G.time_interval.
+
   iter_recipe:
-    Specifies the iterations to be performed per gain term. This argument
-    expects a list as long or longer than solver.terms. If solver.terms
-    was given as [K,G,B], an iteration recipe of [20,10,5] would do 20
-    iterations for K, 10 for G and 5 for B. To loop over the gains multiple
-    times, use a longer list e.g. [20,10,5,15,5,0] would do the same as
-    the first example but then do an additional 15 iterations for K, 5 for G
-    and skip B. Setting to zero effectively disables solving for that term
-    and can be used in conjunction with iterpolation.
+    dtype: List[int]
+    default: [25]
+    info:
+      Specifies the iterations to be performed per gain term. This argument
+      expects a list as long or longer than solver.terms. If solver.terms
+      was given as [K,G,B], an iteration recipe of [20,10,5] would do 20
+      iterations for K, 10 for G and 5 for B. To loop over the gains multiple
+      times, use a longer list e.g. [20,10,5,15,5,0] would do the same as
+      the first example but then do an additional 15 iterations for K, 5 for
+      G and skip B. Setting to zero effectively disables solving for that
+      term and can be used in conjunction with iterpolation.
+
   propagate_flags:
-    Controls whether gain flags/flags raised inside the solver are propagated
-    and ultimately written to the FLAG column. This should almost always be
-    enabled so that data associated with diverging gains is properly flagged.
+    dtype: bool
+    default: True
+    info:
+      Controls whether gain flags/flags raised inside the solver are
+      propagated and ultimately written to the FLAG column. This should
+      almost always be enabled so that data associated with diverging gains
+      is properly flagged.
+
   robust:
-    Enable robust reweighting in solvers. Note that this only works when the
-    solver.iter_recipe loops through the chain multiple times. The reweighting
-    step only happens once per traversal of the chain.
+    dtype: bool
+    default: False
+    info:
+      Enable robust reweighting in solvers. Note that this only works when
+      the solver.iter_recipe loops through the chain multiple times. The
+      reweighting step only happens once per traversal of the chain.
+
   threads:
-    Number of Numba threads per Dask thread (enables nested parallelism) to
-    be used when running the solvers. The total number of threads used will be
-    dask.threads*solver.threads; if this product exceeds the number of
-    available threads, performance will suffer.
-  convergence_criteria:
-    The change in the value of the gain below which it considered to have
-    converged. Set to zero to iterate for the number of interations specified
-    in solver.iter_recipe.
+    dtype: int
+    default: 1
+    info:
+      Number of Numba threads per Dask thread (enables nested parallelism) to
+      be used when running the solvers. The total number of threads used will be
+      dask.threads*solver.threads; if this product exceeds the number of
+      available threads, performance will suffer.
+
   convergence_fraction:
-    The fraction of gain values which must converge before a solver will exit
-    prematurely.
+    dtype: float
+    default: 0.99
+    info:
+      The fraction of gain values which must converge before a solver will
+      exit prematurely.
+
+  convergence_criteria:
+    dtype: float
+    default: 1e-6
+    info:
+      The change in the value of the gain below which it considered to have
+      converged. Set to zero to iterate for the number of interations
+      specified in solver.iter_recipe.
+
   reference_antenna:
-    A reference antenna to use for terms which require one. This is shared by
-    all terms and currently only used for delay estimates - QuartiCal does not
-    guarantee zero phase on an antenna. Specify as the integer index of the
-    antenna - antenna names are not currently supported.
+    dtype: int
+    default: 0
+    info:
+      A reference antenna to use for terms which require one. QuartiCal will
+      also guarantee zero phase on the specified antenna for diagonal terms.
+      Specify as the integer index of the antenna - antenna names are not
+      currently supported.
 
 dask:
   threads:
-    Number of threads to use in the dask scheduler. Setting to zero (the
-    default) will use all available resources.
+    dtype: Optional[int]
+    info:
+      Number of threads to use in the dask scheduler. Setting to zero (the
+      default) will use all available resources.
+
   workers:
-    Number of workers to use in the dask distributed scheduler. Advanced users
-    only.
+    dtype: int
+    default: 1
+    info:
+      Number of workers to use in the dask distributed scheduler. Advanced
+      users only.
+
   address:
-    Distributed scheduler address.
-  scheduler:
-    Which dask scheduler to use. The default, threads, is the most appropriate
-    for non-cluster use.
+    dtype: Optional[str]
+    info:
+      Distributed scheduler address.
 
-gain:
-  type:
-    Type of gain to solve for.
-  solve_per:
-    Determines whether this term should be solved per antenna (conventional)
-    or over the entire array (doesn't vary with antenna).
-  direction_dependent:
-    Determines whether this term is treated as direction dependent.
-  time_interval:
-    Number of timeslots/amount of time to include in a single solution.
-    Specify as an integer number of timeslots, or a value with a unit
-    (e.g. '300s'). 0 means use full time axis.
-  freq_interval:
-    Number of channels/bandwidth to include in a single solution. Specify as
-    an integer number of channels, or a value with a unit (e.g. '128MHz').
-    0 means use full frequency axis.
-  respect_scan_boundaries:
-    Determines whether solution intervals may span multiple scans. This only
-    works when input_ms.group_by does not include SCAN_NUMBER. Can be used
-    in conjunction with time_interval to solve a term per scan even when
-    data is not partitioned by scan (by setting this to True and
-    time_interval to 0).
-  initial_estimate:
-    Controls whether or not a term will be populated with an initial
-    estimiate where applicable. Currently only supported for delay terms.
-  load_from:
-    Load solutions from given database.
-  interp_mode:
-    Set interpolation mode.
-  interp_method:
-    Set interpolation method.
-  #   exclude-directions:
-  #       nargs: +
-  #       type: int
-  #       help: For direction-dependent terms, makes the listed directions
-  #             (specified by index) non-solvable. -1 disables.
-  #       default: -1
+  scheduler:
+    default: threads
+    choices: ["threads", "single-threaded", "distributed"]
+    info:
+      Which dask scheduler to use. The default, threads, is the most
+      appropriate for non-cluster use.
```

### Comparing `quartical-0.1.9/quartical/config/internal.py` & `quartical-0.2.0/quartical/config/internal.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,37 @@
-from dataclasses import make_dataclass
-from quartical.config.external import Gain
 from daskms.fsspec_store import DaskMSStore
+from quartical.gains import TERM_TYPES
 
 
 def gains_to_chain(opts):
 
     terms = opts.solver.terms
 
-    Chain = make_dataclass(
-        "Chain",
-        [(t, Gain, Gain()) for t in terms]
-    )
-
-    chain = Chain()
-
-    for t in terms:
-        setattr(chain, t, getattr(opts, t))
+    # NOTE: Currently a simple list, but we could also implement an object.
+    chain = [
+        TERM_TYPES[getattr(opts, t).type](t, getattr(opts, t)) for t in terms
+    ]
 
     return chain
 
 
-def yield_from(obj, flds=None, name=True):
-
-    flds = (flds,) if isinstance(flds, str) else flds
-
-    for k in obj.__dataclass_fields__.keys():
-        if flds is None:
-            yield k
-        elif name:
-            yield (k, *(getattr(getattr(obj, k), fld) for fld in flds))
-        else:
-            yield (*(getattr(getattr(obj, k), fld) for fld in flds),)
-
-
 def additional_validation(config):
 
     chain = gains_to_chain(config)
 
     store = DaskMSStore(config.output.gain_directory)
 
     if store.exists() and not config.output.overwrite:
         raise FileExistsError(f"{store.url} already exists. Specify "
                               f"output.overwrite=1 to suppress this "
                               f"error and overwrite files/folders.")
     elif store.exists():
         store.rm(recursive=True)
 
-    load_stores = \
-        [DaskMSStore(lf) for _, lf in yield_from(chain, "load_from") if lf]
+    load_stores = [DaskMSStore(t.load_from) for t in chain if t.load_from]
 
     msg = (
         f"Output directory {str(store.url)} contains terms which will be "
         f"loaded/interpolated. This is not supported. Please specify a "
         f"different output directory."
     )
```

### Comparing `quartical-0.1.9/quartical/config/parser.py` & `quartical-0.2.0/quartical/config/parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 import sys
 import os
 from loguru import logger
 from ruamel.yaml import round_trip_dump
 from omegaconf import OmegaConf as oc
 from quartical.config.external import finalize_structure
 from quartical.config.internal import additional_validation
+from omegaconf.errors import ConfigKeyError, ValidationError
 
 
 def create_user_config():
     """Creates a blank .yaml file with up-to-date field names and defaults."""
 
-    if not sys.argv[-1].endswith("goquartical-config"):
-        config_file_path = sys.argv[-1]
-    else:
-        config_file_path = "user_config.yaml"
+    config_file_path = (
+        "user_config.yaml" if len(sys.argv) == 1 else sys.argv[-1]
+    )
 
     logger.info("Output config file path: {}", config_file_path)
 
     # We add this so that the user config comes out with a gain field.
     additional_config = [oc.from_dotlist(["solver.terms=['G']"])]
 
     FinalConfig = finalize_structure(additional_config)
@@ -30,16 +30,17 @@
             oc.to_container(config),
             outfile,
             default_flow_style=False,
             width=60,
             indent=2
         )
 
-    logger.success("{} successfully generated. Go forth and calibrate!",
-                   config_file_path)
+    logger.success(
+        f"{config_file_path} successfully generated. Go forth and calibrate!"
+    )
 
     return
 
 
 def log_final_config(config, config_files=[]):
     """Logs the final state of the configuration object.
 
@@ -59,42 +60,39 @@
         columns, _ = os.get_terminal_size(0)
     else:
         columns = 80  # Fall over to some sensible default.
 
     for cf in config_files:
         logger.info(f"Using user-defined config file: {cf}")
 
-    log_message = "Final configuration state:"
-
-    current_section = None
+    log_message = "Final configuration state:\n\n"
 
     for section, options in config.items():
 
-        if current_section != section:
-            log_message += "" if current_section is None \
-                else "<blue>{0:-^{1}}</blue>\n".format("", columns)
-            log_message += "\n<blue>{0:-^{1}}</blue>\n".format(
-                section, columns)
-            current_section = section
+        log_message += f"<blue>{section:-^{columns}}</blue>\n"
 
         maxlen = max(map(len, [f"{section}.{key}" for key in options.keys()]))
 
         for key, value in options.items():
             option = f"{section}.{key}"
             msg = f"{option:<{maxlen + 1}}{str(value):>{columns - maxlen - 1}}"
 
             if len(msg) > columns:
-                split = [msg[i:i+columns] for i in range(0, len(msg), columns)]
 
-                msg = "\n".join((split[0],
-                                *[f"{s:>{columns}}" for s in split[1:]]))
+                split = [
+                    msg[i:i + columns] for i in range(0, len(msg), columns)
+                ]
+
+                msg = "\n".join(
+                    (split[0], *[f"{s:>{columns}}" for s in split[1:]])
+                )
 
             log_message += msg + "\n"
 
-    log_message += "<blue>{0:-^{1}}</blue>".format("", columns)
+        log_message += f"<blue>{'':-^{columns}}</blue>\n\n"
 
     logger.opt(ansi=True).info(log_message)
 
 
 def parse_inputs(bypass_sysargv=None):
     """Combines command line and config files to produce a config object."""
 
@@ -117,15 +115,31 @@
     yml_config = [oc.load(file) for file in config_files]
     cli_config = [] if bypass_sysargv else [oc.from_cli()]
     additional_config = [*yml_config, *cli_config]
 
     # Merge all configuration - priority is file1 < file2 < ... < cli.
     FinalConfig = finalize_structure(additional_config)
     config = oc.structured(FinalConfig)
-    config = oc.merge(config, *additional_config)
+
+    try:
+        config = oc.merge(config, *additional_config)
+    except ConfigKeyError as error:
+        raise ValueError(
+            f"User has specified an unrecognised parameter: {error.full_key}. "
+            f"This often indicates a simple typo or the use of a deprecated "
+            f"parameter. Please use 'goquartical help' to confirm that the "
+            f"parameter exists."
+        )
+    except ValidationError as error:
+        raise ValueError(
+            f"The value specified for {error.full_key} was not understood. "
+            f"This often means that the type of the argument was incorrect. "
+            f"Please use 'goquartical help' to check for the expected type "
+            f"and pay particular attention to parameters which expect lists."
+        )
 
     # Log the final state of the configuration object so that users are aware
     # of what the ultimate configuration was.
 
     config_obj = oc.to_object(config)  # Ensures post_init methods are run.
 
     additional_validation(config_obj)
```

### Comparing `quartical-0.1.9/quartical/config/preprocess.py` & `quartical-0.2.0/quartical/config/preprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,27 +19,38 @@
 
 @dataclass
 class Recipe:
     ingredients: Ingredients
     instructions: Dict[int, List[Any]]
 
 
+@dataclass
+class IdentityRecipe(Recipe):
+    pass
+
+
 def transcribe_recipe(user_recipe):
     """Interpret the model recipe string.
 
     Given the config object, create an internal recipe implementing the user
     specified recipe.
 
     Args:
         model_opts: An ModelInputs configuration object.
 
     Returns:
         model_Recipe: A Recipe object.
     """
 
+    if user_recipe is None:
+        logger.warning(
+            "input_model.recipe was not supplied. Assuming identity model."
+        )
+        return IdentityRecipe(Ingredients(set(), set()), dict())
+
     model_columns = set()
     sky_models = set()
     instructions = {}
 
     # Strip accidental whitepsace from input recipe and splits on ":".
     input_recipes = user_recipe.replace(" ", "").split(":")
```

### Comparing `quartical-0.1.9/quartical/data_handling/angles.py` & `quartical-0.2.0/quartical/data_handling/angles.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import casacore.quanta as pq
 
 from daskms import xds_from_storage_table
 import dask.array as da
 import threading
 from dask.graph_manipulation import clone
 import xarray
-from numba import generated_jit
+from numba import njit
+from numba.extending import overload
+from quartical.utils.numba import coerce_literal, JIT_OPTIONS
 from quartical.utils.dask import blockwise_unique
 import quartical.gains.general.factories as factories
-from quartical.utils.numba import coerce_literal
 
 
 # Create thread local storage for the measures server. TODO: This works for
 # Simon but I think it may break things for me. Investigate.
 _thread_local = threading.local()
 
 
@@ -199,41 +200,68 @@
             _, utime_ind = blockwise_unique(time_col,
                                             chunks=(utime_chunks,),
                                             return_inverse=True)
 
             # Negate the angles if the desired output is a derotation.
             parangles = -parangles if derotate else parangles
 
-            rot_vars[data_var_name] = da.blockwise(py_apply_parangle_rot,
-                                                   "rfc",
-                                                   data_var, "rfc",
-                                                   parangles, "ra2",
-                                                   utime_ind, "r",
-                                                   ant1_col, "r",
-                                                   ant2_col, "r",
-                                                   corr_mode, None,
-                                                   feed_type, None,
-                                                   align_arrays=False,
-                                                   concatenate=True,
-                                                   dtype=data_var.dtype)
+            rot_vars[data_var_name] = da.blockwise(
+                apply_parangle, "rfc",
+                data_var, "rfc",
+                parangles, "ra2",
+                utime_ind, "r",
+                ant1_col, "r",
+                ant2_col, "r",
+                corr_mode, None,
+                feed_type, None,
+                align_arrays=False,
+                concatenate=True,
+                dtype=data_var.dtype
+            )
 
         output_data_xds_list.append(
             xds.assign({n: ((xds[n].dims), v) for n, v in rot_vars.items()}))
 
     return output_data_xds_list
 
 
-def py_apply_parangle_rot(data_col, parangles, utime_ind, ant1_col, ant2_col,
-                          corr_mode, feed_type):
-    """Wrapper for numba function to ensure pickling works."""
-    return nb_apply_parangle_rot(data_col, parangles, utime_ind, ant1_col,
-                                 ant2_col, corr_mode, feed_type)
+@njit(**JIT_OPTIONS)
+def apply_parangle(
+    data_col,
+    parangles,
+    utime_ind,
+    ant1_col,
+    ant2_col,
+    corr_mode,
+    feed_type
+):
+    return apply_parangle_impl(
+        data_col,
+        parangles,
+        utime_ind,
+        ant1_col,
+        ant2_col,
+        corr_mode,
+        feed_type
+    )
+
+
+def apply_parangle_impl(
+    data_col,
+    parangles,
+    utime_ind,
+    ant1_col,
+    ant2_col,
+    corr_mode,
+    feed_type
+):
+    return NotImplementedError
 
 
-@generated_jit(nopython=True, nogil=True, fastmath=True, cache=True)
+@overload(apply_parangle_impl, jit_options=JIT_OPTIONS)
 def nb_apply_parangle_rot(data_col, parangles, utime_ind, ant1_col, ant2_col,
                           corr_mode, feed_type):
 
     coerce_literal(nb_apply_parangle_rot, ["corr_mode", "feed_type"])
 
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
```

### Comparing `quartical-0.1.9/quartical/data_handling/bda.py` & `quartical-0.2.0/quartical/data_handling/bda.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             and merged data.
         utime_per_xds: List of number of unique times per xds.
     """
 
     # If WEIGHT_SPECTRUM is not in use, BDA data makes no sense. TODO: This is
     # not strictly true. Any weight column with a frequency axis is valid.
     if weight_column != "WEIGHT_SPECTRUM":
-        raise ValueError("--input-ms-weight column must be "
+        raise ValueError("input_ms.weight_column must be "
                          "WEIGHT_SPECTRUM for BDA data.")
 
     # Figure out the highest frequency resolution and its DDID.
     spw_dims = {i: xds.dims["chan"] for i, xds in enumerate(spw_xds_list)}
     max_nchan_ddid = max(spw_dims, key=spw_dims.get)
     max_nchan = spw_dims[max_nchan_ddid]
 
@@ -240,15 +240,15 @@
                     data = data.sum(axis=chan_ind + 1)/(nchan//ref_nchan)
                 elif np.issubdtype(scdtype, np.integer):
                     # Corresponds to BITFLAG style column. Bitwise or.
                     data = data.map_blocks(
                         lambda d, a: np.bitwise_or.reduce(d, axis=a),
                         chan_ind + 1,
                         drop_axis=chan_ind + 1)
-                elif np.issubdtype(scdtype, np.bool):
+                elif np.issubdtype(scdtype, bool):
                     # Corresponds to FLAG style column.
                     data = data.any(axis=chan_ind + 1)
 
                 bda_xds = bda_xds.assign({col_name: (col.dims, data)})
 
             else:
                 bda_xds = bda_xds.assign({col_name: (col.dims, col.data)})
```

### Comparing `quartical-0.1.9/quartical/data_handling/chunking.py` & `quartical-0.2.0/quartical/data_handling/chunking.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,24 +43,28 @@
     zipper = zip(row_chunking_per_xds, chan_chunking_per_xds)
     chunking_per_data_xds = [{"row": r, "chan": c} for r, c in zipper]
 
     chunking_per_spw_xds = \
         [{"__row__": 1, "chan": c} for c in chan_chunking_per_spw.values()]
 
     if compute:
-        return da.compute(utime_chunking_per_xds,
-                          chunking_per_data_xds,
-                          chunking_per_spw_xds)
+        return da.compute(
+            utime_chunking_per_xds,
+            chunking_per_data_xds,
+            chunking_per_spw_xds
+        )
     else:
         utime_chunking_per_xds, chunking_per_data_xds, chunking_per_spw_xds
 
 
-def chan_chunking(spw_xds_list,
-                  freq_chunk,
-                  compute=True):
+def chan_chunking(
+    spw_xds_list,
+    freq_chunk,
+    compute=True
+):
     """Compute frequency chunks for the input data.
 
     Given a list of indexing xds's, and a list of spw xds's, determines how to
     chunk the data in frequency given the chunking parameters.
 
     Args:
         indexing_xds_list: List of xarray.dataset objects contatining indexing
@@ -107,19 +111,25 @@
 
         else:
 
             def integer_chunking(chan_widths, freq_chunk):
 
                 n_chan = chan_widths.size
                 freq_chunk = freq_chunk or n_chan  # Catch zero case.
-                chunks = (freq_chunk,) * (n_chan // freq_chunk)
-                remainder = n_chan - sum(chunks)
-                chunks += (remainder,) if remainder else ()
 
-                return np.array(chunks, dtype=np.int32)
+                chunk_starts = np.arange(0, n_chan, freq_chunk)
+
+                chunks = np.array(
+                    [
+                        freq_chunk if i + freq_chunk < n_chan else n_chan - i
+                        for i in chunk_starts
+                    ]
+                )
+
+                return chunks.astype(np.int32)
 
             chunking = da.map_blocks(integer_chunking,
                                      xds.CHAN_WIDTH.data[0],
                                      freq_chunk,
                                      chunks=((np.nan,),),
                                      dtype=np.int32)
 
@@ -128,17 +138,19 @@
 
     if compute:
         return da.compute(chan_chunking_per_spw)[0]
     else:
         return chan_chunking_per_spw
 
 
-def row_chunking(indexing_xds_list,
-                 time_chunk,
-                 compute=True):
+def row_chunking(
+    indexing_xds_list,
+    time_chunk,
+    compute=True
+):
     """Compute time and frequency chunks for the input data.
 
     Given a list of indexing xds's, and a list of spw xds's, determines how to
     chunk the data given the chunking parameters.
 
     Args:
         indexing_xds_list: List of xarray.dataset objects contatining indexing
@@ -146,34 +158,32 @@
         time_chunk: Int or float specifying chunking.
         compute: Boolean indicating whether or not to compute the result.
 
     Returns:
         A tuple of utime_chunking_per_xds and row_chunking_per_xds which
         describe the chunking of the data.
     """
-    # row_chunks is a list of dictionaries containing row chunks per data set.
 
     row_chunking_per_xds = []
     utime_chunking_per_xds = []
 
     for xds in indexing_xds_list:
 
         # If the chunking interval is a float after preprocessing, we are
-        # dealing with a duration rather than a number of intervals. TODO:
-        # Need to take resulting chunks and reprocess them based on chunk-on
-        # columns and jumps.
+        # dealing with a duration rather than a number of intervals.
 
         # TODO: BDA will assume no chunking, and in general we can skip this
         # bit if the row axis is unchunked.
 
         if isinstance(time_chunk, float):
 
             def interval_chunking(time_col, interval_col, time_chunk):
+                """Given a time column, figure out interval chunking."""
 
-                utimes, uinds, ucounts = \
+                _, uinds, ucounts = \
                     np.unique(time_col, return_counts=True, return_index=True)
                 cumulative_interval = np.cumsum(interval_col[uinds])
                 cumulative_interval -= cumulative_interval[0]
                 chunk_map = \
                     (cumulative_interval // time_chunk).astype(np.int32)
 
                 _, utime_chunks = np.unique(chunk_map, return_counts=True)
@@ -181,48 +191,55 @@
                 chunk_starts = np.zeros(utime_chunks.size, dtype=np.int32)
                 chunk_starts[1:] = np.cumsum(utime_chunks)[:-1]
 
                 row_chunks = np.add.reduceat(ucounts, chunk_starts)
 
                 return np.vstack((utime_chunks, row_chunks)).astype(np.int32)
 
-            chunking = da.map_blocks(interval_chunking,
-                                     xds.TIME.data,
-                                     xds.INTERVAL.data,
-                                     time_chunk,
-                                     chunks=((2,), (np.nan,)),
-                                     dtype=np.int32)
+            chunking = da.map_blocks(
+                interval_chunking,
+                xds.TIME.data,
+                xds.INTERVAL.data,
+                time_chunk,
+                chunks=((2,), (np.nan,)),
+                dtype=np.int32
+            )
 
         else:
 
             def integer_chunking(time_col, time_chunk):
+                """Given a time column, figure out integer chunking."""
 
                 utimes, ucounts = np.unique(time_col, return_counts=True)
                 n_utime = utimes.size
-                time_chunk = time_chunk or n_utime  # Catch time_chunk == 0.
-
-                utime_chunks = [time_chunk] * (n_utime // time_chunk)
-                last_chunk = n_utime % time_chunk
-
-                utime_chunks += [last_chunk] if last_chunk else []
-                utime_chunks = np.array(utime_chunks)
+                time_chunk = time_chunk or n_utime  # Catch 0.
 
                 chunk_starts = np.arange(0, n_utime, time_chunk)
 
+                utime_chunks = np.array(
+                    [
+                        time_chunk if i + time_chunk < n_utime else n_utime - i
+                        for i in chunk_starts
+                    ]
+                )
+
                 row_chunks = np.add.reduceat(ucounts, chunk_starts)
 
                 return np.vstack((utime_chunks, row_chunks)).astype(np.int32)
 
-            chunking = da.map_blocks(integer_chunking,
-                                     xds.TIME.data,
-                                     time_chunk,
-                                     chunks=((2,), (np.nan,)),
-                                     dtype=np.int32)
+            chunking = da.map_blocks(
+                integer_chunking,
+                xds.TIME.data,
+                time_chunk,
+                chunks=((2,), (np.nan,)),
+                dtype=np.int32
+            )
 
         # We use delayed to convert to tuples and satisfy daskms/dask.
+        # TODO: Why was this necessary and can we avoid it?
         utime_per_chunk = dd(tuple)(chunking[0, :])
         row_chunks = dd(tuple)(chunking[1, :])
 
         utime_chunking_per_xds.append(utime_per_chunk)
         row_chunking_per_xds.append(row_chunks)
 
     if compute:
```

### Comparing `quartical-0.1.9/quartical/data_handling/model_handler.py` & `quartical-0.2.0/quartical/data_handling/model_handler.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 # -*- coding: utf-8 -*-
 import dask.array as da
+import numpy as np
 from quartical.data_handling.predict import predict
 from quartical.data_handling.angles import apply_parangles
+from quartical.config.preprocess import IdentityRecipe, Ingredients
+from quartical.utils.array import flat_ident_like
 from loguru import logger  # noqa
 
 
-def add_model_graph(data_xds_list, parangle_xds_list, model_vis_recipe,
-                    ms_path, model_opts):
+def add_model_graph(
+    data_xds_list,
+    parangle_xds_list,
+    model_vis_recipe,
+    ms_path,
+    model_opts
+):
     """Creates the graph necessary to produce a model per xds.
 
     Given a list of input xarray data sets and the options, constructs a graph
     in accordance with the internal model recipe. This can produce
     direction-dependent models using the recipe syntax.
 
     Args:
@@ -32,14 +40,21 @@
         predict_schemes = predict(data_xds_list,
                                   model_vis_recipe,
                                   ms_path,
                                   model_opts)
     else:
         predict_schemes = [{}]*len(data_xds_list)
 
+    # Special case: in the event that we have an IdentityRecipe, modify the
+    # datasets and model appropriately.
+    if isinstance(model_vis_recipe, IdentityRecipe):
+        data_xds_list, model_vis_recipe = assign_identity_model(data_xds_list)
+
+    model_columns = model_vis_recipe.ingredients.model_columns
+
     # NOTE: At this point we are ready to construct the model array. First,
     # however, we need to apply parallactic angle corrections to model columns
     # which require them. P Jones is applied to predicted components
     # internally, so we only need to consider model columns for now.
 
     n_corr = {xds.dims["corr"] for xds in data_xds_list}.pop()
 
@@ -50,15 +65,14 @@
         # it is not reversible. We support it for input models but warn the
         # user that it is not a good idea.
         if n_corr != 4:
             logger.warning(
                 "input_model.apply_p_jones is not recommended for data with "
                 "less than four correlations. Proceed with caution."
             )
-        model_columns = model_vis_recipe.ingredients.model_columns
         data_xds_list = apply_parangles(data_xds_list,
                                         parangle_xds_list,
                                         model_columns)
 
     # Initialise a list to contain the xdss after the model data has been
     # assigned.
 
@@ -131,14 +145,74 @@
 
         n_dir = len(model)  # The number of terms is the number of directions.
 
         # This creates the direction axis by stacking the model terms. The
         # rechunking is necessary to ensure the solver gets appropriate blocks.
         model = da.stack(model, axis=2).rechunk({2: n_dir})
 
-        modified_xds = xds.assign(
+        # Get rid of model columns which are not used after this point.
+        modified_xds = xds.drop_vars(model_columns)
+
+        modified_xds = modified_xds.assign(
             {"MODEL_DATA": (("row", "chan", "dir", "corr"), model)}
         )
 
         model_xds_list.append(modified_xds)
 
     return model_xds_list
+
+
+def assign_identity_model(data_xds_list):
+    """Given dataset list, creates recipe and assigns an identity model.
+
+    This is a special case where we have no input model and simply want to use
+    the identity. This is common when constraining phase solutions on a
+    calibrator.
+
+    Args:
+        data_xds_list: A list of xarray.Datasets objects containing MS data.
+
+    Returns:
+        data_xds_list: A list of xarray.Datasets with new model assigned.
+        recipe: A modified Recipe object consistent with this case.
+    """
+
+    ingredients = Ingredients({"__IDENT__"}, set())
+    instructions = {0: ["__IDENT__"]}
+
+    recipe = IdentityRecipe(ingredients, instructions)
+
+    model_dims = [
+        (
+            xds.dims['row'],
+            xds.dims['chan'],
+            xds.dims['corr']
+        )
+        for xds in data_xds_list
+    ]
+
+    model_chunks = [
+        (
+            xds.chunks['row'],
+            xds.chunks['chan'],
+            xds.chunks['corr']
+        )
+        for xds in data_xds_list
+    ]
+
+    data_xds_list = [
+        xds.assign(
+            {
+                "__IDENT__": (
+                    ("row", "chan", "corr"),
+                    flat_ident_like(
+                        da.empty(dims, chunks=chunks, dtype=np.complex64)
+                    )
+                )
+            }
+        )
+        for xds, dims, chunks in zip(
+            data_xds_list, model_dims, model_chunks
+        )
+    ]
+
+    return data_xds_list, recipe
```

### Comparing `quartical-0.1.9/quartical/data_handling/ms_handler.py` & `quartical-0.2.0/quartical/data_handling/ms_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,31 +79,33 @@
     columns += (ms_opts.data_column,)
     columns += (ms_opts.weight_column,) if ms_opts.weight_column else ()
     columns += (ms_opts.sigma_column,) if ms_opts.sigma_column else ()
     columns += \
         ("SCAN_NUMBER",) if "SCAN_NUMBER" not in ms_opts.group_by else ()
     columns += (*model_columns,)
 
-    available_columns = list(xds_from_storage_ms(ms_opts.path)[0].keys())
-    assert all(c in available_columns for c in columns), \
-           f"One or more columns in: {columns} is not present in the data."
-
     schema = {cn: {'dims': ('chan', 'corr')} for cn in model_columns}
 
     known_weight_cols = ("WEIGHT", "WEIGHT_SPECTRUM")
     if ms_opts.weight_column not in known_weight_cols:
         schema[ms_opts.weight_column] = {'dims': ('chan', 'corr')}
 
-    data_xds_list = xds_from_storage_ms(
-        ms_opts.path,
-        columns=columns,
-        index_cols=("TIME",),
-        group_cols=ms_opts.group_by,
-        chunks=chunking_per_data_xds,
-        table_schema=["MS", {**schema}])
+    try:
+        data_xds_list = xds_from_storage_ms(
+            ms_opts.path,
+            columns=columns,
+            index_cols=("TIME",),
+            group_cols=ms_opts.group_by,
+            chunks=chunking_per_data_xds,
+            table_schema=["MS", {**schema}]
+        )
+    except RuntimeError as e:
+        raise RuntimeError(
+            f"Invalid/missing column specified. Underlying error: {e}."
+        ) from e
 
     spw_xds_list = xds_from_storage_table(
         ms_opts.path + "::SPECTRAL_WINDOW",
         group_cols=["__row__"],
         columns=["CHAN_FREQ", "CHAN_WIDTH"],
         chunks=chunking_per_spw_xds
     )
@@ -135,39 +137,49 @@
         # Add the actual channel frequecies to the xds - this is in preparation
         # for solvers which require this information. Also adds the antenna
         # names which will be useful when reference antennas are required.
 
         chan_freqs = clone(spw_xds_list[xds.DATA_DESC_ID].CHAN_FREQ.data)
         chan_widths = clone(spw_xds_list[xds.DATA_DESC_ID].CHAN_WIDTH.data)
 
-        _xds = _xds.assign({"CHAN_FREQ": (("chan",), chan_freqs[0]),
-                            "CHAN_WIDTH": (("chan",), chan_widths[0])})
+        _xds = _xds.assign(
+            {
+                "CHAN_FREQ": (("chan",), chan_freqs[0]),
+                "CHAN_WIDTH": (("chan",), chan_widths[0])
+            }
+        )
 
         # Add an attribute to the xds on which we will store the names of
         # fields which must be written to the MS. Also add the attribute which
         # stores the unique time chunking per xds. We have to convert the
         # chunking to python integers to avoid problems with serialization.
 
-        utime_chunks = tuple(map(int, utime_chunking_per_data_xds[xds_ind]))
+        utime_chunks = utime_chunking_per_data_xds[xds_ind]
         field_id = getattr(xds, "FIELD_ID", None)
         field_name = "UNKNOWN" if field_id is None else field_names[field_id]
 
-        _xds = _xds.assign_attrs({"UTIME_CHUNKS": utime_chunks,
-                                  "FIELD_NAME": field_name})
+        _xds = _xds.assign_attrs(
+            {
+                "UTIME_CHUNKS": utime_chunks,
+                "FIELD_NAME": field_name
+            }
+        )
 
         _data_xds_list.append(_xds)
 
     data_xds_list = _data_xds_list
 
     # Filter out fields/ddids which we are not interested in. Also select out
     # correlations. TODO: Does this type of selection/filtering belong here?
 
-    data_xds_list = filter_xds_list(data_xds_list,
-                                    ms_opts.select_fields,
-                                    ms_opts.select_ddids)
+    data_xds_list = filter_xds_list(
+        data_xds_list,
+        ms_opts.select_fields,
+        ms_opts.select_ddids
+    )
 
     # TODO: Do we want to select on index or corr_type?
     if ms_opts.select_corr:
         try:
             data_xds_list = [xds.isel(corr=ms_opts.select_corr)
                              for xds in data_xds_list]
         except IndexError:
```

### Comparing `quartical-0.1.9/quartical/data_handling/predict.py` & `quartical-0.2.0/quartical/data_handling/predict.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,18 @@
             logger.info(f"Setting the default reference frequency for "
                         f"{sky_model_name} to {fallback_freq0}.")
 
         for source in sources:
 
             tagged = any([source.getTag(tag) for tag in sky_model_tags])
 
-            parent_group = source.getTag("cluster") if tagged else "DIE"
+            if tagged:
+                parent_group = source.getTag("cluster") or source.name
+            else:
+                parent_group = "DIE"
 
             ra = source.pos.ra
             dec = source.pos.dec
             typecode = source.typecode.lower()
             flux = [getattr(source.flux, sto, 0) for sto in "IQUV"]
             spectrum = getattr(source, "spectrum", _empty_spectrum)
```

### Comparing `quartical-0.1.9/quartical/executor.py` & `quartical-0.2.0/quartical/executor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -*- coding: utf-8 -*-
-# Sets up logger - hereafter import logger from Loguru.
 from contextlib import ExitStack
 import sys
 from loguru import logger
 import dask
 from dask.distributed import Client, LocalCluster
 import time
 from quartical.config import parser, preprocess, helper, internal
@@ -11,22 +10,20 @@
 from quartical.data_handling.ms_handler import (read_xds_list,
                                                 write_xds_list,
                                                 preprocess_xds_list,
                                                 postprocess_xds_list)
 from quartical.data_handling.model_handler import add_model_graph
 from quartical.data_handling.angles import make_parangle_xds_list
 from quartical.calibration.calibrate import add_calibration_graph
-from quartical.statistics.statistics import (make_stats_xds_list,
-                                             assign_presolve_chisq,
-                                             assign_postsolve_chisq)
-from quartical.statistics.logging import (embed_stats_logging,
-                                          log_summary_stats)
+from quartical.statistics.statistics import make_stats_xds_list
+from quartical.statistics.logging import log_summary_stats
 from quartical.flagging.flagging import finalise_flags, add_mad_graph
 from quartical.scheduling import install_plugin
 from quartical.gains.datasets import write_gain_datasets
+from quartical.gains.baseline import write_baseline_datasets
 from quartical.utils.dask import compute_context
 
 
 @logger.catch(onerror=lambda _: sys.exit(1))
 def execute():
     with ExitStack() as stack:
         _execute(stack)
@@ -43,15 +40,15 @@
     # Split out all the configuration objects. Mitigates god-object problems.
     ms_opts = opts.input_ms
     model_opts = opts.input_model
     solver_opts = opts.solver
     output_opts = opts.output
     mad_flag_opts = opts.mad_flags
     dask_opts = opts.dask
-    chain_opts = internal.gains_to_chain(opts)  # Special handling.
+    chain = internal.gains_to_chain(opts)  # Special handling.
 
     # Init the logging proxy - an object which helps us ensure that logging
     # works for both threads an processes. It is easily picklable.
 
     time_str = time.strftime("%Y%m%d_%H%M%S")
     proxy_logger = ProxyLogger(
         output_opts.log_directory,
@@ -108,34 +105,39 @@
 
     # Make a list of datasets containing the parallactic angles as these
     # can be expensive to compute and may be used several times. NOTE: At
     # present, these also include the effect of the receptor angles.
     parangle_xds_list = make_parangle_xds_list(ms_opts.path, data_xds_list)
 
     # A list of xdss onto which appropriate model data has been assigned.
-    data_xds_list = add_model_graph(data_xds_list,
-                                    parangle_xds_list,
-                                    model_vis_recipe,
-                                    ms_opts.path,
-                                    model_opts)
+    data_xds_list = add_model_graph(
+        data_xds_list,
+        parangle_xds_list,
+        model_vis_recipe,
+        ms_opts.path,
+        model_opts
+    )
 
     stats_xds_list = make_stats_xds_list(data_xds_list)
-    stats_xds_list = assign_presolve_chisq(data_xds_list, stats_xds_list)
 
     # Adds the dask graph describing the calibration of the data. TODO:
     # This call has excess functionality now. Split out mapping and outputs.
-    gain_xds_lod, net_xds_lod, data_xds_list = add_calibration_graph(
+    cal_outputs = add_calibration_graph(
         data_xds_list,
+        stats_xds_list,
         solver_opts,
-        chain_opts,
+        chain,
         output_opts
     )
 
-    stats_xds_list = assign_postsolve_chisq(data_xds_list, stats_xds_list)
-    stats_xds_list = embed_stats_logging(stats_xds_list)
+    (gain_xds_lod,
+     net_xds_lod,
+     data_xds_list,
+     stats_xds_list,
+     bl_corr_xds_list) = cal_outputs
 
     if mad_flag_opts.enable:
         data_xds_list = add_mad_graph(data_xds_list, mad_flag_opts)
 
     data_xds_list = finalise_flags(data_xds_list)
 
     # This will apply the inverse of P-Jones but can also be extended.
@@ -145,30 +147,34 @@
 
     ms_writes = write_xds_list(data_xds_list,
                                ref_xds_list,
                                ms_opts.path,
                                output_opts)
 
     gain_writes = write_gain_datasets(gain_xds_lod,
-                                      net_xds_lod,
-                                      output_opts)
+                                      output_opts.gain_directory,
+                                      net_xds_lod)
+
+    bl_corr_writes = write_baseline_datasets(bl_corr_xds_list,
+                                             output_opts)
 
     logger.success("{:.2f} seconds taken to build graph.", time.time() - t0)
 
     logger.info("Computation starting. Please be patient - log messages will "
                 "only appear per completed chunk.")
 
     t0 = time.time()
 
     with compute_context(dask_opts, output_opts, time_str):
 
-        _, _, stats_xds_list = dask.compute(
+        _, _, stats_xds_list, _ = dask.compute(
             ms_writes,
             gain_writes,
             stats_xds_list,
+            bl_corr_writes,
             num_workers=dask_opts.threads,
             optimize_graph=True,
             scheduler=dask_opts.scheduler
         )
 
     logger.success("{:.2f} seconds taken to execute graph.", time.time() - t0)
```

### Comparing `quartical-0.1.9/quartical/flagging/flagging.py` & `quartical-0.2.0/quartical/flagging/flagging.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
         # Reintroduce the correlation axis.
         flag_col = da.broadcast_to(flag_col[:, :, None],
                                    data_col.shape,
                                    chunks=data_col.chunks)
 
         # Convert back to a boolean array.
-        flag_col = flag_col.astype(np.bool)
+        flag_col = flag_col.astype(bool)
 
         # Make the FLAG_ROW column consistent with FLAG.
         flag_row_col = da.all(flag_col, axis=(1, 2))
 
         updated_xds = xds.assign(
             {
                 "FLAG": (xds.DATA.dims, flag_col),
@@ -95,18 +95,24 @@
     # decisions per element.
 
     # We assume that the first and last entries of the correlation axis
     # are the on-diagonal terms. TODO: This should be safe provided we don't
     # have off-diagonal only data, although in that case the flagging
     # logic is probablly equally applicable.
 
-    missing_points = np.any(data_col[..., (0, -1)] == 0, axis=-1)
+    n_corr = data_col.shape[-1]
+    start = 0
+    stop = n_corr
+    step = 3 if n_corr == 4 else 1
+    corr_sel = slice(start, stop, step)
+
+    missing_points = np.any(data_col[..., corr_sel] == 0, axis=-1)
     flags[missing_points] = True
 
-    noweight_points = np.any(weight_col[..., (0, -1)] == 0, axis=-1)
+    noweight_points = np.any(weight_col[..., corr_sel] == 0, axis=-1)
     flags[noweight_points] = True
 
     # At this point, if any correlation is flagged, flag other correlations.
     flags = np.any(flags, axis=-1).astype(np.int8)
 
     return flags
 
@@ -134,58 +140,57 @@
                 xds._WEIGHT.data,
                 name="unity_weights-" + uuid4().hex
             )
         flag_col = xds.FLAG.data
         ant1_col = xds.ANTENNA1.data
         ant2_col = xds.ANTENNA2.data
         n_ant = xds.dims["ant"]
+        n_bl_w_autos = (n_ant * (n_ant - 1))/2 + n_ant
         n_t_chunk, n_f_chunk, _ = residuals.numblocks
 
         wres = da.blockwise(
             compute_whitened_residual, ("rowlike", "chan", "corr"),
             residuals, ("rowlike", "chan", "corr"),
             weight_col, ("rowlike", "chan", "corr"),
             dtype=residuals.dtype,
             align_arrays=False,
             concatenate=True
         )
 
         bl_mad_and_med_real = da.blockwise(
             compute_bl_mad_and_med,
-            ("rowlike", "chan", "ant1", "ant2", "corr", "est"),
+            ("rowlike", "chan", "bl", "corr", "est"),
             wres.real, ("rowlike", "chan", "corr"),
             flag_col, ("rowlike", "chan"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
             n_ant, None,
             dtype=wres.real.dtype,
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": (1,)*n_t_chunk,
                            "chan": (1,)*n_f_chunk},
-            new_axes={"ant1": n_ant,
-                      "ant2": n_ant,
+            new_axes={"bl": n_bl_w_autos,
                       "est": 2}
         )
 
         bl_mad_and_med_imag = da.blockwise(
             compute_bl_mad_and_med,
-            ("rowlike", "chan", "ant1", "ant2", "corr", "est"),
+            ("rowlike", "chan", "bl", "corr", "est"),
             wres.imag, ("rowlike", "chan", "corr"),
             flag_col, ("rowlike", "chan"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
             n_ant, None,
             dtype=wres.imag.dtype,
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": (1,)*n_t_chunk,
                            "chan": (1,)*n_f_chunk},
-            new_axes={"ant1": n_ant,
-                      "ant2": n_ant,
+            new_axes={"bl": n_bl_w_autos,
                       "est": 2}
         )
 
         gbl_mad_and_med_real = da.blockwise(
             compute_gbl_mad_and_med, ("rowlike", "chan", "corr", "est"),
             wres.real, ("rowlike", "chan", "corr"),
             flag_col, ("rowlike", "chan"),
@@ -207,48 +212,33 @@
             adjust_chunks={"rowlike": (1,)*n_t_chunk,
                            "chan": (1,)*n_f_chunk},
             new_axes={"est": 2}
         )
 
         row_chunks = residuals.chunks[0]
 
-        mad_flags_real = da.blockwise(
+        mad_flags = da.blockwise(
             compute_mad_flags, ("rowlike", "chan"),
-            wres.real, ("rowlike", "chan", "corr"),
+            wres, ("rowlike", "chan", "corr"),
             gbl_mad_and_med_real, ("rowlike", "chan", "corr", "est"),
-            bl_mad_and_med_real,
-            ("rowlike", "chan", "ant1", "ant2", "corr", "est"),
-            ant1_col, ("rowlike",),
-            ant2_col, ("rowlike",),
-            gbl_thresh, None,
-            bl_thresh, None,
-            max_deviation, None,
-            dtype=np.int8,
-            align_arrays=False,
-            concatenate=True,
-            adjust_chunks={"rowlike": row_chunks},
-        )
-
-        mad_flags_imag = da.blockwise(
-            compute_mad_flags, ("rowlike", "chan"),
-            wres.imag, ("rowlike", "chan", "corr"),
             gbl_mad_and_med_imag, ("rowlike", "chan", "corr", "est"),
-            bl_mad_and_med_imag,
-            ("rowlike", "chan", "ant1", "ant2", "corr", "est"),
+            bl_mad_and_med_real, ("rowlike", "chan", "bl", "corr", "est"),
+            bl_mad_and_med_imag, ("rowlike", "chan", "bl", "corr", "est"),
             ant1_col, ("rowlike",),
             ant2_col, ("rowlike",),
             gbl_thresh, None,
             bl_thresh, None,
             max_deviation, None,
+            n_ant, None,
             dtype=np.int8,
             align_arrays=False,
             concatenate=True,
             adjust_chunks={"rowlike": row_chunks},
         )
 
-        flag_col = da.where(mad_flags_real | mad_flags_imag, 1, flag_col)
+        flag_col = da.where(mad_flags, 1, flag_col)
 
         flagged_data_xds = xds.assign({"FLAG": (("row", "chan"), flag_col)})
 
         flagged_data_xds_list.append(flagged_data_xds)
 
     return flagged_data_xds_list
```

### Comparing `quartical-0.1.9/quartical/gains/amplitude/kernel.py` & `quartical-0.2.0/quartical/gains/amplitude/kernel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,95 +1,116 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
+from numba import prange, njit
+from numba.extending import overload
+from quartical.utils.numba import (coerce_literal,
+                                   JIT_OPTIONS,
+                                   PARALLEL_JIT_OPTIONS)
 from quartical.gains.general.generics import (native_intermediaries,
                                               upsampled_itermediaries,
                                               per_array_jhj_jhr,
                                               resample_solints,
                                               downsample_jhj_jhr)
 from quartical.gains.general.flagging import (flag_intermediaries,
                                               update_gain_flags,
                                               finalize_gain_flags,
-                                              apply_gain_flags,
+                                              apply_gain_flags_to_flag_col,
                                               update_param_flags)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
-
-
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
-
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
-
-amplitude_args = namedtuple(
-    "amplitude_args",
-    (
-        "params",
-        "param_flags",
-        "t_bin_arr"
-    )
-)
 
 
 def get_identity_params(corr_mode):
 
     if corr_mode.literal_value in (2, 4):
         return np.ones((2,), dtype=np.float64)
     elif corr_mode.literal_value == 1:
         return np.ones((1,), dtype=np.float64)
     else:
         raise ValueError("Unsupported number of correlations.")
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def amplitude_solver(base_args, term_args, meta_args, corr_mode):
+@njit(**JIT_OPTIONS)
+def amplitude_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return amplitude_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
+
+
+def amplitude_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(amplitude_solver_impl, jit_options=JIT_OPTIONS)
+def nb_amplitude_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
 
-    coerce_literal(amplitude_solver, ["corr_mode"])
+    coerce_literal(nb_amplitude_solver_impl, ["corr_mode"])
 
     identity_params = get_identity_params(corr_mode)
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
-        active_params = term_args.params[active_term]
+        active_params = chain_inputs.params[active_term]
 
         # Set up some intemediaries used for flagging
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
         abs2_diffs_trend = np.zeros_like(active_gain_flags, dtype=np.float64)
-        flag_imdry = \
-            flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
+        flag_imdry = flag_intermediaries(
+            km1_gain, km1_abs2_diffs, abs2_diffs_trend
+        )
 
         # Set up some intemediaries used for solving.
         real_dtype = active_gain.real.dtype
         param_shape = active_params.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_g = base_args.f_map_arr[0, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_g = mapping_inputs.freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, param_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
         extents = get_extents(resampler.upsample_t_map, active_f_map_g)
@@ -101,93 +122,120 @@
         jhj = upsampled_jhj[:param_shape[0]]
         jhr = upsampled_jhr[:param_shape[0]]
         update = np.zeros(param_shape, dtype=real_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        for loop_idx in range(max_iter):
+        for loop_idx in range(max_iter or 1):
 
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            corr_mode)
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
-            compute_update(native_imdry,
-                           corr_mode)
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
+            compute_update(native_imdry, corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Propagate gain flags to parameter flags.
-            update_param_flags(base_args,
-                               term_args,
-                               meta_args,
-                               identity_params)
+            update_param_flags(
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                identity_params
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     absv1_idiv_absv2 = factories.absv1_idiv_absv2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
@@ -195,42 +243,44 @@
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        a1 = base_args.a1
-        a2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr = base_args.f_map_arr[0]  # We only need the gain mappings.
-        d_map_arr = base_args.d_map_arr
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        dir_maps = mapping_inputs.dir_maps
+
+        gains = chain_inputs.gains
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
-        _, n_chan, n_dir, n_corr = model.shape
+        n_row, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
         jhr[:] = 0
 
         n_tint, n_fint, n_ant, n_gdir, n_param = jhr.shape
         n_int = n_tint*n_fint
 
@@ -281,15 +331,15 @@
 
             jhr_tifi = jhr[ti, fi]
             jhj_tifi = jhj[ti, fi]
 
             for row_ind in range(rs, re):
 
                 row = get_row(row_ind, row_map)
-                a1_m, a2_m = a1[row], a2[row]
+                a1_m, a2_m = antenna1[row], antenna2[row]
 
                 for f in range(fs, fe):
 
                     if flags[row, f]:  # Skip flagged data points.
                         continue
 
                     # Apply row weights in the BDA case, otherwise a no-op.
@@ -306,17 +356,17 @@
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -343,15 +393,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -388,20 +438,20 @@
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -432,40 +482,65 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, loop_idx,
-                    corr_mode):
+def finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
+    raise NotImplementedError
 
-    set_identity = factories.set_identity_factory(corr_mode)
-    param_to_gain = param_to_gain_factory(corr_mode)
 
-    def impl(base_args, term_args, meta_args, native_imdry, loop_idx,
-             corr_mode):
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
 
-        active_term = meta_args.active_term
+    set_identity = factories.set_identity_factory(corr_mode)
+    param_to_gain = param_to_gain_factory(corr_mode)
 
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
+    def impl(
+        chain_inputs,
+        meta_inputs,
+        native_imdry,
+        loop_idx,
+        corr_mode
+    ):
 
-        params = term_args.params[active_term]
+        dd_term = meta_inputs.dd_term
+        active_term = meta_inputs.active_term
+        pinned_directions = meta_inputs.pinned_directions
+
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
+        params = chain_inputs.params[active_term]
 
         update = native_imdry.update
 
         n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
 
+        if dd_term:
+            dir_loop = [d for d in range(n_dir) if d not in pinned_directions]
+        else:
+            dir_loop = [d for d in range(n_dir)]
+
         for ti in range(n_tint):
             for fi in range(n_fint):
                 for a in range(n_ant):
-                    for d in range(n_dir):
+                    for d in dir_loop:
 
                         p = params[ti, fi, a, d]
                         g = gain[ti, fi, a, d]
                         fl = gain_flags[ti, fi, a, d]
                         upd = update[ti, fi, a, d]
 
                         if fl == 1:
@@ -584,7 +659,29 @@
             w_00 = unpack(w)
 
             jhj[0, 0] += (jh_00*w_00*j_00).real
     else:
         raise ValueError("Unsupported number of correlations.")
 
     return factories.qcjit(impl)
+
+
+@njit(**JIT_OPTIONS)
+def amplitude_params_to_gains(
+    params,
+    gains
+):
+
+    n_time, n_freq, n_ant, n_dir, n_corr = gains.shape
+
+    for t in range(n_time):
+        for f in range(n_freq):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    g = gains[t, f, a, d]
+                    p = params[t, f, a, d]
+
+                    g[0] = p[0]
+
+                    if n_corr > 1:
+                        g[-1] = p[-1]
```

### Comparing `quartical-0.1.9/quartical/gains/complex/diag_kernel.py` & `quartical-0.2.0/quartical/gains/complex/diag_kernel.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,57 +1,85 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
+from numba import prange, njit
+from numba.extending import overload
+from quartical.utils.numba import (coerce_literal,
+                                   JIT_OPTIONS,
+                                   PARALLEL_JIT_OPTIONS)
 from quartical.gains.general.generics import (native_intermediaries,
                                               upsampled_itermediaries,
                                               per_array_jhj_jhr,
                                               resample_solints,
                                               downsample_jhj_jhr)
 from quartical.gains.general.flagging import (flag_intermediaries,
                                               update_gain_flags,
                                               finalize_gain_flags,
-                                              apply_gain_flags)
+                                              apply_gain_flags_to_flag_col,
+                                              apply_gain_flags_to_gains)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
 
 
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
+@njit(**JIT_OPTIONS)
+def diag_complex_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return diag_complex_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
 
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
 
-complex_args = namedtuple("complex_args", ())
+def diag_complex_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def diag_complex_solver(base_args, term_args, meta_args, corr_mode):
+@overload(diag_complex_solver_impl, jit_options=JIT_OPTIONS)
+def nb_diag_complex_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
 
-    coerce_literal(diag_complex_solver, ["corr_mode"])
+    coerce_literal(nb_diag_complex_solver_impl, ["corr_mode"])
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
 
         # Set up some intemediaries used for flagging. TODO: Move?
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
@@ -59,16 +87,16 @@
         flag_imdry = \
             flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
 
         # Set up some intemediaries used for solving.
         complex_dtype = active_gain.dtype
         gain_shape = active_gain.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_g = base_args.f_map_arr[0, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_g = mapping_inputs.freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, gain_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
         extents = get_extents(resampler.upsample_t_map, active_f_map_g)
@@ -79,129 +107,158 @@
         jhj = upsampled_jhj[:gain_shape[0]]
         jhr = upsampled_jhr[:gain_shape[0]]
         update = np.zeros(gain_shape, dtype=complex_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        for loop_idx in range(max_iter):
+        for loop_idx in range(max_iter or 1):
 
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            corr_mode)
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
-            compute_update(native_imdry,
-                           corr_mode)
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
+            compute_update(native_imdry, corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
+
+        reference_gains(chain_inputs, meta_inputs, corr_mode)
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
     iadd = factories.iadd_factory(corr_mode)
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        antenna1 = base_args.a1
-        antenna2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr = base_args.f_map_arr[0]  # We only need the gain mappings.
-        d_map_arr = base_args.d_map_arr
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        dir_maps = mapping_inputs.dir_maps
+
+        gains = chain_inputs.gains
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
-        _, n_chan, n_dir, n_corr = model.shape
+        n_row, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
         jhr[:] = 0
 
         n_tint, n_fint, n_ant, n_gdir, n_corr = jhr.shape
         n_int = n_tint*n_fint
 
@@ -278,17 +335,17 @@
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -315,15 +372,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -360,20 +417,20 @@
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -404,38 +461,63 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, loop_idx,
-                    corr_mode):
+def finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
 
     set_identity = factories.set_identity_factory(corr_mode)
 
-    def impl(base_args, term_args, meta_args, native_imdry, loop_idx,
-             corr_mode):
+    def impl(
+        chain_inputs,
+        meta_inputs,
+        native_imdry,
+        loop_idx,
+        corr_mode
+    ):
 
-        dd_term = meta_args.dd_term
-        active_term = meta_args.active_term
+        dd_term = meta_inputs.dd_term
+        active_term = meta_inputs.active_term
+        pinned_directions = meta_inputs.pinned_directions
 
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
 
         update = native_imdry.update
 
         n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
 
+        if dd_term:
+            dir_loop = [d for d in range(n_dir) if d not in pinned_directions]
+        else:
+            dir_loop = [d for d in range(n_dir)]
+
         for ti in range(n_tint):
             for fi in range(n_fint):
                 for a in range(n_ant):
-                    for d in range(n_dir):
+                    for d in dir_loop:
 
                         g = gain[ti, fi, a, d]
                         fl = gain_flags[ti, fi, a, d]
                         upd = update[ti, fi, a, d]
 
                         if fl == 1:
                             set_identity(g)
@@ -529,7 +611,63 @@
             w_00 = unpack(w)
 
             jhj[0] += jh_00*w_00*j_00
     else:
         raise ValueError("Unsupported number of correlations.")
 
     return factories.qcjit(impl)
+
+
+@njit(**JIT_OPTIONS)
+def reference_gains(chain_inputs, meta_inputs, mode):
+    return reference_gains_impl(chain_inputs, meta_inputs, mode)
+
+
+def reference_gains_impl(chain_inputs, meta_inputs, mode):
+    raise NotImplementedError
+
+
+@overload(reference_gains_impl, jit_options=JIT_OPTIONS)
+def nb_reference_gains_impl(chain_inputs, meta_inputs, mode):
+
+    coerce_literal(nb_reference_gains_impl, ["mode"])
+    v1_imul_v2 = factories.v1_imul_v2_factory(mode)
+
+    def impl(chain_inputs, meta_inputs, mode):
+
+        active_term = meta_inputs.active_term
+        ref_ant = meta_inputs.reference_antenna
+
+        gains = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
+
+        n_ti, n_fi, n_ant, n_dir, n_corr = gains.shape
+
+        ref_gains = gains[:, :, ref_ant: ref_ant + 1, :, :].copy()
+
+        for t in range(n_ti):
+            for f in range(n_fi):
+                for d in range(n_dir):
+
+                    if gain_flags[t, f, ref_ant, d]:  # TODO: Flagged refant?
+                        continue
+                    elif n_corr in (1, 2):
+                        rg = ref_gains[t, f, 0, d]
+                        rg[...] = rg.conjugate()/np.abs(rg)
+                    else:
+                        rg = ref_gains[t, f, 0, d]
+                        rg[1:3] = 0
+                        rg[::3] = rg[::3].conjugate()/np.abs(rg[::3])
+
+        for t in range(n_ti):
+            for f in range(n_fi):
+                for a in range(n_ant):
+                    for d in range(n_dir):
+
+                        g = gains[t, f, a, d]
+                        rg = ref_gains[t, f, 0, d]
+
+                        v1_imul_v2(g, rg, g)
+
+        apply_gain_flags_to_gains(gain_flags, gains)
+
+    return impl
```

### Comparing `quartical-0.1.9/quartical/gains/complex/kernel.py` & `quartical-0.2.0/quartical/gains/complex/kernel.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,76 +1,104 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
+from numba import prange, njit
+from numba.extending import overload
+from quartical.utils.numba import (coerce_literal,
+                                   JIT_OPTIONS,
+                                   PARALLEL_JIT_OPTIONS)
 from quartical.gains.general.generics import (native_intermediaries,
                                               upsampled_itermediaries,
                                               per_array_jhj_jhr,
                                               resample_solints,
                                               downsample_jhj_jhr)
 from quartical.gains.general.flagging import (flag_intermediaries,
                                               update_gain_flags,
                                               finalize_gain_flags,
-                                              apply_gain_flags)
+                                              apply_gain_flags_to_flag_col)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
 
 
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
+@njit(**JIT_OPTIONS)
+def complex_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return complex_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
 
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
 
-complex_args = namedtuple("complex_args", ())
+def complex_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def complex_solver(base_args, term_args, meta_args, corr_mode):
+@overload(complex_solver_impl, jit_options=JIT_OPTIONS)
+def nb_complex_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
 
-    coerce_literal(complex_solver, ["corr_mode"])
+    coerce_literal(nb_complex_solver_impl, ["corr_mode"])
 
     get_jhj_dims = get_jhj_dims_factory(corr_mode)
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
 
         # Set up some intemediaries used for flagging. TODO: Move?
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
         abs2_diffs_trend = np.zeros_like(active_gain_flags, dtype=np.float64)
-        flag_imdry = \
-            flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
+        flag_imdry = flag_intermediaries(
+            km1_gain, km1_abs2_diffs, abs2_diffs_trend
+        )
 
         # Set up some intemediaries used for solving.
         complex_dtype = active_gain.dtype
         gain_shape = active_gain.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_g = base_args.f_map_arr[0, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_g = mapping_inputs.freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, gain_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
         extents = get_extents(resampler.upsample_t_map, active_f_map_g)
@@ -82,129 +110,156 @@
         jhj = upsampled_jhj[:gain_shape[0]]
         jhr = upsampled_jhr[:gain_shape[0]]
         update = np.zeros(gain_shape, dtype=complex_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        for loop_idx in range(max_iter):
+        for loop_idx in range(max_iter or 1):
 
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            corr_mode)
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
-            compute_update(native_imdry,
-                           corr_mode)
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
+            compute_update(native_imdry, corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
     iadd = factories.iadd_factory(corr_mode)
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        antenna1 = base_args.a1
-        antenna2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr = base_args.f_map_arr[0]  # We only need the gain mappings.
-        d_map_arr = base_args.d_map_arr
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        dir_maps = mapping_inputs.dir_maps
+
+        gains = chain_inputs.gains
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
-        _, n_chan, n_dir, n_corr = model.shape
+        n_row, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
         jhr[:] = 0
 
         n_tint, n_fint, n_ant, n_gdir, n_corr = jhr.shape
         n_int = n_tint*n_fint
 
@@ -281,17 +336,17 @@
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -318,15 +373,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -363,20 +418,20 @@
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -407,38 +462,63 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, loop_idx,
-                    corr_mode):
+def finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
 
     set_identity = factories.set_identity_factory(corr_mode)
 
-    def impl(base_args, term_args, meta_args, native_imdry, loop_idx,
-             corr_mode):
+    def impl(
+        chain_inputs,
+        meta_inputs,
+        native_imdry,
+        loop_idx,
+        corr_mode
+    ):
 
-        dd_term = meta_args.dd_term
-        active_term = meta_args.active_term
+        dd_term = meta_inputs.dd_term
+        active_term = meta_inputs.active_term
+        pinned_directions = meta_inputs.pinned_directions
 
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
 
         update = native_imdry.update
 
         n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
 
+        if dd_term:
+            dir_loop = [d for d in range(n_dir) if d not in pinned_directions]
+        else:
+            dir_loop = [d for d in range(n_dir)]
+
         for ti in range(n_tint):
             for fi in range(n_fint):
                 for a in range(n_ant):
-                    for d in range(n_dir):
+                    for d in dir_loop:
 
                         g = gain[ti, fi, a, d]
                         fl = gain_flags[ti, fi, a, d]
                         upd = update[ti, fi, a, d]
 
                         if fl == 1:
                             set_identity(g)
```

### Comparing `quartical-0.1.9/quartical/gains/crosshand_phase/kernel.py` & `quartical-0.2.0/quartical/gains/crosshand_phase/kernel.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,113 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
+from numba import prange, njit
+from numba.extending import overload
+from quartical.utils.numba import (coerce_literal,
+                                   JIT_OPTIONS,
+                                   PARALLEL_JIT_OPTIONS)
 from quartical.gains.general.generics import (native_intermediaries,
                                               upsampled_itermediaries,
                                               per_array_jhj_jhr,
                                               resample_solints,
                                               downsample_jhj_jhr)
 from quartical.gains.general.flagging import (flag_intermediaries,
                                               update_gain_flags,
                                               finalize_gain_flags,
-                                              apply_gain_flags,
+                                              apply_gain_flags_to_flag_col,
                                               update_param_flags)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
-
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
-
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
-
-crosshand_phase_args = namedtuple(
-    "crosshand_phase_args",
-    (
-        "params",
-        "param_flags",
-        "t_bin_arr"
-    )
-)
 
 
 def get_identity_params(corr_mode):
 
     if corr_mode.literal_value == 4:
         return np.zeros((1,), dtype=np.float64)
     else:
         raise ValueError("Unsupported number of correlations.")
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def crosshand_phase_solver(base_args, term_args, meta_args, corr_mode):
+@njit(**JIT_OPTIONS)
+def crosshand_phase_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return crosshand_phase_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
+
 
-    coerce_literal(crosshand_phase_solver, ["corr_mode"])
+def crosshand_phase_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(crosshand_phase_solver_impl, jit_options=JIT_OPTIONS)
+def nb_crosshand_phase_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+
+    coerce_literal(nb_crosshand_phase_solver_impl, ["corr_mode"])
 
     identity_params = get_identity_params(corr_mode)
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
-        active_params = term_args.params[active_term]
+        active_params = chain_inputs.params[active_term]
 
         # Set up some intemediaries used for flagging.
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
         abs2_diffs_trend = np.zeros_like(active_gain_flags, dtype=np.float64)
         flag_imdry = \
             flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
 
         # Set up some intemediaries used for solving.
         real_dtype = active_gain.real.dtype
         param_shape = active_params.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_g = base_args.f_map_arr[0, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_g = mapping_inputs.freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, param_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
         extents = get_extents(resampler.upsample_t_map, active_f_map_g)
@@ -98,94 +119,121 @@
         jhj = upsampled_jhj[:param_shape[0]]
         jhr = upsampled_jhr[:param_shape[0]]
         update = np.zeros(param_shape, dtype=real_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        for loop_idx in range(max_iter):
+        for loop_idx in range(max_iter or 1):
 
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            corr_mode)
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
-            compute_update(native_imdry,
-                           corr_mode)
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
+            compute_update(native_imdry, corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode,
-                                          numbness=1e9)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode,
+                numbness=1e9
+            )
 
             # Propagate gain flags to parameter flags.
-            update_param_flags(base_args,
-                               term_args,
-                               meta_args,
-                               identity_params)
+            update_param_flags(
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                identity_params
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     absv1_idiv_absv2 = factories.absv1_idiv_absv2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
@@ -193,37 +241,39 @@
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        antenna1 = base_args.a1
-        antenna2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr = base_args.f_map_arr[0]  # We only need the gain mappings.
-        d_map_arr = base_args.d_map_arr
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        dir_maps = mapping_inputs.dir_maps
+
+        gains = chain_inputs.gains
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
         _, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
@@ -306,17 +356,17 @@
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -343,15 +393,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -392,20 +442,20 @@
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -436,40 +486,65 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, loop_idx,
-                    corr_mode):
+def finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
+    raise NotImplementedError
 
-    set_identity = factories.set_identity_factory(corr_mode)
-    param_to_gain = param_to_gain_factory(corr_mode)
 
-    def impl(base_args, term_args, meta_args, native_imdry, loop_idx,
-             corr_mode):
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
 
-        active_term = meta_args.active_term
+    set_identity = factories.set_identity_factory(corr_mode)
+    param_to_gain = param_to_gain_factory(corr_mode)
 
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
+    def impl(
+        chain_inputs,
+        meta_inputs,
+        native_imdry,
+        loop_idx,
+        corr_mode
+    ):
 
-        params = term_args.params[active_term]
+        dd_term = meta_inputs.dd_term
+        active_term = meta_inputs.active_term
+        pinned_directions = meta_inputs.pinned_directions
+
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
+        params = chain_inputs.params[active_term]
 
         update = native_imdry.update
 
         n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
 
+        if dd_term:
+            dir_loop = [d for d in range(n_dir) if d not in pinned_directions]
+        else:
+            dir_loop = [d for d in range(n_dir)]
+
         for ti in range(n_tint):
             for fi in range(n_fint):
                 for a in range(n_ant):
-                    for d in range(n_dir):
+                    for d in dir_loop:
 
                         p = params[ti, fi, a, d]
                         g = gain[ti, fi, a, d]
                         fl = gain_flags[ti, fi, a, d]
                         upd = update[ti, fi, a, d]
 
                         if fl == 1:
@@ -554,7 +629,27 @@
             jhj[0, 0] += jhwj_00.real
 
     else:
         raise ValueError("Crosshand phase can only be solved for with four "
                          "correlation data.")
 
     return factories.qcjit(impl)
+
+
+@njit(**JIT_OPTIONS)
+def crosshand_params_to_gains(
+    params,
+    gains
+):
+
+    n_time, n_freq, n_ant, n_dir, n_corr = gains.shape
+
+    for t in range(n_time):
+        for f in range(n_freq):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    g = gains[t, f, a, d]
+                    p = params[t, f, a, d]
+
+                    g[0] = np.exp(1j*p[0])
+                    g[-1] = 1
```

### Comparing `quartical-0.1.9/quartical/gains/datasets.py` & `quartical-0.2.0/quartical/gains/datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,370 +1,273 @@
 # -*- coding: utf-8 -*-
 from quartical.config.external import Gain
-from quartical.config.internal import yield_from
 from loguru import logger  # noqa
 import numpy as np
 import dask.array as da
+import xarray
+from uuid import uuid4
 from daskms.experimental.zarr import xds_to_zarr
+from quartical.gains.gain import gain_spec_tup, param_spec_tup
 from quartical.gains import TERM_TYPES
-from quartical.utils.dask import blockwise_unique
-from quartical.utils.maths import mean_for_index
 from quartical.gains.general.generics import combine_gains, combine_flags
 
 
-def make_gain_xds_lod(data_xds_list,
-                      tipc_list,
-                      fipc_list,
-                      coords_per_xds,
-                      chain_opts):
+def make_gain_xds_lod(data_xds_list, chain):
     """Returns a list of dicts of xarray.Dataset objects describing the gains.
 
     For a given input xds containing data, creates an xarray.Dataset object
     per term which describes the term's dimensions.
 
     Args:
         data_xds_list: A list of xarray.Dataset objects containing MS data.
-        tipc_list: List of numpy.ndarray objects containing number of time
-            intervals in a chunk.
-        fipc_list: List of numpy.ndarray objects containing number of freq
-            intervals in a chunk.
-        coords_per_xds: A List of Dicts containing coordinates.
-        chain_opts: A Chain config object.
+        chains: A list of Gain objects.
 
     Returns:
         gain_xds_lod: A List of Dicts of xarray.Dataset objects describing the
             gain terms assosciated with each data xarray.Dataset.
     """
 
-    gain_xds_lod = []
+    scaffolds_per_xds = []
 
-    for xds_ind, data_xds in enumerate(data_xds_list):
+    for data_xds in data_xds_list:
 
-        term_xds_dict = {}
+        gain_scaffolds = {}
 
-        term_coords = coords_per_xds[xds_ind]
+        for gain_obj in chain:
 
-        for loop_vars in enumerate(yield_from(chain_opts, "type")):
-            term_ind, (term_name, term_type) = loop_vars
+            gain_scaffolds[gain_obj.name] = \
+                scaffold_from_data_xds(data_xds, gain_obj)
 
-            term_t_chunks = tipc_list[xds_ind][:, :, term_ind]
-            term_f_chunks = fipc_list[xds_ind][:, :, term_ind]
-            term_opts = getattr(chain_opts, term_name)
+        scaffolds_per_xds.append(gain_scaffolds)
 
-            term_obj = TERM_TYPES[term_type](term_name,
-                                             term_opts,
-                                             data_xds,
-                                             term_coords,
-                                             term_t_chunks,
-                                             term_f_chunks)
-
-            term_xds_dict[term_name] = term_obj.make_xds()
+    # NOTE: This triggers an early compute to determine all the chunking info.
+    gain_xds_lod = [
+        {
+            tn: xarray.Dataset(**ts) for tn, ts in gain_scaffolds.items()
+        }
+        for gain_scaffolds in da.compute(scaffolds_per_xds)[0]
+    ]
 
-        gain_xds_lod.append(term_xds_dict)
+    # This is a nasty workaround for the one problem with the scaffolds -
+    # the chunk specs coming out containing arrays.
+    # TODO: Think about a neater approach.
+    for gain_xdss in gain_xds_lod:
+        for _, gain_xds in gain_xdss.items():
+            gain_xds.attrs["GAIN_SPEC"] = \
+                gain_spec_tup(*list(map(tuple, gain_xds.GAIN_SPEC)))
+            if "PARAM_SPEC" in gain_xds.attrs:
+                gain_xds.attrs["PARAM_SPEC"] = \
+                    param_spec_tup(*list(map(tuple, gain_xds.PARAM_SPEC)))
 
     return gain_xds_lod
 
 
-def compute_interval_chunking(data_xds_list, t_map_list, f_map_list):
-    '''Compute the per-term chunking of the gains.
-
-    Given a list of data xarray.Datasets as well as information about the
-    time and frequency mappings, computes the chunk sizes of the gain terms.
-
-    Args:
-        data_xds_list: A list of data-containing xarray.Dataset objects.
-        t_map_list: A list of arrays describing how times map to solint.
-        f_map_list: A list of arrays describing how freqs map to solint.
-
-    Returns:
-        A tuple of lists containing arrays which descibe the chunking.
-    '''
-
-    tipc_list = []
-    fipc_list = []
-
-    for xds_ind, _ in enumerate(data_xds_list):
-
-        t_map_arr = t_map_list[xds_ind]
-        f_map_arr = f_map_list[xds_ind]
-
-        tipc_per_term = da.map_blocks(lambda arr: arr[:, -1:, :] + 1,
-                                      t_map_arr,
-                                      chunks=((2,),
-                                              (1,)*t_map_arr.numblocks[1],
-                                              t_map_arr.chunks[2]))
-
-        fipc_per_term = da.map_blocks(lambda arr: arr[:, -1:, :] + 1,
-                                      f_map_arr,
-                                      chunks=((2,),
-                                              (1,)*f_map_arr.numblocks[1],
-                                              f_map_arr.chunks[2]))
-
-        tipc_list.append(tipc_per_term)
-        fipc_list.append(fipc_per_term)
-
-    # This is an early compute which is necessary to figure out the gain dims.
-    return da.compute(tipc_list, fipc_list)
-
-
-def compute_dataset_coords(data_xds_list,
-                           t_bin_list,
-                           f_map_list,
-                           tipc_list,
-                           fipc_list,
-                           terms):
-    '''Compute the cooridnates for the gain datasets.
-
-    Given a list of data xarray.Datasets as well as information about the
-    binning along the time and frequency axes, computes the true coordinate
-    values for the gain xarray.Datasets.
-
-    Args:
-        data_xds_list: A list of data-containing xarray.Dataset objects.
-        t_bin_list: A list of arrays describing how times map to solint.
-        f_map_list: A list of arrays describing how freqs map to solint.
-        tipc_list: A list of arrays contatining the number of time intervals
-            per chunk.
-        fipc_list: A list of arrays contatining the number of freq intervals
-            per chunk.
-
-    Returns:
-        A list of dictionaries containing the computed coordinate values.
-    '''
-
-    coords_per_xds = []
-
-    for xds_ind, data_xds in enumerate(data_xds_list):
-
-        utime_chunks = list(map(int, data_xds.UTIME_CHUNKS))
-
-        # NOTE: Use the BDA version of the column if it is present.
-        time_col = data_xds.get("UPSAMPLED_TIME", data_xds.TIME).data
-
-        unique_times = blockwise_unique(time_col,
-                                        chunks=(utime_chunks,))
-        unique_freqs = data_xds.CHAN_FREQ.data
-
-        coord_dict = {"time": unique_times,  # Doesn't vary with term.
-                      "freq": unique_freqs}  # Doesn't vary with term.
-
-        for term_ind, term_name in enumerate(terms):
-
-            # This indexing corresponds to grabbing the info per xds, per term.
-            tipc = tipc_list[xds_ind][:, :, term_ind]
-            fipc = fipc_list[xds_ind][:, :, term_ind]
-            term_t_bins = t_bin_list[xds_ind][:, :, term_ind]
-            term_f_map = f_map_list[xds_ind][:, :, term_ind]
-
-            mean_gtimes = da.map_blocks(mean_for_index,
-                                        unique_times,
-                                        term_t_bins[0],
-                                        dtype=unique_times.dtype,
-                                        chunks=(tuple(map(int, tipc[0])),))
-
-            mean_ptimes = da.map_blocks(mean_for_index,
-                                        unique_times,
-                                        term_t_bins[1],
-                                        dtype=unique_times.dtype,
-                                        chunks=(tuple(map(int, tipc[1])),))
-
-            mean_gfreqs = da.map_blocks(mean_for_index,
-                                        unique_freqs,
-                                        term_f_map[0],
-                                        dtype=unique_freqs.dtype,
-                                        chunks=(tuple(map(int, fipc[0])),))
-
-            mean_pfreqs = da.map_blocks(mean_for_index,
-                                        unique_freqs,
-                                        term_f_map[1],
-                                        dtype=unique_freqs.dtype,
-                                        chunks=(tuple(map(int, fipc[1])),))
-
-            coord_dict[f"{term_name}_mean_gtime"] = mean_gtimes
-            coord_dict[f"{term_name}_mean_ptime"] = mean_ptimes
-            coord_dict[f"{term_name}_mean_gfreq"] = mean_gfreqs
-            coord_dict[f"{term_name}_mean_pfreq"] = mean_pfreqs
-
-        coords_per_xds.append(coord_dict)
-
-    # We take the hit on a second early compute in order to make loading and
-    # interpolating gains a less complicated operation.
-    return da.compute(coords_per_xds)[0]
-
-
-def make_net_xds_list(data_xds_list, coords_per_xds, output_opts):
+def make_net_xds_lod(data_xds_list, chain, output_opts):
     """Construct a list of dicts of xarray.Datasets to house the net gains.
 
     Args:
         data_xds_list: A List of xarray.Dataset objects containing MS data.
-        coords_per_xds: A List of Dicts containing dataset coords.
         output_opts: An output config object.
 
     Returns:
         net_gain_xds_dol: A Dict of Lists of xarray.Dataset objects to house
             the net gains.
     """
 
     net_names = [f"{''.join(lt)}-net" for lt in output_opts.net_gains]
 
-    net_gain_xds_lod = []
-
-    for data_xds, xds_coords in zip(data_xds_list, coords_per_xds):
-
-        net_t_chunks = np.tile(data_xds.UTIME_CHUNKS, 2).reshape(2, -1)
-        net_f_chunks = np.tile(data_xds.chunks["chan"], 2).reshape(2, -1)
-
-        net_dict = {}
-
-        for net_name in net_names:
+    direction_dependent = any(t.direction_dependent for t in chain)
 
-            # Create a default config object, consistent with the net gain.
-            # NOTE: If we have a direction-dependent model, assume the net gain
-            # is also direction dependent.
-            config = Gain(direction_dependent=bool(data_xds.dims["dir"]))
+    net_configs = [
+        Gain(direction_dependent=direction_dependent) for _ in net_names
+    ]
 
-            net_obj = TERM_TYPES["complex"](net_name,
-                                            config,
-                                            data_xds,
-                                            xds_coords,
-                                            net_t_chunks,
-                                            net_f_chunks)
+    net_chain = [
+        TERM_TYPES["complex"](n, c) for n, c in zip(net_names, net_configs)
+    ]
 
-            net_dict[net_name] = net_obj.make_xds()
+    return make_gain_xds_lod(data_xds_list, net_chain)
 
-        net_gain_xds_lod.append(net_dict)
 
-    return net_gain_xds_lod
-
-
-def combine_gains_wrapper(t_bin_arr, f_map_arr, d_map_arr, term_ids, net_shape,
-                          corr_mode, *gains):
+def combine_gains_wrapper(
+    net_shape,
+    corr_mode,
+    *args
+):
     """Wrapper to stop dask from getting confused. See issue #99."""
 
-    return combine_gains(t_bin_arr, f_map_arr, d_map_arr, term_ids, net_shape,
-                         corr_mode, *gains)
-
-
-def combine_flags_wrapper(t_bin_arr, f_map_arr, d_map_arr, term_ids, net_shape,
-                          corr_mode, *flags):
+    gains = tuple(args[::4])
+    time_maps = tuple(args[1::4])
+    freq_maps = tuple(args[2::4])
+    dir_maps = tuple(args[3::4])
+
+    return combine_gains(
+        gains,
+        time_maps,
+        freq_maps,
+        dir_maps,
+        net_shape,
+        corr_mode,
+    )
+
+
+def combine_flags_wrapper(
+    net_shape,
+    *args
+):
     """Wrapper to stop dask from getting confused. See issue #99."""
 
-    return combine_flags(t_bin_arr, f_map_arr, d_map_arr, term_ids, net_shape,
-                         corr_mode, *flags)
+    flags = tuple(args[::4])
+    time_bins = tuple(args[1::4])
+    freq_maps = tuple(args[2::4])
+    dir_maps = tuple(args[3::4])
+
+    return combine_flags(
+        flags,
+        time_bins,
+        freq_maps,
+        dir_maps,
+        net_shape
+    )
 
 
 def populate_net_xds_list(
     net_gain_xds_lod,
     solved_gain_xds_lod,
-    t_bin_list,
-    f_map_list,
-    d_map_list,
+    mapping_xds_list,
     output_opts
 ):
-    """Poplulate the list net gain datasets with net gain values.
+    """Populate the list net gain datasets with net gain values.
 
     Args:
         net_gain_xds_list: A List of xarray.Dataset objects to house the
             net gains.
         solved_gain_xds_lol: A List of Lists of xarray.Dataset objects housing
             the solved gain terms.
         t_bin_list: A List of dask.Arrays containing mappings from unique
             time to solution interval.
         f_map_list: A List of dask.Arrays containing mappings from channel
             to solution interval.
         d_map_list: A List of numpy.ndarrays containing mappings between
             direction dependent terms and direction independent terms.
-        output_opts: An output configuration object,
+        output_opts: An output configuration object.
 
     Returns:
         net_gain_xds_list: A List of xarray.Dataset objects to house the
             net gains.
     """
 
     net_terms = output_opts.net_gains
 
+    # TODO: Can tenchically get this from the datasets.
     net_names = [f"{''.join(lt)}-net" for lt in net_terms]
 
     net_map = dict(zip(net_names, net_terms))
 
-    gain_dims = ("gain_t", "gain_f", "ant", "dir", "corr")
-    gain_schema = ("time", "chan", "ant", "dir", "corr")
-    flag_schema = ("time", "chan", "ant", "dir")
     populated_net_gain_xds_lod = []
 
-    for ind, (solved_gains, net_gains) in enumerate(zip(solved_gain_xds_lod,
-                                                        net_gain_xds_lod)):
+    # TODO: Move into flag combining function?
+    identity_elements = {
+        1: np.ones(1, dtype=np.complex128),
+        2: np.ones(2, dtype=np.complex128),
+        4: np.array((1, 0, 0, 1), dtype=np.complex128)
+    }
 
-        gains = [itm for xds in solved_gains.values()
-                 for itm in (xds.gains.data, gain_schema)]
-        gain_dtype = np.find_common_type(
-            [xds.gains.data.dtype for xds in solved_gains.values()], []
-        )
-        identity_elements = {
-            1: np.ones(1, dtype=gain_dtype),
-            2: np.ones(2, dtype=gain_dtype),
-            4: np.array((1, 0, 0, 1), dtype=gain_dtype)
-        }
+    itr = zip(solved_gain_xds_lod, net_gain_xds_lod, mapping_xds_list)
 
-        flags = [itm for xds in solved_gains.values()
-                 for itm in (xds.gain_flags.data, flag_schema)]
-        flag_dtype = np.find_common_type(
-            [xds.gain_flags.dtype for xds in solved_gains.values()], []
-        )
+    for solved_gains, net_gains, mapping_xds in itr:
 
         net_xds_dict = {}
 
         for net_name, req_terms in net_map.items():
 
+            req_time_bins = tuple(
+                [mapping_xds.get(f"{k}_time_bins").data for k in req_terms]
+            )
+            req_freq_maps = tuple(
+                [mapping_xds.get(f"{k}_freq_map").data for k in req_terms]
+            )
+            req_dir_maps = tuple(
+                [mapping_xds.get(f"{k}_dir_map").data for k in req_terms]
+            )
+
             net_xds = net_gains[net_name]
 
-            net_shape = tuple(net_xds.dims[d] for d in gain_dims)
+            net_shape = tuple(net_xds.dims[d] for d in net_xds.GAIN_AXES)
 
             corr_mode = net_shape[-1]
 
-            req_term_ids = \
-                [list(solved_gains.keys()).index(tn) for tn in req_terms]
+            req_term_gains = [solved_gains[t].gains for t in req_terms]
+            req_term_flags = [solved_gains[t].gain_flags for t in req_terms]
+
+            itr = zip(
+                req_term_gains,
+                req_time_bins,
+                req_freq_maps,
+                req_dir_maps
+            )
+
+            req_args = []
+
+            for g, tb, fm, dm in itr:
+                req_args.extend([g.data, g.dims])
+                req_args.extend([tb, ("gain_time",)])
+                req_args.extend([fm, ("gain_freq",)])
+                req_args.extend([dm, ("direction",)])
 
             net_gain = da.blockwise(
-                combine_gains_wrapper, ("time", "chan", "ant", "dir", "corr"),
-                t_bin_list[ind], ("param", "time", "term"),
-                f_map_list[ind], ("param", "chan", "term"),
-                d_map_list[ind], None,
-                req_term_ids, None,
+                combine_gains_wrapper, net_xds.GAIN_AXES,
                 net_shape, None,
                 corr_mode, None,
-                *gains,
-                dtype=gain_dtype,
+                *req_args,
+                dtype=np.complex128,
                 align_arrays=False,
                 concatenate=True,
-                adjust_chunks={"time": net_xds.GAIN_SPEC.tchunk,
-                               "chan": net_xds.GAIN_SPEC.fchunk,
-                               "dir": net_xds.GAIN_SPEC.dchunk}
+                adjust_chunks={
+                    "gain_time": net_xds.GAIN_SPEC.tchunk,
+                    "gain_freq": net_xds.GAIN_SPEC.fchunk,
+                    "direction": net_xds.GAIN_SPEC.dchunk
+                }
+            )
+
+            itr = zip(
+                req_term_flags,
+                req_time_bins,
+                req_freq_maps,
+                req_dir_maps
             )
 
+            req_args = []
+
+            for f, tb, fm, dm in itr:
+                req_args.extend([f.data, f.dims])
+                req_args.extend([tb, ("gain_time",)])
+                req_args.extend([fm, ("gain_freq",)])
+                req_args.extend([dm, ("direction",)])
+
             net_flags = da.blockwise(
-                combine_flags_wrapper, ("time", "chan", "ant", "dir"),
-                t_bin_list[ind], ("param", "time", "term"),
-                f_map_list[ind], ("param", "chan", "term"),
-                d_map_list[ind], None,
-                req_term_ids, None,
-                net_shape[:-1], None,
-                *flags,
-                dtype=flag_dtype,
+                combine_flags_wrapper, net_xds.GAIN_AXES[:-1],
+                net_shape, None,
+                *req_args,
+                dtype=np.int8,
                 align_arrays=False,
                 concatenate=True,
-                adjust_chunks={"time": net_xds.GAIN_SPEC.tchunk,
-                               "chan": net_xds.GAIN_SPEC.fchunk,
-                               "dir": net_xds.GAIN_SPEC.dchunk}
+                adjust_chunks={
+                    "gain_time": net_xds.GAIN_SPEC.tchunk,
+                    "gain_freq": net_xds.GAIN_SPEC.fchunk,
+                    "direction": net_xds.GAIN_SPEC.dchunk
+                }
             )
 
-            net_gain = da.blockwise(np.where, "tfadc",
-                                    net_flags[..., None], "tfadc",
-                                    identity_elements[corr_mode], None,
-                                    net_gain, "tfadc")
+            net_gain = da.blockwise(
+                np.where, net_xds.GAIN_AXES,
+                net_flags[..., None], net_xds.GAIN_AXES,
+                identity_elements[corr_mode], None,
+                net_gain, net_xds.GAIN_AXES
+            )
 
             net_xds = net_xds.assign(
                 {
                     "gains": (net_xds.GAIN_AXES, net_gain),
                     "gain_flags": (net_xds.GAIN_AXES[:-1], net_flags)
                 }
             )
@@ -372,25 +275,23 @@
             net_xds_dict[net_name] = net_xds
 
         populated_net_gain_xds_lod.append(net_xds_dict)
 
     return populated_net_gain_xds_lod
 
 
-def write_gain_datasets(gain_xds_lod, net_xds_lod, output_opts):
+def write_gain_datasets(gain_xds_lod, directory, net_xds_lod=None):
     """Write the contents of gain_xds_lol to zarr in accordance with opts."""
 
-    gain_path = output_opts.gain_directory
-
     term_names = [xds.NAME for xds in gain_xds_lod[0].values()]
 
     writable_xds_dol = {tn: [d[tn] for d in gain_xds_lod] for tn in term_names}
 
     # If net gains have been requested, add them to the writes.
-    if output_opts.net_gains:
+    if net_xds_lod:
         net_names = [xds.NAME for xds in net_xds_lod[0].values()]
         net_xds_dol = {tn: [d[tn] for d in net_xds_lod] for tn in net_names}
         term_names.extend(net_names)
         writable_xds_dol.update(net_xds_dol)
 
     gain_writes_lol = []
 
@@ -401,29 +302,197 @@
         # The following rechunks to some sensible chunk size. This ensures
         # that the chunks are regular and <2GB, which is necessary for zarr.
 
         for xds in term_xds_list:
 
             target_chunks = {}
 
-            if hasattr(xds, "PARAM_AXES"):
-                rechunked_params = \
-                    xds.params.chunk({ax: "auto" for ax in xds.PARAM_AXES[:2]})
+            if "params" in xds.data_vars.keys():
+                rechunked_params = xds.params.chunk(
+                    {ax: "auto" for ax in xds.PARAM_AXES[:2]}
+                )
                 target_chunks.update(rechunked_params.chunksizes)
 
-            rechunked_gains = \
-                xds.gains.chunk({ax: "auto" for ax in xds.GAIN_AXES[:2]})
-            target_chunks.update(rechunked_gains.chunksizes)
+            if "gains" in xds.data_vars.keys():
+                rechunked_gains = xds.gains.chunk(
+                    {ax: "auto" for ax in xds.GAIN_AXES[:2]}
+                )
+                target_chunks.update(rechunked_gains.chunksizes)
 
             rechunked_xds = xds.chunk(target_chunks)
 
             term_write_xds_list.append(rechunked_xds)
 
-        output_path = f"{gain_path}{'::' + term_name}"
+        output_path = f"{directory}::{term_name}"
+
+        gain_writes = xds_to_zarr(
+            term_write_xds_list, output_path, rechunk=True
+        )
 
-        gain_writes_lol.append(xds_to_zarr(term_write_xds_list, output_path))
+        gain_writes_lol.append(gain_writes)
 
     # This converts the interpolated list of lists into a list of dicts.
     write_xds_lod = [{tn: term for tn, term in zip(term_names, terms)}
                      for terms in zip(*gain_writes_lol)]
 
     return write_xds_lod
+
+
+def scaffold_from_data_xds(data_xds, gain_obj):
+    """Produces a scaffold (xarray.Dataset coords and attrs).
+
+    Given an xarray.Dataset containing measurement set data and a gain object,
+    produces a scaffold for an xarray.Dataset to hold the gains. A scaffold is
+    the necessary coords and attributes represented as dask arrays in a
+    dictionary. Once computed, these can be passed to the xarray.Dataset
+    constructor.
+
+    Args:
+        data_xds: An xarray.Dataset containing measurement set data.
+        gain_obj: An Gain object providing configuration information.
+
+    Returns:
+        scaffold: A dictionary of dask.arrays which can be used to construct
+            an xarray.Dataset.
+    """
+
+    # Check whether we are dealing with BDA data.
+    if hasattr(data_xds, "UPSAMPLED_TIME"):
+        time_col = data_xds.UPSAMPLED_TIME.data
+        interval_col = data_xds.UPSAMPLED_INTERVAL.data
+    else:
+        time_col = data_xds.TIME.data
+        interval_col = data_xds.INTERVAL.data
+
+    # If SCAN_NUMBER was a partitioning column it will not be present on
+    # the dataset - we reintroduce it for cases where we need to ensure
+    # solution intervals don't span scan boundaries.
+    if "SCAN_NUMBER" in data_xds.data_vars.keys():
+        scan_col = data_xds.SCAN_NUMBER.data
+    else:
+        scan_col = da.zeros_like(
+            time_col,
+            dtype=np.int32,
+            name="scan_number-" + uuid4().hex
+        )
+
+    time_interval = gain_obj.time_interval
+    respect_scan_boundaries = gain_obj.respect_scan_boundaries
+
+    # TODO: Add in parameterized case.
+    time_bins = gain_obj.make_time_bins(
+        time_col,
+        interval_col,
+        scan_col,
+        time_interval,
+        respect_scan_boundaries
+    )
+
+    time_chunks = gain_obj.make_time_chunks(time_bins)
+
+    chan_freqs = data_xds.CHAN_FREQ.data
+    chan_widths = data_xds.CHAN_WIDTH.data
+    freq_interval = gain_obj.freq_interval
+
+    freq_map = gain_obj.make_freq_map(
+        chan_freqs,
+        chan_widths,
+        freq_interval
+    )
+
+    freq_chunks = gain_obj.make_freq_chunks(freq_map)
+
+    n_dir = data_xds.dims["dir"]
+
+    dir_map = gain_obj.make_dir_map(
+        n_dir,
+        gain_obj.direction_dependent
+    )
+
+    gain_times = gain_obj.make_time_coords(time_col, time_bins)
+    gain_freqs = gain_obj.make_freq_coords(chan_freqs, freq_map)
+
+    direction = dir_map if gain_obj.direction_dependent else dir_map[:1]
+    n_gdir = direction.size
+
+    partition_schema = data_xds.__daskms_partition_schema__
+    id_attrs = {f: data_xds.attrs[f] for f, _ in partition_schema}
+
+    # TODO: Move this the the gain object?
+    n_corr = data_xds.dims["corr"]
+    n_ant = data_xds.dims["ant"]
+    chunk_spec = gain_spec_tup(
+        time_chunks,
+        freq_chunks,
+        (n_ant,),
+        (n_gdir,),
+        (n_corr,)
+    )
+
+    scaffold = {
+        "coords": {
+            "gain_time": (("gain_time",), gain_times),
+            "gain_freq": (("gain_freq",), gain_freqs),
+            "time_chunk": (("time_chunk",), da.arange(time_chunks.size)),
+            "freq_chunk": (("freq_chunk",), da.arange(freq_chunks.size)),
+            "direction": (("direction",), direction),
+            "antenna": (("antenna",), data_xds.ant.data),
+            "correlation": (("correlation",), data_xds.corr.data)
+        },
+        "attrs": {
+            **id_attrs,
+            "FIELD_NAME": data_xds.FIELD_NAME,
+            "NAME": gain_obj.name,
+            "TYPE": gain_obj.type,
+            "GAIN_SPEC": chunk_spec,
+            "GAIN_AXES": gain_obj.gain_axes
+        }
+    }
+
+    if hasattr(gain_obj, "param_axes"):
+        param_time_bins = gain_obj.make_param_time_bins(
+            time_col,
+            interval_col,
+            scan_col,
+            time_interval,
+            respect_scan_boundaries
+        )
+
+        param_time_chunks = gain_obj.make_param_time_chunks(param_time_bins)
+
+        param_freq_map = gain_obj.make_param_freq_map(
+            chan_freqs,
+            chan_widths,
+            freq_interval
+        )
+
+        param_freq_chunks = gain_obj.make_param_freq_chunks(param_freq_map)
+
+        param_times = gain_obj.make_time_coords(time_col, param_time_bins)
+        param_freqs = gain_obj.make_freq_coords(chan_freqs, param_freq_map)
+
+        param_names = gain_obj.make_param_names(data_xds.corr.data)
+        n_param = len(param_names)
+
+        param_chunk_spec = param_spec_tup(
+           param_time_chunks,
+           param_freq_chunks,
+           (n_ant,),
+           (n_gdir,),
+           (n_param,)
+        )
+
+        scaffold["coords"].update(
+            {
+                "param_time": (("param_time",), param_times),
+                "param_freq": (("param_freq",), param_freqs),
+                "param_name": (("param_name",), param_names)
+            }
+        )
+        scaffold["attrs"].update(
+            {
+                "PARAM_SPEC": param_chunk_spec,
+                "PARAM_AXES": gain_obj.param_axes
+            }
+        )
+
+    return scaffold
```

### Comparing `quartical-0.1.9/quartical/gains/delay/__init__.py` & `quartical-0.2.0/quartical/gains/delay/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,107 +1,91 @@
-from quartical.gains.gain import Gain, gain_spec_tup, param_spec_tup
-from quartical.gains.delay.kernel import delay_solver, delay_args
 import numpy as np
+from collections import namedtuple
+from quartical.gains.conversion import no_op
+from quartical.gains.parameterized_gain import ParameterizedGain
+from quartical.gains.delay.kernel import (
+    delay_solver,
+    delay_params_to_gains
+)
+from quartical.gains.general.flagging import (
+    apply_gain_flags_to_gains,
+    apply_param_flags_to_params
+)
+
+# Overload the default measurement set inputs to include the frequencies.
+ms_inputs = namedtuple(
+    'ms_inputs', ParameterizedGain.ms_inputs._fields + ('CHAN_FREQ',)
+)
+
+
+class Delay(ParameterizedGain):
+
+    solver = staticmethod(delay_solver)
+    ms_inputs = ms_inputs
+
+    native_to_converted = (
+        (1, (no_op,)),
+    )
+    converted_to_native = (
+        (1, no_op),
+    )
+    converted_dtype = np.float64
+    native_dtype = np.float64
+
+    def __init__(self, term_name, term_opts):
+
+        super().__init__(term_name, term_opts)
+
+    @classmethod
+    def _make_freq_map(cls, chan_freqs, chan_widths, freq_interval):
+        # Overload gain mapping construction - we evaluate it in every channel.
+        return np.arange(chan_freqs.size, dtype=np.int32)
 
+    @classmethod
+    def make_param_names(cls, correlations):
 
-class Delay(Gain):
-
-    solver = delay_solver
-    term_args = delay_args
+        # TODO: This is not dasky, unlike the other functions. Delayed?
+        parameterisable = ["XX", "YY", "RR", "LL"]
 
-    def __init__(self, term_name, term_opts, data_xds, coords, tipc, fipc):
+        param_corr = [c for c in correlations if c in parameterisable]
 
-        Gain.__init__(self, term_name, term_opts, data_xds, coords, tipc, fipc)
+        template = ("delay_{}",)
 
-        parameterisable = ["XX", "YY", "RR", "LL"]
+        return [n.format(c) for c in param_corr for n in template]
 
-        self.parameterised_corr = \
-            [ct for ct in self.corr_types if ct in parameterisable]
-        self.n_param = 2 * len(self.parameterised_corr)
-
-        self.gain_chunk_spec = gain_spec_tup(self.n_tipc_g,
-                                             self.n_fipc_g,
-                                             (self.n_ant,),
-                                             (self.n_dir,),
-                                             (self.n_corr,))
-        self.param_chunk_spec = param_spec_tup(self.n_tipc_g,
-                                               self.n_fipc_p,
-                                               (self.n_ant,),
-                                               (self.n_dir,),
-                                               (self.n_param,))
-
-        self.gain_axes = ("gain_t", "gain_f", "ant", "dir", "corr")
-        self.param_axes = ("param_t", "param_f", "ant", "dir", "param")
-
-    def make_xds(self):
-
-        xds = Gain.make_xds(self)
-
-        param_template = ["phase_offset_{}", "delay_{}"]
-
-        param_labels = [pt.format(ct) for ct in self.parameterised_corr
-                        for pt in param_template]
-
-        xds = xds.assign_coords({"param": np.array(param_labels),
-                                 "param_t": self.gain_times,
-                                 "param_f": self.param_freqs})
-        xds = xds.assign_attrs({"GAIN_SPEC": self.gain_chunk_spec,
-                                "PARAM_SPEC": self.param_chunk_spec,
-                                "GAIN_AXES": self.gain_axes,
-                                "PARAM_AXES": self.param_axes})
-
-        return xds
-
-    @staticmethod
-    def make_f_maps(chan_freqs, chan_widths, f_int):
-        """Internals of the frequency interval mapper."""
-
-        n_chan = chan_freqs.size
-
-        # The leading dimension corresponds (gain, param). For unparameterised
-        # gains, the parameter mapping is irrelevant.
-        f_map_arr = np.zeros((2, n_chan,), dtype=np.int32)
-
-        if isinstance(f_int, float):
-            net_ivl = 0
-            bin_num = 0
-            for i, ivl in enumerate(chan_widths):
-                f_map_arr[1, i] = bin_num
-                net_ivl += ivl
-                if net_ivl >= f_int:
-                    net_ivl = 0
-                    bin_num += 1
-        else:
-            f_map_arr[1, :] = np.arange(n_chan)//f_int
-
-        f_map_arr[0, :] = np.arange(n_chan)
-
-        return f_map_arr
-
-    @staticmethod
-    def init_term(
-        gain, param, term_ind, term_spec, term_opts, ref_ant, **kwargs
-    ):
+    def init_term(self, term_spec, ref_ant, ms_kwargs, term_kwargs):
         """Initialise the gains (and parameters)."""
 
-        loaded = Gain.init_term(
-            gain, param, term_ind, term_spec, term_opts, ref_ant, **kwargs
+        gains, gain_flags, params, param_flags = super().init_term(
+            term_spec, ref_ant, ms_kwargs, term_kwargs
+        )
+
+        # Convert the parameters into gains.
+        delay_params_to_gains(
+            params,
+            gains,
+            ms_kwargs["CHAN_FREQ"],
+            term_kwargs[f"{self.name}_param_freq_map"],
         )
 
-        if loaded or not term_opts.initial_estimate:
-            return
+        if self.load_from or not self.initial_estimate:
 
-        data = kwargs["data"]  # (row, chan, corr)
-        flags = kwargs["flags"]  # (row, chan)
-        a1 = kwargs["a1"]
-        a2 = kwargs["a2"]
-        chan_freq = kwargs["chan_freqs"]
-        t_map = kwargs["t_map_arr"][0, :, term_ind]  # time -> solint
-        f_map = kwargs["f_map_arr"][1, :, term_ind]  # freq -> solint
-        _, n_chan, n_ant, n_dir, n_corr = gain.shape
+            apply_param_flags_to_params(param_flags, params, 0)
+            apply_gain_flags_to_gains(gain_flags, gains)
+
+            return gains, gain_flags, params, param_flags
+
+        data = ms_kwargs["DATA"]  # (row, chan, corr)
+        flags = ms_kwargs["FLAG"]  # (row, chan)
+        a1 = ms_kwargs["ANTENNA1"]
+        a2 = ms_kwargs["ANTENNA2"]
+        chan_freq = ms_kwargs["CHAN_FREQ"]
+        t_map = term_kwargs[f"{term_spec.name}_time_map"]
+        f_map = term_kwargs[f"{term_spec.name}_param_freq_map"]
+        _, n_chan, n_ant, n_dir, n_corr = gains.shape
 
         # We only need the baselines which include the ref_ant.
         sel = np.where((a1 == ref_ant) | (a2 == ref_ant))
         a1 = a1[sel]
         a2 = a2[sel]
         t_map = t_map[sel]
         data = data[sel]
@@ -162,24 +146,26 @@
                 if n_corr > 1:
                     delay_est_ind_11 = np.argmax(fft_data[..., -1], axis=1)
                     delay_est_11 = fft_freq[delay_est_ind_11]
                     delay_est_11[~valid_ant] = 0
 
                 for t, p, q in zip(t_map[sel], a1[sel], a2[sel]):
                     if p == ref_ant:
-                        param[t, uf, q, 0, 1] = -delay_est_00[q]
+                        params[t, uf, q, 0, 0] = -delay_est_00[q]
                         if n_corr > 1:
-                            param[t, uf, q, 0, 3] = -delay_est_11[q]
+                            params[t, uf, q, 0, 1] = -delay_est_11[q]
                     else:
-                        param[t, uf, p, 0, 1] = delay_est_00[p]
+                        params[t, uf, p, 0, 0] = delay_est_00[p]
                         if n_corr > 1:
-                            param[t, uf, p, 0, 3] = delay_est_11[p]
+                            params[t, uf, p, 0, 1] = delay_est_11[p]
 
-        for ut in utint:
-            for f in range(n_chan):
-                fm = f_map[f]
-                cf = 2j * np.pi * chan_freq[f]
+        delay_params_to_gains(
+            params,
+            gains,
+            ms_kwargs["CHAN_FREQ"],
+            term_kwargs[f"{self.name}_param_freq_map"],
+        )
 
-                gain[ut, f, :, :, 0] = np.exp(cf * param[ut, fm, :, :, 1])
+        apply_param_flags_to_params(param_flags, params, 0)
+        apply_gain_flags_to_gains(gain_flags, gains)
 
-                if n_corr > 1:
-                    gain[ut, f, :, :, -1] = np.exp(cf * param[ut, fm, :, :, 3])
+        return gains, gain_flags, params, param_flags
```

### Comparing `quartical-0.1.9/quartical/gains/delay/kernel.py` & `quartical-0.2.0/quartical/gains/phase/kernel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,206 +1,246 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
+from numba import prange, njit
+from numba.extending import overload
+from quartical.utils.numba import (coerce_literal,
+                                   JIT_OPTIONS,
+                                   PARALLEL_JIT_OPTIONS)
 from quartical.gains.general.generics import (native_intermediaries,
                                               upsampled_itermediaries,
                                               per_array_jhj_jhr,
                                               resample_solints,
                                               downsample_jhj_jhr)
 from quartical.gains.general.flagging import (flag_intermediaries,
                                               update_gain_flags,
                                               finalize_gain_flags,
-                                              apply_gain_flags,
-                                              update_param_flags)
+                                              apply_gain_flags_to_flag_col,
+                                              update_param_flags,
+                                              apply_gain_flags_to_gains,
+                                              apply_param_flags_to_params)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
-
-
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
-
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
-
-delay_args = namedtuple(
-    "delay_args",
-    (
-        "params",
-        "param_flags",
-        "chan_freqs",
-        "t_bin_arr"
-    )
-)
 
 
 def get_identity_params(corr_mode):
 
     if corr_mode.literal_value in (2, 4):
-        return np.zeros((4,), dtype=np.float64)
-    elif corr_mode.literal_value == 1:
         return np.zeros((2,), dtype=np.float64)
+    elif corr_mode.literal_value == 1:
+        return np.zeros((1,), dtype=np.float64)
     else:
         raise ValueError("Unsupported number of correlations.")
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def delay_solver(base_args, term_args, meta_args, corr_mode):
+@njit(**JIT_OPTIONS)
+def phase_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return phase_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
+
 
-    coerce_literal(delay_solver, ["corr_mode"])
+def phase_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(phase_solver_impl, jit_options=JIT_OPTIONS)
+def nb_phase_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+
+    coerce_literal(nb_phase_solver_impl, ["corr_mode"])
 
     identity_params = get_identity_params(corr_mode)
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
-        active_params = term_args.params[active_term]
+        active_params = chain_inputs.params[active_term]
 
         # Set up some intemediaries used for flagging.
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
         abs2_diffs_trend = np.zeros_like(active_gain_flags, dtype=np.float64)
         flag_imdry = \
             flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
 
         # Set up some intemediaries used for solving.
         real_dtype = active_gain.real.dtype
         param_shape = active_params.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_p = base_args.f_map_arr[1, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_g = mapping_inputs.freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, param_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
-        extents = get_extents(resampler.upsample_t_map, active_f_map_p)
+        extents = get_extents(resampler.upsample_t_map, active_f_map_g)
 
         upsample_shape = resampler.upsample_shape
         upsampled_jhj = np.empty(upsample_shape + (upsample_shape[-1],),
                                  dtype=real_dtype)
         upsampled_jhr = np.empty(upsample_shape, dtype=real_dtype)
         jhj = upsampled_jhj[:param_shape[0]]
         jhr = upsampled_jhr[:param_shape[0]]
         update = np.zeros(param_shape, dtype=real_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        scaled_cf = term_args.chan_freqs.copy()  # Don't mutate.
-        min_freq = np.min(scaled_cf)
-        scaled_cf /= min_freq  # Scale freqs to avoid precision.
-        active_params[..., 1::2] *= min_freq  # Scale delay consistently.
-        scaled_cf *= 2*np.pi  # Introduce 2pi here - neglect everywhere else.
-
-        for loop_idx in range(max_iter):
-
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            scaled_cf,
-                            corr_mode)
+        for loop_idx in range(max_iter or 1):
+
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
             compute_update(native_imdry,
                            corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            scaled_cf,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode,
-                                          numbness=1e9)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode,
+                numbness=1e9
+            )
 
             # Propagate gain flags to parameter flags.
-            update_param_flags(base_args,
-                               term_args,
-                               meta_args,
-                               identity_params)
+            update_param_flags(
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                identity_params
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
+
+        reference_params(chain_inputs, meta_inputs)
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
-
-        active_params[..., 1::2] /= min_freq  # Undo scaling for SI units.
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
-    scaled_cf,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     absv1_idiv_absv2 = factories.absv1_idiv_absv2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
@@ -208,60 +248,61 @@
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
-        scaled_cf,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
+
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        dir_maps = mapping_inputs.dir_maps
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        antenna1 = base_args.a1
-        antenna2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr_g = base_args.f_map_arr[0]
-        d_map_arr = base_args.d_map_arr
+        gains = chain_inputs.gains
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
-        row_starts = extents.row_starts
-        row_stops = extents.row_stops
-        chan_starts = extents.chan_starts
-        chan_stops = extents.chan_stops
-
         _, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
         jhr[:] = 0
 
         n_tint, n_fint, n_ant, n_gdir, n_param = jhr.shape
         n_int = n_tint*n_fint
 
         complex_dtype = gains[active_term].dtype
         weight_dtype = weights.dtype
 
         n_gains = len(gains)
 
+        row_starts = extents.row_starts
+        row_stops = extents.row_stops
+        chan_starts = extents.chan_starts
+        chan_stops = extents.chan_stops
+
         # Determine loop variables based on where we are in the chain.
         # gt means greater than (n>j) and lt means less than (n<j).
         all_terms, gt_active, lt_active = make_loop_vars(n_gains, active_term)
 
         # Parallel over all solution intervals.
         for i in prange(n_int):
 
@@ -322,17 +363,17 @@
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr_g[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -359,15 +400,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -375,57 +416,53 @@
                         v1_imul_v2ct(v_pqd, rop_pq, v_pqd)
                         iadd(v_pq, v_pqd)
 
                     absv1_idiv_absv2(v_pq, r_pq, norm_factors)
                     imul(r_pq, norm_factors)
                     isub(r_pq, v_pq)
 
-                    nu = scaled_cf[f]
-
                     for d in range(n_gdir):
 
                         iunpack(wr_pq, r_pq)
                         imul(wr_pq, w)
                         iunpackct(wr_qp, wr_pq)
 
                         lop_pq_d = lop_pq_arr[d]
                         rop_pq_d = rop_pq_arr[d]
 
                         compute_jhwj_jhwr_elem(lop_pq_d,
                                                rop_pq_d,
                                                w,
                                                norm_factors,
-                                               nu,
                                                gains_p[active_term],
                                                wr_pq,
                                                jhr_tifi[a1_m, d],
                                                jhj_tifi[a1_m, d])
 
                         lop_qp_d = lop_qp_arr[d]
                         rop_qp_d = rop_qp_arr[d]
 
                         compute_jhwj_jhwr_elem(lop_qp_d,
                                                rop_qp_d,
                                                w,
                                                norm_factors,
-                                               nu,
                                                gains_q[active_term],
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -456,77 +493,94 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, scaled_cf,
-                    loop_idx, corr_mode):
+def finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
 
     set_identity = factories.set_identity_factory(corr_mode)
     param_to_gain = param_to_gain_factory(corr_mode)
 
-    if corr_mode.literal_value in (1, 2, 4):
-        def impl(base_args, term_args, meta_args, native_imdry, scaled_cf,
-                 loop_idx, corr_mode):
-
-            active_term = meta_args.active_term
-
-            gain = base_args.gains[active_term]
-            gain_flags = base_args.gain_flags[active_term]
-            f_map_arr_p = base_args.f_map_arr[1, :, active_term]
-            d_map_arr = base_args.d_map_arr[active_term, :]
-
-            params = term_args.params[active_term]
-
-            update = native_imdry.update
-
-            update /= 2
-            params += update
-
-            n_time, n_freq, n_ant, n_dir, _ = gain.shape
-
-            for t in range(n_time):
-                for f in range(n_freq):
-                    cf = scaled_cf[f]
-                    f_m = f_map_arr_p[f]
-                    for a in range(n_ant):
-                        for d in range(n_dir):
-
-                            d_m = d_map_arr[d]
-                            g = gain[t, f, a, d]
-                            fl = gain_flags[t, f, a, d]
-                            p = params[t, f_m, a, d_m]
-
-                            if fl == 1:
-                                set_identity(g)
-                            else:
-                                param_to_gain(p, cf, g)
-    else:
-        raise ValueError("Unsupported number of correlations.")
+    def impl(
+        chain_inputs,
+        meta_inputs,
+        native_imdry,
+        loop_idx,
+        corr_mode
+    ):
+
+        dd_term = meta_inputs.dd_term
+        active_term = meta_inputs.active_term
+        pinned_directions = meta_inputs.pinned_directions
+
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
+        params = chain_inputs.params[active_term]
+
+        update = native_imdry.update
+
+        n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
+
+        if dd_term:
+            dir_loop = [d for d in range(n_dir) if d not in pinned_directions]
+        else:
+            dir_loop = [d for d in range(n_dir)]
+
+        for ti in range(n_tint):
+            for fi in range(n_fint):
+                for a in range(n_ant):
+                    for d in dir_loop:
+
+                        p = params[ti, fi, a, d]
+                        g = gain[ti, fi, a, d]
+                        fl = gain_flags[ti, fi, a, d]
+                        upd = update[ti, fi, a, d]
+
+                        if fl == 1:
+                            p[:] = 0
+                            set_identity(g)
+                        else:
+                            p += upd
+                            param_to_gain(p, g)
 
     return impl
 
 
 def param_to_gain_factory(corr_mode):
 
     if corr_mode.literal_value == 4:
-        def impl(params, chanfreq, gain):
-            gain[0] = np.exp(1j*(chanfreq*params[1] + params[0]))
-            gain[3] = np.exp(1j*(chanfreq*params[3] + params[2]))
+        def impl(params, gain):
+            gain[0] = np.exp(1j*params[0])
+            gain[3] = np.exp(1j*params[1])
     elif corr_mode.literal_value == 2:
-        def impl(params, chanfreq, gain):
-            gain[0] = np.exp(1j*(chanfreq*params[1] + params[0]))
-            gain[1] = np.exp(1j*(chanfreq*params[3] + params[2]))
+        def impl(params, gain):
+            gain[0] = np.exp(1j*params[0])
+            gain[1] = np.exp(1j*params[1])
     elif corr_mode.literal_value == 1:
-        def impl(params, chanfreq, gain):
-            gain[0] = np.exp(1j*(chanfreq*params[1] + params[0]))
+        def impl(params, gain):
+            gain[0] = np.exp(1j*params[0])
     else:
         raise ValueError("Unsupported number of correlations.")
 
     return factories.qcjit(impl)
 
 
 def compute_jhwj_jhwr_elem_factory(corr_mode):
@@ -535,15 +589,15 @@
     unpack = factories.unpack_factory(corr_mode)
     unpackc = factories.unpackc_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iabsdivsq = factories.iabsdivsq_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
 
     if corr_mode.literal_value == 4:
-        def impl(lop, rop, w, normf, nu, gain, res, jhr, jhj):
+        def impl(lop, rop, w, normf, gain, res, jhr, jhj):
 
             # Effectively apply zero weight to off-diagonal terms.
             # TODO: Can be tidied but requires moving other weighting code.
             res[1] = 0
             res[2] = 0
 
             # Compute normalization factor.
@@ -559,29 +613,26 @@
 
             r_0, _, _, r_3 = unpack(res)  # NOTE: XX, XY, YX, YY
 
             _, _, _, g_3 = unpack(gain)
             gc_0, _, _, gc_3 = unpackc(gain)
 
             drv_00 = -1j*gc_0
-            drv_23 = -1j*gc_3
+            drv_13 = -1j*gc_3
 
             upd_00 = (drv_00*r_0).real
-            upd_11 = (drv_23*r_3).real
+            upd_11 = (drv_13*r_3).real
 
             jhr[0] += upd_00
-            jhr[1] += nu*upd_00
-            jhr[2] += upd_11
-            jhr[3] += nu*upd_11
+            jhr[1] += upd_11
 
             w_0, _, _, w_3 = unpack(w)  # NOTE: XX, XY, YX, YY
             n_0, _, _, n_3 = unpack(normf)
 
-            # Apply normalisation factors by scaling w. # Neglect (set weight
-            # to zero) off diagonal terms.
+            # Apply normalisation factors by scaling w.
             w_0 = n_0 * w_0
             w_3 = n_3 * w_3
 
             lop_00, lop_01, lop_10, lop_11 = unpack(lop)
             rop_00, rop_10, rop_01, rop_11 = unpack(rop)  # "Transpose"
 
             jh_00 = lop_00 * rop_00
@@ -596,41 +647,21 @@
             j_30 = jh_30.conjugate()
             j_33 = jh_33.conjugate()
 
             jhwj_00 = jh_00*w_0*j_00 + jh_03*w_3*j_03
             jhwj_03 = jh_00*w_0*j_30 + jh_03*w_3*j_33
             jhwj_33 = jh_30*w_0*j_30 + jh_33*w_3*j_33
 
-            nusq = nu * nu
-
-            tmp_0 = jhwj_00.real
-            jhj[0, 0] += tmp_0
-            jhj[0, 1] += tmp_0*nu
-            tmp_1 = (jhwj_03*gc_0*g_3).real
-            jhj[0, 2] += tmp_1
-            jhj[0, 3] += tmp_1*nu
-
+            jhj[0, 0] += jhwj_00.real
+            jhj[0, 1] += (gc_0*jhwj_03*g_3).real
             jhj[1, 0] = jhj[0, 1]
-            jhj[1, 1] += tmp_0*nusq
-            jhj[1, 2] = jhj[0, 3]
-            jhj[1, 3] += tmp_1*nusq
-
-            jhj[2, 0] = jhj[0, 2]
-            jhj[2, 1] = jhj[1, 2]
-            tmp_2 = jhwj_33.real
-            jhj[2, 2] += tmp_2
-            jhj[2, 3] += tmp_2*nu
-
-            jhj[3, 0] = jhj[0, 3]
-            jhj[3, 1] = jhj[1, 3]
-            jhj[3, 2] = jhj[2, 3]
-            jhj[3, 3] += tmp_2*nusq
+            jhj[1, 1] += jhwj_33.real
 
     elif corr_mode.literal_value == 2:
-        def impl(lop, rop, w, normf, nu, gain, res, jhr, jhj):
+        def impl(lop, rop, w, normf, gain, res, jhr, jhj):
 
             # Compute normalization factor.
             iunpack(normf, rop)
             iabsdivsq(normf)
             imul(res, normf)  # Apply normalization factor to r.
 
             # Accumulate an element of jhwr.
@@ -642,40 +673,28 @@
             drv_00 = -1j*gc_0
             drv_23 = -1j*gc_1
 
             upd_00 = (drv_00*r_0).real
             upd_11 = (drv_23*r_1).real
 
             jhr[0] += upd_00
-            jhr[1] += nu*upd_00
-            jhr[2] += upd_11
-            jhr[3] += nu*upd_11
+            jhr[1] += upd_11
 
             # Accumulate an element of jhwj.
             jh_00, jh_11 = unpack(rop)
             j_00, j_11 = unpackc(rop)
             w_00, w_11 = unpack(w)
             n_00, n_11 = unpack(normf)
 
-            nusq = nu*nu
-
-            tmp = (jh_00*n_00*w_00*j_00).real
-            jhj[0, 0] += tmp
-            jhj[0, 1] += tmp*nu
-            jhj[1, 0] += tmp*nu
-            jhj[1, 1] += tmp*nusq
-
-            tmp = (jh_11*n_11*w_11*j_11).real
-            jhj[2, 2] += tmp
-            jhj[2, 3] += tmp*nu
-            jhj[3, 2] += tmp*nu
-            jhj[3, 3] += tmp*nusq
+            # TODO: Consider representing as a vector?
+            jhj[0, 0] += (jh_00*n_00*w_00*j_00).real
+            jhj[1, 1] += (jh_11*n_11*w_11*j_11).real
 
     elif corr_mode.literal_value == 1:
-        def impl(lop, rop, w, normf, nu, gain, res, jhr, jhj):
+        def impl(lop, rop, w, normf, gain, res, jhr, jhj):
 
             # Compute normalization factor.
             iunpack(normf, rop)
             iabsdivsq(normf)
             imul(res, normf)  # Apply normalization factor to r.
 
             # Accumulate an element of jhwr.
@@ -685,26 +704,76 @@
             gc_0 = unpackc(gain)
 
             drv_00 = -1j*gc_0
 
             upd_00 = (drv_00*r_0).real
 
             jhr[0] += upd_00
-            jhr[1] += nu*upd_00
 
             # Accumulate an element of jhwj.
             jh_00 = unpack(rop)
             j_00 = unpackc(rop)
             w_00 = unpack(w)
             n_00 = unpack(normf)
 
-            nusq = nu*nu
-
-            tmp = (jh_00*n_00*w_00*j_00).real
-            jhj[0, 0] += tmp
-            jhj[0, 1] += tmp*nu
-            jhj[1, 0] += tmp*nu
-            jhj[1, 1] += tmp*nusq
+            jhj[0, 0] += (jh_00*n_00*w_00*j_00).real
     else:
         raise ValueError("Unsupported number of correlations.")
 
     return factories.qcjit(impl)
+
+
+@njit(**JIT_OPTIONS)
+def phase_params_to_gains(
+    params,
+    gains
+):
+
+    n_time, n_freq, n_ant, n_dir, n_corr = gains.shape
+
+    for t in range(n_time):
+        for f in range(n_freq):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    g = gains[t, f, a, d]
+                    p = params[t, f, a, d]
+
+                    g[0] = np.exp(1j*p[0])
+
+                    if n_corr > 1:
+                        g[-1] = np.exp(1j*p[-1])
+
+
+@njit(**JIT_OPTIONS)
+def reference_params(chain_inputs, meta_inputs):
+
+    active_term = meta_inputs.active_term
+    ref_ant = meta_inputs.reference_antenna
+
+    gains = chain_inputs.gains[active_term]
+    gain_flags = chain_inputs.gain_flags[active_term]
+    params = chain_inputs.params[active_term]
+    param_flags = chain_inputs.param_flags[active_term]
+
+    n_ti, n_fi, n_ant, n_dir, n_corr = params.shape
+
+    ref_params = params[:, :, ref_ant: ref_ant + 1, :, :].copy()
+
+    for t in range(n_ti):
+        for f in range(n_fi):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    p = params[t, f, a, d]
+                    rp = ref_params[t, f, 0, d]
+
+                    if param_flags[t, f, a, d] == 1:
+                        continue
+                    else:
+                        p -= rp
+
+    phase_params_to_gains(params, gains)
+
+    # Referencing may move flagged gains/params from identity.
+    apply_param_flags_to_params(param_flags, params, 0)
+    apply_gain_flags_to_gains(gain_flags, gains)
```

### Comparing `quartical-0.1.9/quartical/gains/general/convenience.py` & `quartical-0.2.0/quartical/gains/general/convenience.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 # -*- coding: utf-8 -*-
-from numba import jit, types, generated_jit
+from numba import njit, types
+from numba.extending import overload
+from quartical.utils.numba import JIT_OPTIONS
 import numpy as np
 from collections import namedtuple
 
 
 extent_tuple = namedtuple(
     "extent_tuple",
     (
         "row_starts",
         "row_stops",
         "chan_starts",
         "chan_stops"
     )
 )
 
-# Handy alias for functions that need to be jitted in this way.
-qcjit = jit(nogil=True,
-            nopython=True,
-            fastmath=True,
-            cache=True,
-            inline="always")
-
-qcgjit = generated_jit(nogil=True,
-                       nopython=True,
-                       fastmath=True,
-                       cache=True)
 
 # TODO: Consider whether these should have true optionals. This will likely
-# require them all to be implemented as overloads.
+# require them all to be implemented as overloads. We could also consider
+# moving this code into the factories.
 
 
-@qcgjit
+@njit(**JIT_OPTIONS)
 def get_dims(col, row_map):
+    return get_dims_impl(col, row_map)
+
+
+def get_dims_impl(col, row_map):
+    return NotImplementedError
+
+
+@overload(get_dims_impl, jit_options=JIT_OPTIONS)
+def nb_get_dims_impl(col, row_map):
     """Returns effective column dimensions. This may be larger than col.
 
     Args:
         col: A numpy.ndrray containing column-like data.
         row_map: A nominal to effective row mapping. If not None, the returned
             shape will have the effective number of rows.
 
@@ -55,16 +56,25 @@
             def impl(col, row_map):
                 _, n_chan, n_corr = col.shape
                 return (row_map.size, n_chan, n_corr)
 
     return impl
 
 
-@qcgjit
+@njit(**JIT_OPTIONS)
 def get_row(row_ind, row_map):
+    return get_row_impl(row_ind, row_map)
+
+
+def get_row_impl(row_ind, row_map):
+    return NotImplementedError
+
+
+@overload(get_row_impl, jit_options=JIT_OPTIONS)
+def nb_get_row_impl(row_ind, row_map):
     """Gets the current row index. Row map is needed for the BDA case.
 
     Args:
         row_ind: Integer index of current row.
         row_map: A nominal to effective row mapping.
 
     Returns:
@@ -76,25 +86,25 @@
     else:
         def impl(row_ind, row_map):
             return row_map[row_ind]
 
     return impl
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def get_extents(t_map, f_map):
     """Given the time/freq mappings, determine run start and stop indices."""
 
     row_starts, row_stops = get_row_extents(t_map)
     chan_starts, chan_stops = get_chan_extents(f_map)
 
     return extent_tuple(row_starts, row_stops, chan_starts, chan_stops)
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def get_chan_extents(f_map_arr):
     """Given the frequency mappings, determines the start/stop indices."""
 
     n_fint = f_map_arr.max() + 1
     n_chan = f_map_arr.size
 
     chan_starts = np.empty(n_fint, dtype=np.int32)
@@ -107,15 +117,15 @@
     if n_fint > 1:
         chan_starts[1:] = 1 + np.where(f_map_arr[1:] - f_map_arr[:-1])[0]
         chan_stops[:-1] = chan_starts[1:]
 
     return chan_starts, chan_stops
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def get_row_extents(t_map_arr):
     """Given the time mappings, determines the row start/stop indices."""
 
     n_tint = t_map_arr.max() + 1
 
     row_starts = np.empty(n_tint, dtype=np.int32)
     row_starts[0] = 0
```

### Comparing `quartical-0.1.9/quartical/gains/general/factories.py` & `quartical-0.2.0/quartical/gains/general/factories.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 # -*- coding: utf-8 -*-
-from numba import jit, types
 import numpy as np
+from numba import njit, types
+from quartical.utils.numba import JIT_OPTIONS
+
 
 # Handy alias for functions that need to be jitted in this way.
-qcjit = jit(nogil=True,
-            nopython=True,
-            fastmath=True,
-            cache=True,
-            inline="always")
+qcjit = njit(**JIT_OPTIONS, inline="always")
 
 
 def imul_rweight_factory(mode, weight):
 
     if isinstance(weight, types.NoneType):
         if mode.literal_value == 4:
             def impl(invec, outvec, weight, ind):
```

### Comparing `quartical-0.1.9/quartical/gains/general/flagging.py` & `quartical-0.2.0/quartical/gains/general/flagging.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,88 +1,84 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import jit, generated_jit
+from numba import njit
+from numba.extending import overload
+from quartical.utils.numba import coerce_literal, JIT_OPTIONS
 from collections import namedtuple
 from quartical.gains.general.convenience import get_row
 import quartical.gains.general.factories as factories
-from quartical.utils.numba import coerce_literal
 
 
 flag_intermediaries = namedtuple(
     "flag_intermediaries",
     (
         "km1_gain",
         "km1_abs2_diffs",
         "abs2_diffs_trend"
     )
 
 )
 
 
-def init_gain_flags(term_shape, term_ind, **kwargs):
-    """Initialise the gain flags for a term using the various mappings."""
-
-    flag_col = kwargs["flags"]
-    ant1_col = kwargs["a1"]
-    ant2_col = kwargs["a2"]
-    t_map_arr = kwargs["t_map_arr"][0]
-    f_map_arr = kwargs["f_map_arr"][0]
-    row_map = kwargs.get("row_map", None)
-
-    return _init_flags(term_shape, term_ind, flag_col, ant1_col, ant2_col,
-                       t_map_arr, f_map_arr, row_map)
-
-
-def init_param_flags(term_shape, term_ind, **kwargs):
-    """Initialise the param flags for a term using the various mappings."""
-
-    flag_col = kwargs["flags"]
-    ant1_col = kwargs["a1"]
-    ant2_col = kwargs["a2"]
-    t_map_arr = kwargs["t_map_arr"][1]
-    f_map_arr = kwargs["f_map_arr"][1]
-    row_map = kwargs.get("row_map", None)
-
-    return _init_flags(term_shape, term_ind, flag_col, ant1_col, ant2_col,
-                       t_map_arr, f_map_arr, row_map)
-
-
-@jit(nopython=True, fastmath=True, parallel=False, cache=True, nogil=True)
-def _init_flags(term_shape, term_ind, flag_col, ant1_col, ant2_col,
-                t_map_arr, f_map_arr, row_map):
+@njit(**JIT_OPTIONS)
+def init_flags(
+    term_shape,
+    time_map,
+    freq_map,
+    flag_col,
+    ant1_col,
+    ant2_col,
+    row_map
+):
     """Initialise the flags for a term using the various mappings."""
 
     flags = np.ones(term_shape[:-1], dtype=np.int8)
     _, _, _, n_dir, _ = term_shape
 
-    n_row = t_map_arr.shape[0]
-    n_chan = f_map_arr.shape[0]
+    n_row = time_map.shape[0]
+    n_chan = freq_map.shape[0]
 
     for row_ind in range(n_row):
-        ti = t_map_arr[row_ind, term_ind]
+        ti = time_map[row_ind]
 
         # NOTE: The following handles the BDA case where an element in the
         # time map may be backed by a different row in the data.
         row = get_row(row_ind, row_map)
         a1, a2 = ant1_col[row], ant2_col[row]
 
         for f in range(n_chan):
-            fi = f_map_arr[f, term_ind]
+            fi = freq_map[f]
             flag = flag_col[row, f]
             for d in range(n_dir):
                 flags[ti, fi, a1, d] &= flag
                 flags[ti, fi, a2, d] &= flag
 
     return flags
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def update_gain_flags(base_args, term_args, meta_args, flag_imdry, loop_idx,
-                      corr_mode, numbness=1e-6):
+def update_gain_flags(
+    chain_inputs,
+    meta_inputs,
+    flag_imdry,
+    loop_idx,
+    corr_mode,
+    numbness=1e-6
+):
+    raise NotImplementedError
+
+
+@overload(update_gain_flags, jit_options=JIT_OPTIONS)
+def nb_update_gain_flags(
+    chain_inputs,
+    meta_inputs,
+    flag_imdry,
+    loop_idx,
+    corr_mode,
+    numbness=1e-6
+):
     """Update the current state of the gain flags.
 
     Uses the current (km0) and previous (km1) gains to identify diverging
     soultions. This implements trendy flagging - see overleaf document.
     TODO: Add link.
 
     Args:
@@ -95,35 +91,34 @@
             accumulated trend values of the differences between absolute
             differences of the gains.
         critera: A float value below which a gain is considered converged.
         corr_mode: An int which controls how we handle coreelations.
         iteration: An int containing the iteration number.
     """
 
-    coerce_literal(update_gain_flags, ['corr_mode'])
+    coerce_literal(nb_update_gain_flags, ['corr_mode'])
 
     set_identity = factories.set_identity_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        chain_inputs,
+        meta_inputs,
         flag_imdry,
         loop_idx,
         corr_mode,
         numbness=1e-6
     ):
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        stop_frac = meta_args.stop_frac
-        stop_crit2 = meta_args.stop_crit**2
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        stop_frac = meta_inputs.stop_frac
+        stop_crit2 = meta_inputs.stop_crit**2
 
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
 
         km1_gain = flag_imdry.km1_gain
         km1_abs2_diffs = flag_imdry.km1_abs2_diffs
         abs2_diffs_trend = flag_imdry.abs2_diffs_trend
 
         n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
 
@@ -210,17 +205,20 @@
             km1_gain[:] = gain
 
         return conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_gain_flags(base_args, meta_args, flag_imdry, corr_mode):
+def finalize_gain_flags(chain_inputs, meta_inputs, flag_imdry, corr_mode):
+    return NotImplementedError
+
+
+@overload(finalize_gain_flags, jit_options=JIT_OPTIONS)
+def nb_finalize_gain_flags(chain_inputs, meta_inputs, flag_imdry, corr_mode):
     """Removes soft flags and flags points which failed to converge.
 
     Given the gains, assosciated gain flags and the trend of abosolute
     differences, remove soft flags which were never hardened and hard flag
     points which have positive trend values. This corresponds to points
     which have bad solutions when convergence/maximum iterations are reached.
 
@@ -228,22 +226,24 @@
         gain: A (ti, fi, a, d, c) array of gain values.
         gain_flags: A (ti, fi, a, d) array of flag values.
         ab2_diffs_trends: An array containing the accumulated trend values of
             the absolute difference between gains at each iteration. Positive
             values correspond to points which are nowhere near convergence.
     """
 
+    coerce_literal(nb_finalize_gain_flags, ['corr_mode'])
+
     set_identity = factories.set_identity_factory(corr_mode)
 
-    def impl(base_args, meta_args, flag_imdry, corr_mode):
+    def impl(chain_inputs, meta_inputs, flag_imdry, corr_mode):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
+        gain = chain_inputs.gains[active_term]
+        gain_flags = chain_inputs.gain_flags[active_term]
 
         abs2_diffs_trend = flag_imdry.abs2_diffs_trend
 
         n_tint, n_fint, n_ant, n_dir = gain_flags.shape
 
         for ti in range(n_tint):
             for fi in range(n_fint):
@@ -254,52 +254,72 @@
                             set_identity(gain[ti, fi, a, d])
                         elif gain_flags[ti, fi, a, d] == -1:
                             gain_flags[ti, fi, a, d] = 0
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def update_param_flags(base_args, term_args, meta_args, identity_params):
+def update_param_flags(
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    identity_params
+):
+    return NotImplementedError
+
+
+@overload(update_param_flags, jit_options=JIT_OPTIONS)
+def update_param_flags_impl(
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    identity_params
+):
     """Propagate gain flags into parameter flags.
 
     Given the gain flags, parameter flags and the relevant mappings, propagate
     gain flags into parameter flags. NOTE: This may not be the best approach.
     We could flag on the parameters directly but this is difficult due to
     having a variable set of identitiy paramters and no reason to believe that
     the parameters live on the same scale.
 
     Args:
         gain_flags: A (gti, gfi, a, d) array of gain flags.
         param_flags: A (pti, pfi, a, d) array of paramter flag values.
         t_bin_arr: A (2, n_utime, n_term) array of utime to solint mappings.
         f_map_arr: A (2, n_ufreq, n_term) array of ufreq to solint mappings.
         d_map_arr: A (n_term, n_dir) array of direction mappings.
-        """
+    """
 
-    def impl(base_args, term_args, meta_args, identity_params):
+    def impl(
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        identity_params
+    ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
         # NOTE: We don't yet let params and gains have different direction
         # maps but this will eventually be neccessary.
-        t_bin_arr = term_args.t_bin_arr[:, :, active_term]
-        f_map_arr = base_args.f_map_arr[:, :, active_term]
-
-        gain_flags = base_args.gain_flags[active_term]
-        param_flags = term_args.param_flags[active_term]
-        params = term_args.params[active_term]
+        time_bins = mapping_inputs.time_bins[active_term]
+        param_time_bins = mapping_inputs.param_time_bins[active_term]
+        freq_maps = mapping_inputs.freq_maps[active_term]
+        param_freq_maps = mapping_inputs.param_freq_maps[active_term]
+
+        gain_flags = chain_inputs.gain_flags[active_term]
+        param_flags = chain_inputs.param_flags[active_term]
+        params = chain_inputs.params[active_term]
 
         _, _, n_ant, n_dir = gain_flags.shape
 
         param_flags[:] = 1
 
-        for gt, pt in zip(t_bin_arr[0], t_bin_arr[1]):
-            for gf, pf in zip(f_map_arr[0], f_map_arr[1]):
+        for gt, pt in zip(time_bins, param_time_bins):
+            for gf, pf in zip(freq_maps, param_freq_maps):
                 for a in range(n_ant):
                     for d in range(n_dir):
 
                         flag = gain_flags[gt, gf, a, d] == 1
                         param_flags[pt, pf, a, d] &= flag
 
         n_tint, n_fint, n_ant, n_dir = param_flags.shape
@@ -310,33 +330,74 @@
                     for d in range(n_dir):
                         if param_flags[ti, fi, a, d] == 1:
                             params[ti, fi, a, d] = identity_params
 
     return impl
 
 
-@jit(nopython=True, fastmath=True, parallel=False, cache=True, nogil=True)
-def apply_gain_flags(base_args, meta_args):
+@njit(**JIT_OPTIONS)
+def apply_gain_flags_to_flag_col(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs
+):
     """Apply gain_flags to flag_col."""
 
-    active_term = meta_args.active_term
+    active_term = meta_inputs.active_term
 
-    gain_flags = base_args.gain_flags[active_term]
-    flag_col = base_args.flags
-    ant1_col = base_args.a1
-    ant2_col = base_args.a2
+    gain_flags = chain_inputs.gain_flags[active_term]
+
+    flag_col = ms_inputs.FLAG
+    ant1_col = ms_inputs.ANTENNA1
+    ant2_col = ms_inputs.ANTENNA2
 
     # Select out just the mappings we need.
-    t_map_arr = base_args.t_map_arr[0, :, active_term]
-    f_map_arr = base_args.f_map_arr[0, :, active_term]
+    t_map_arr = mapping_inputs.time_maps[active_term]
+    f_map_arr = mapping_inputs.freq_maps[active_term]
 
     n_row, n_chan = flag_col.shape
 
     for row in range(n_row):
         a1, a2 = ant1_col[row], ant2_col[row]
         t_m = t_map_arr[row]
         for f in range(n_chan):
             f_m = f_map_arr[f]
 
             # NOTE: We only care about the DI case for now.
             flag_col[row, f] |= gain_flags[t_m, f_m, a1, 0] == 1
             flag_col[row, f] |= gain_flags[t_m, f_m, a2, 0] == 1
+
+
+@njit(**JIT_OPTIONS)
+def apply_gain_flags_to_gains(gain_flags, gains):
+
+    n_time, n_chan, n_ant, n_dir, n_corr = gains.shape
+
+    if n_corr == 4:
+        identity_element = np.array([1, 0, 0, 1], dtype=np.complex128)
+    elif n_corr == 2:
+        identity_element = np.array([1, 1], dtype=np.complex128)
+    else:
+        identity_element = np.array([1], dtype=np.complex128)
+
+    for t in range(n_time):
+        for f in range(n_chan):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    if gain_flags[t, f, a, d]:
+                        gains[t, f, a, d] = identity_element
+
+
+@njit(**JIT_OPTIONS)
+def apply_param_flags_to_params(param_flags, params, identity_element):
+
+    n_time, n_chan, n_ant, n_dir, n_corr = params.shape
+
+    for t in range(n_time):
+        for f in range(n_chan):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    if param_flags[t, f, a, d]:
+                        params[t, f, a, d] = identity_element
```

### Comparing `quartical-0.1.9/quartical/gains/general/inversion.py` & `quartical-0.2.0/quartical/gains/general/inversion.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/gains/phase/kernel.py` & `quartical-0.2.0/quartical/gains/delay/kernel.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,193 +1,268 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
-from quartical.gains.general.generics import (native_intermediaries,
-                                              upsampled_itermediaries,
-                                              per_array_jhj_jhr,
-                                              resample_solints,
-                                              downsample_jhj_jhr)
-from quartical.gains.general.flagging import (flag_intermediaries,
-                                              update_gain_flags,
-                                              finalize_gain_flags,
-                                              apply_gain_flags,
-                                              update_param_flags)
+from numba import njit, prange
+from numba.extending import overload
+from quartical.utils.numba import (
+    coerce_literal,
+    JIT_OPTIONS,
+    PARALLEL_JIT_OPTIONS
+)
+from quartical.gains.general.generics import (
+    native_intermediaries,
+    upsampled_itermediaries,
+    per_array_jhj_jhr,
+    resample_solints,
+    downsample_jhj_jhr
+)
+from quartical.gains.general.flagging import (
+    flag_intermediaries,
+    update_gain_flags,
+    finalize_gain_flags,
+    apply_gain_flags_to_flag_col,
+    update_param_flags,
+    apply_gain_flags_to_gains,
+    apply_param_flags_to_params
+)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
-
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
-
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
-
-phase_args = namedtuple(
-    "phase_args",
-    (
-        "params",
-        "param_flags",
-        "t_bin_arr"
-    )
-)
 
 
 def get_identity_params(corr_mode):
 
     if corr_mode.literal_value in (2, 4):
         return np.zeros((2,), dtype=np.float64)
     elif corr_mode.literal_value == 1:
         return np.zeros((1,), dtype=np.float64)
     else:
         raise ValueError("Unsupported number of correlations.")
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def phase_solver(base_args, term_args, meta_args, corr_mode):
+@njit(**JIT_OPTIONS)
+def delay_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return delay_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
 
-    coerce_literal(phase_solver, ["corr_mode"])
+
+def delay_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(delay_solver_impl, jit_options=JIT_OPTIONS)
+def nb_delay_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+
+    coerce_literal(nb_delay_solver_impl, ["corr_mode"])
 
     identity_params = get_identity_params(corr_mode)
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
-        active_params = term_args.params[active_term]
+        active_params = chain_inputs.params[active_term]
 
         # Set up some intemediaries used for flagging.
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
         abs2_diffs_trend = np.zeros_like(active_gain_flags, dtype=np.float64)
         flag_imdry = \
             flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
 
         # Set up some intemediaries used for solving.
         real_dtype = active_gain.real.dtype
         param_shape = active_params.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_g = base_args.f_map_arr[0, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_p = mapping_inputs.param_freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, param_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
-        extents = get_extents(resampler.upsample_t_map, active_f_map_g)
+        extents = get_extents(resampler.upsample_t_map, active_f_map_p)
 
         upsample_shape = resampler.upsample_shape
         upsampled_jhj = np.empty(upsample_shape + (upsample_shape[-1],),
                                  dtype=real_dtype)
         upsampled_jhr = np.empty(upsample_shape, dtype=real_dtype)
         jhj = upsampled_jhj[:param_shape[0]]
         jhr = upsampled_jhr[:param_shape[0]]
         update = np.zeros(param_shape, dtype=real_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        for loop_idx in range(max_iter):
-
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            corr_mode)
+        # We actually solve for D' = (D(nu_min + nu_max))/2. This helps avoid
+        # numerical issues, but requires some scaling of the parameters.
+        chan_freq = ms_inputs.CHAN_FREQ
+        mid_freq = (chan_freq.min() + chan_freq.max())/2
+        active_params[:] *= mid_freq
+
+        for loop_idx in range(max_iter or 1):
+
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
-            compute_update(native_imdry,
-                           corr_mode)
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
+            compute_update(native_imdry, corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode,
-                                          numbness=1e9)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode,
+                numbness=1e9
+            )
 
             # Propagate gain flags to parameter flags.
-            update_param_flags(base_args,
-                               term_args,
-                               meta_args,
-                               identity_params)
+            update_param_flags(
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                identity_params
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
+
+        reference_params(
+            ms_inputs,
+            mapping_inputs,
+            chain_inputs,
+            meta_inputs,
+        )
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
+
+        # Undo rescaling so that quantities are in native units.
+        active_params[:] /= mid_freq
+        native_imdry.jhj[:] *= mid_freq ** 2
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     absv1_idiv_absv2 = factories.absv1_idiv_absv2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
@@ -195,58 +270,66 @@
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
+
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+        chan_freq = ms_inputs.CHAN_FREQ
+
+        # NOTE: These are the gain maps.
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        dir_maps = mapping_inputs.dir_maps
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        antenna1 = base_args.a1
-        antenna2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr = base_args.f_map_arr[0]  # We only need the gain mappings.
-        d_map_arr = base_args.d_map_arr
+        gains = chain_inputs.gains
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
-        _, n_chan, n_dir, n_corr = model.shape
+        row_starts = extents.row_starts
+        row_stops = extents.row_stops
+        chan_starts = extents.chan_starts
+        chan_stops = extents.chan_stops
+
+        n_row, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
         jhr[:] = 0
 
         n_tint, n_fint, n_ant, n_gdir, n_param = jhr.shape
         n_int = n_tint*n_fint
 
         complex_dtype = gains[active_term].dtype
         weight_dtype = weights.dtype
 
         n_gains = len(gains)
 
-        row_starts = extents.row_starts
-        row_stops = extents.row_stops
-        chan_starts = extents.chan_starts
-        chan_stops = extents.chan_stops
+        cf_min = chan_freq.min()
+        cf_max = chan_freq.max()
+        cf_mid = (cf_min + cf_max) / 2
 
         # Determine loop variables based on where we are in the chain.
         # gt means greater than (n>j) and lt means less than (n<j).
         all_terms, gt_active, lt_active = make_loop_vars(n_gains, active_term)
 
         # Parallel over all solution intervals.
         for i in prange(n_int):
@@ -308,17 +391,17 @@
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -345,15 +428,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -361,53 +444,58 @@
                         v1_imul_v2ct(v_pqd, rop_pq, v_pqd)
                         iadd(v_pq, v_pqd)
 
                     absv1_idiv_absv2(v_pq, r_pq, norm_factors)
                     imul(r_pq, norm_factors)
                     isub(r_pq, v_pq)
 
+                    # Coefficient introduced by differentiation of exponent.
+                    coeff = 2 * np.pi * (chan_freq[f]/cf_mid - 1)
+
                     for d in range(n_gdir):
 
                         iunpack(wr_pq, r_pq)
                         imul(wr_pq, w)
                         iunpackct(wr_qp, wr_pq)
 
                         lop_pq_d = lop_pq_arr[d]
                         rop_pq_d = rop_pq_arr[d]
 
                         compute_jhwj_jhwr_elem(lop_pq_d,
                                                rop_pq_d,
                                                w,
                                                norm_factors,
+                                               coeff,
                                                gains_p[active_term],
                                                wr_pq,
                                                jhr_tifi[a1_m, d],
                                                jhj_tifi[a1_m, d])
 
                         lop_qp_d = lop_qp_arr[d]
                         rop_qp_d = rop_qp_arr[d]
 
                         compute_jhwj_jhwr_elem(lop_qp_d,
                                                rop_qp_d,
                                                w,
                                                norm_factors,
+                                               coeff,
                                                gains_q[active_term],
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -438,69 +526,113 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, loop_idx,
-                    corr_mode):
-
-    set_identity = factories.set_identity_factory(corr_mode)
-    param_to_gain = param_to_gain_factory(corr_mode)
-
-    def impl(base_args, term_args, meta_args, native_imdry, loop_idx,
-             corr_mode):
-
-        active_term = meta_args.active_term
-
-        gain = base_args.gains[active_term]
-        gain_flags = base_args.gain_flags[active_term]
-
-        params = term_args.params[active_term]
+def finalize_update(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
+    raise NotImplementedError
 
-        update = native_imdry.update
 
-        n_tint, n_fint, n_ant, n_dir, n_corr = gain.shape
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    corr_mode
+):
 
-        for ti in range(n_tint):
-            for fi in range(n_fint):
-                for a in range(n_ant):
-                    for d in range(n_dir):
+    set_identity = factories.set_identity_factory(corr_mode)
+    param_to_gain = param_to_gain_factory(corr_mode)
 
-                        p = params[ti, fi, a, d]
-                        g = gain[ti, fi, a, d]
-                        fl = gain_flags[ti, fi, a, d]
-                        upd = update[ti, fi, a, d]
-
-                        if fl == 1:
-                            p[:] = 0
-                            set_identity(g)
-                        else:
-                            p += upd
-                            param_to_gain(p, g)
+    if corr_mode.literal_value in (1, 2, 4):
+        def impl(
+            ms_inputs,
+            mapping_inputs,
+            chain_inputs,
+            meta_inputs,
+            native_imdry,
+            loop_idx,
+            corr_mode
+        ):
+
+            dd_term = meta_inputs.dd_term
+            active_term = meta_inputs.active_term
+            pinned_directions = meta_inputs.pinned_directions
+
+            gain = chain_inputs.gains[active_term]
+            gain_flags = chain_inputs.gain_flags[active_term]
+            params = chain_inputs.params[active_term]
+
+            param_freq_map = mapping_inputs.param_freq_maps[active_term]
+            dir_map = mapping_inputs.dir_maps[active_term]
+
+            update = native_imdry.update
+
+            update /= 2
+            params += update
+
+            n_time, n_freq, n_ant, n_dir, _ = gain.shape
+
+            if dd_term:
+                for pd in pinned_directions:
+                    params[..., pd, :] = 0
+
+            chan_freq = ms_inputs.CHAN_FREQ
+            cf_min = chan_freq.min()
+            cf_max = chan_freq.max()
+            cf_mid = (cf_min + cf_max) / 2
+
+            for t in range(n_time):
+                for f in range(n_freq):
+                    f_m = param_freq_map[f]
+                    coeff = 2 * np.pi * (chan_freq[f]/cf_mid - 1)
+                    for a in range(n_ant):
+                        for d in range(n_dir):
+
+                            d_m = dir_map[d]
+                            g = gain[t, f, a, d]
+                            fl = gain_flags[t, f, a, d]
+                            p = params[t, f_m, a, d_m]
+
+                            if fl == 1:
+                                set_identity(g)
+                            else:
+                                param_to_gain(p, coeff, g)
+    else:
+        raise ValueError("Unsupported number of correlations.")
 
     return impl
 
 
 def param_to_gain_factory(corr_mode):
 
     if corr_mode.literal_value == 4:
-        def impl(params, gain):
-            gain[0] = np.exp(1j*params[0])
-            gain[3] = np.exp(1j*params[1])
+        def impl(params, coeff, gain):
+            gain[0] = np.exp(1j * coeff * params[0])
+            gain[3] = np.exp(1j * coeff * params[1])
     elif corr_mode.literal_value == 2:
-        def impl(params, gain):
-            gain[0] = np.exp(1j*params[0])
-            gain[1] = np.exp(1j*params[1])
+        def impl(params, coeff, gain):
+            gain[0] = np.exp(1j * coeff * params[0])
+            gain[1] = np.exp(1j * coeff * params[1])
     elif corr_mode.literal_value == 1:
-        def impl(params, gain):
-            gain[0] = np.exp(1j*params[0])
+        def impl(params, coeff, gain):
+            gain[0] = np.exp(1j * coeff * params[0])
     else:
         raise ValueError("Unsupported number of correlations.")
 
     return factories.qcjit(impl)
 
 
 def compute_jhwj_jhwr_elem_factory(corr_mode):
@@ -509,15 +641,15 @@
     unpack = factories.unpack_factory(corr_mode)
     unpackc = factories.unpackc_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iabsdivsq = factories.iabsdivsq_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
 
     if corr_mode.literal_value == 4:
-        def impl(lop, rop, w, normf, gain, res, jhr, jhj):
+        def impl(lop, rop, w, normf, coeff, gain, res, jhr, jhj):
 
             # Effectively apply zero weight to off-diagonal terms.
             # TODO: Can be tidied but requires moving other weighting code.
             res[1] = 0
             res[2] = 0
 
             # Compute normalization factor.
@@ -538,16 +670,16 @@
 
             drv_00 = -1j*gc_0
             drv_13 = -1j*gc_3
 
             upd_00 = (drv_00*r_0).real
             upd_11 = (drv_13*r_3).real
 
-            jhr[0] += upd_00
-            jhr[1] += upd_11
+            jhr[0] += coeff*upd_00
+            jhr[1] += coeff*upd_11
 
             w_0, _, _, w_3 = unpack(w)  # NOTE: XX, XY, YX, YY
             n_0, _, _, n_3 = unpack(normf)
 
             # Apply normalisation factors by scaling w.
             w_0 = n_0 * w_0
             w_3 = n_3 * w_3
@@ -567,21 +699,23 @@
             j_30 = jh_30.conjugate()
             j_33 = jh_33.conjugate()
 
             jhwj_00 = jh_00*w_0*j_00 + jh_03*w_3*j_03
             jhwj_03 = jh_00*w_0*j_30 + jh_03*w_3*j_33
             jhwj_33 = jh_30*w_0*j_30 + jh_33*w_3*j_33
 
-            jhj[0, 0] += jhwj_00.real
-            jhj[0, 1] += (gc_0*jhwj_03*g_3).real
+            coeffsq = coeff ** 2
+
+            jhj[0, 0] += coeffsq * jhwj_00.real
+            jhj[0, 1] += coeffsq * (gc_0*jhwj_03*g_3).real
             jhj[1, 0] = jhj[0, 1]
-            jhj[1, 1] += jhwj_33.real
+            jhj[1, 1] += coeffsq * jhwj_33.real
 
     elif corr_mode.literal_value == 2:
-        def impl(lop, rop, w, normf, gain, res, jhr, jhj):
+        def impl(lop, rop, w, normf, coeff, gain, res, jhr, jhj):
 
             # Compute normalization factor.
             iunpack(normf, rop)
             iabsdivsq(normf)
             imul(res, normf)  # Apply normalization factor to r.
 
             # Accumulate an element of jhwr.
@@ -592,29 +726,30 @@
 
             drv_00 = -1j*gc_0
             drv_23 = -1j*gc_1
 
             upd_00 = (drv_00*r_0).real
             upd_11 = (drv_23*r_1).real
 
-            jhr[0] += upd_00
-            jhr[1] += upd_11
+            jhr[0] += coeff*upd_00
+            jhr[1] += coeff*upd_11
 
             # Accumulate an element of jhwj.
             jh_00, jh_11 = unpack(rop)
             j_00, j_11 = unpackc(rop)
             w_00, w_11 = unpack(w)
             n_00, n_11 = unpack(normf)
 
-            # TODO: Consider representing as a vector?
-            jhj[0, 0] += (jh_00*n_00*w_00*j_00).real
-            jhj[1, 1] += (jh_11*n_11*w_11*j_11).real
+            coeffsq = coeff ** 2
+
+            jhj[0, 0] += coeffsq * (jh_00*n_00*w_00*j_00).real
+            jhj[1, 1] += coeffsq * (jh_11*n_11*w_11*j_11).real
 
     elif corr_mode.literal_value == 1:
-        def impl(lop, rop, w, normf, gain, res, jhr, jhj):
+        def impl(lop, rop, w, normf, coeff, gain, res, jhr, jhj):
 
             # Compute normalization factor.
             iunpack(normf, rop)
             iabsdivsq(normf)
             imul(res, normf)  # Apply normalization factor to r.
 
             # Accumulate an element of jhwr.
@@ -623,20 +758,99 @@
             r_0 = unpack(res)
             gc_0 = unpackc(gain)
 
             drv_00 = -1j*gc_0
 
             upd_00 = (drv_00*r_0).real
 
-            jhr[0] += upd_00
+            jhr[0] += coeff*upd_00
 
             # Accumulate an element of jhwj.
             jh_00 = unpack(rop)
             j_00 = unpackc(rop)
             w_00 = unpack(w)
             n_00 = unpack(normf)
 
-            jhj[0, 0] += (jh_00*n_00*w_00*j_00).real
+            jhj[0, 0] += coeff ** 2 * (jh_00*n_00*w_00*j_00).real
     else:
         raise ValueError("Unsupported number of correlations.")
 
     return factories.qcjit(impl)
+
+
+@njit(**JIT_OPTIONS)
+def delay_params_to_gains(
+    params,
+    gains,
+    chan_freq,
+    param_freq_map,
+    rescaled=False
+):
+
+    n_time, n_freq, n_ant, n_dir, n_corr = gains.shape
+
+    cf_min = chan_freq.min()
+    cf_max = chan_freq.max()
+    cf_mid = (cf_min + cf_max) / 2
+
+    if rescaled:
+        offset = 1.0
+        denom = cf_mid
+    else:
+        offset = cf_mid
+        denom = 1.0
+
+    for t in range(n_time):
+        for f in range(n_freq):
+            f_m = param_freq_map[f]
+            coeff = 2 * np.pi * (chan_freq[f] / denom - offset)
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    g = gains[t, f, a, d]
+                    p = params[t, f_m, a, d]
+
+                    g[0] = np.exp(1j * coeff * p[0])
+
+                    if n_corr > 1:
+                        g[-1] = np.exp(1j * coeff * p[1])
+
+
+@njit(**JIT_OPTIONS)
+def reference_params(ms_inputs, mapping_inputs, chain_inputs, meta_inputs):
+
+    chan_freq = ms_inputs.CHAN_FREQ
+
+    active_term = meta_inputs.active_term
+    ref_ant = meta_inputs.reference_antenna
+
+    gains = chain_inputs.gains[active_term]
+    gain_flags = chain_inputs.gain_flags[active_term]
+    params = chain_inputs.params[active_term]
+    param_flags = chain_inputs.param_flags[active_term]
+
+    param_freq_map = mapping_inputs.param_freq_maps[active_term]
+
+    n_ti, n_fi, n_ant, n_dir, n_corr = params.shape
+
+    ref_params = params[:, :, ref_ant: ref_ant + 1, :, :].copy()
+
+    for t in range(n_ti):
+        for f in range(n_fi):
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    p = params[t, f, a, d]
+                    rp = ref_params[t, f, 0, d]
+
+                    if param_flags[t, f, a, d] == 1:
+                        continue
+                    else:
+                        p -= rp
+
+    delay_params_to_gains(
+        params, gains, chan_freq, param_freq_map, rescaled=True
+    )
+
+    # Referencing may move flagged gains/params from identity.
+    apply_param_flags_to_params(param_flags, params, 0)
+    apply_gain_flags_to_gains(gain_flags, gains)
```

### Comparing `quartical-0.1.9/quartical/gains/rotation_measure/kernel.py` & `quartical-0.2.0/quartical/gains/rotation_measure/kernel.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,113 @@
 # -*- coding: utf-8 -*-
 import numpy as np
-from numba import prange, generated_jit
-from quartical.utils.numba import coerce_literal
+from numba import prange, njit
+from numba.extending import overload
+from quartical.utils.numba import (coerce_literal,
+                                   JIT_OPTIONS,
+                                   PARALLEL_JIT_OPTIONS)
 from quartical.gains.general.generics import (native_intermediaries,
                                               upsampled_itermediaries,
                                               per_array_jhj_jhr,
                                               resample_solints,
                                               downsample_jhj_jhr)
 from quartical.gains.general.flagging import (flag_intermediaries,
                                               update_gain_flags,
                                               finalize_gain_flags,
-                                              apply_gain_flags,
+                                              apply_gain_flags_to_flag_col,
                                               update_param_flags)
 from quartical.gains.general.convenience import (get_row,
                                                  get_extents)
 import quartical.gains.general.factories as factories
 from quartical.gains.general.inversion import (invert_factory,
                                                inversion_buffer_factory)
-from collections import namedtuple
-
-
-# This can be done without a named tuple now. TODO: Add unpacking to
-# constructor.
-stat_fields = {"conv_iters": np.int64,
-               "conv_perc": np.float64}
-
-term_conv_info = namedtuple("term_conv_info", " ".join(stat_fields.keys()))
-
-rm_args = namedtuple(
-    "rm_args",
-    (
-        "params",
-        "chan_freqs",
-        "param_flags",
-        "t_bin_arr"
-    )
-)
 
 
 def get_identity_params(corr_mode):
 
     if corr_mode.literal_value == 4:
         return np.zeros((1,), dtype=np.float64)
     else:
         raise ValueError("Unsupported number of correlations.")
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=False,
-               cache=True,
-               nogil=True)
-def rm_solver(base_args, term_args, meta_args, corr_mode):
+@njit(**JIT_OPTIONS)
+def rm_solver(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    return rm_solver_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    )
+
+
+def rm_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+    raise NotImplementedError
 
-    coerce_literal(rm_solver, ["corr_mode"])
+
+@overload(rm_solver_impl, jit_options=JIT_OPTIONS)
+def nb_rm_solver_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    corr_mode
+):
+
+    coerce_literal(nb_rm_solver_impl, ["corr_mode"])
 
     identity_params = get_identity_params(corr_mode)
 
-    def impl(base_args, term_args, meta_args, corr_mode):
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
+        corr_mode
+    ):
 
-        gains = base_args.gains
-        gain_flags = base_args.gain_flags
+        gains = chain_inputs.gains
+        gain_flags = chain_inputs.gain_flags
 
-        active_term = meta_args.active_term
-        max_iter = meta_args.iters
-        solve_per = meta_args.solve_per
-        dd_term = meta_args.dd_term
-        n_thread = meta_args.threads
+        active_term = meta_inputs.active_term
+        max_iter = meta_inputs.iters
+        solve_per = meta_inputs.solve_per
+        dd_term = meta_inputs.dd_term
+        n_thread = meta_inputs.threads
 
         active_gain = gains[active_term]
         active_gain_flags = gain_flags[active_term]
-        active_params = term_args.params[active_term]
+        active_params = chain_inputs.params[active_term]
 
         # Set up some intemediaries used for flagging. TODO: Move?
         km1_gain = active_gain.copy()
         km1_abs2_diffs = np.zeros_like(active_gain_flags, dtype=np.float64)
         abs2_diffs_trend = np.zeros_like(active_gain_flags, dtype=np.float64)
         flag_imdry = \
             flag_intermediaries(km1_gain, km1_abs2_diffs, abs2_diffs_trend)
 
         # Set up some intemediaries used for solving.
         real_dtype = active_gain.real.dtype
         param_shape = active_params.shape
 
-        active_t_map_g = base_args.t_map_arr[0, :, active_term]
-        active_f_map_p = base_args.f_map_arr[1, :, active_term]
+        active_t_map_g = mapping_inputs.time_maps[active_term]
+        active_f_map_p = mapping_inputs.param_freq_maps[active_term]
 
         # Create more work to do in paralllel when needed, else no-op.
         resampler = resample_solints(active_t_map_g, param_shape, n_thread)
 
         # Determine the starts and stops of the rows and channels associated
         # with each solution interval.
         extents = get_extents(resampler.upsample_t_map, active_f_map_p)
@@ -100,144 +119,177 @@
         jhj = upsampled_jhj[:param_shape[0]]
         jhr = upsampled_jhr[:param_shape[0]]
         update = np.zeros(param_shape, dtype=real_dtype)
 
         upsampled_imdry = upsampled_itermediaries(upsampled_jhj, upsampled_jhr)
         native_imdry = native_intermediaries(jhj, jhr, update)
 
-        chan_freqs = term_args.chan_freqs
+        chan_freqs = ms_inputs.CHAN_FREQ
         lambda_sq = (299792458/chan_freqs)**2
 
-        for loop_idx in range(max_iter):
+        for loop_idx in range(max_iter or 1):
 
-            compute_jhj_jhr(base_args,
-                            term_args,
-                            meta_args,
-                            upsampled_imdry,
-                            extents,
-                            lambda_sq,
-                            corr_mode)
+            compute_jhj_jhr(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                upsampled_imdry,
+                extents,
+                lambda_sq,
+                corr_mode
+            )
 
             if resampler.active:
                 downsample_jhj_jhr(upsampled_imdry, resampler.downsample_t_map)
 
             if solve_per == "array":
                 per_array_jhj_jhr(native_imdry)
 
+            if not max_iter:  # Non-solvable term, we just want jhj.
+                conv_perc = 0  # Didn't converge.
+                loop_idx = -1  # Did zero iterations.
+                break
+
             compute_update(native_imdry,
                            corr_mode)
 
-            finalize_update(base_args,
-                            term_args,
-                            meta_args,
-                            native_imdry,
-                            lambda_sq,
-                            loop_idx,
-                            corr_mode)
+            finalize_update(
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                native_imdry,
+                loop_idx,
+                lambda_sq,
+                corr_mode
+            )
 
             # Check for gain convergence. Produced as a side effect of
             # flagging. The converged percentage is based on unflagged
             # intervals.
-            conv_perc = update_gain_flags(base_args,
-                                          term_args,
-                                          meta_args,
-                                          flag_imdry,
-                                          loop_idx,
-                                          corr_mode)
+            conv_perc = update_gain_flags(
+                chain_inputs,
+                meta_inputs,
+                flag_imdry,
+                loop_idx,
+                corr_mode,
+                numbness=1e9
+            )
 
             # Propagate gain flags to parameter flags.
-            update_param_flags(base_args,
-                               term_args,
-                               meta_args,
-                               identity_params)
+            update_param_flags(
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs,
+                identity_params
+            )
 
-            if conv_perc >= meta_args.stop_frac:
+            if conv_perc >= meta_inputs.stop_frac:
                 break
 
         # NOTE: Removes soft flags and flags points which have bad trends.
-        finalize_gain_flags(base_args,
-                            meta_args,
-                            flag_imdry,
-                            corr_mode)
+        finalize_gain_flags(
+            chain_inputs,
+            meta_inputs,
+            flag_imdry,
+            corr_mode
+        )
 
         # Call this one last time to ensure points flagged by finialize are
         # propagated (in the DI case).
         if not dd_term:
-            apply_gain_flags(base_args,
-                             meta_args)
+            apply_gain_flags_to_flag_col(
+                ms_inputs,
+                mapping_inputs,
+                chain_inputs,
+                meta_inputs
+            )
 
-        return native_imdry.jhj, term_conv_info(loop_idx + 1, conv_perc)
+        return native_imdry.jhj, loop_idx + 1, conv_perc
 
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_jhj_jhr(
-    base_args,
-    term_args,
-    meta_args,
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    upsampled_imdry,
+    extents,
+    lambda_sq,
+    corr_mode
+):
+    return NotImplementedError
+
+
+@overload(compute_jhj_jhr, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_jhj_jhr(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
     upsampled_imdry,
     extents,
     lambda_sq,
     corr_mode
 ):
 
     # We want to dispatch based on this field so we need its type.
-    row_weight_type = base_args[base_args.fields.index('row_weights')]
+    row_weights_idx = ms_inputs.fields.index('ROW_WEIGHTS')
+    row_weights_type = ms_inputs[row_weights_idx]
 
-    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weight_type)
+    imul_rweight = factories.imul_rweight_factory(corr_mode, row_weights_type)
     v1_imul_v2 = factories.v1_imul_v2_factory(corr_mode)
     v1_imul_v2ct = factories.v1_imul_v2ct_factory(corr_mode)
     v1ct_imul_v2 = factories.v1ct_imul_v2_factory(corr_mode)
     iunpack = factories.iunpack_factory(corr_mode)
     iunpackct = factories.iunpackct_factory(corr_mode)
     imul = factories.imul_factory(corr_mode)
     iadd = factories.iadd_factory(corr_mode)
     isub = factories.isub_factory(corr_mode)
     valloc = factories.valloc_factory(corr_mode)
     make_loop_vars = factories.loop_var_factory(corr_mode)
     set_identity = factories.set_identity_factory(corr_mode)
     compute_jhwj_jhwr_elem = compute_jhwj_jhwr_elem_factory(corr_mode)
 
     def impl(
-        base_args,
-        term_args,
-        meta_args,
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        meta_inputs,
         upsampled_imdry,
         extents,
         lambda_sq,
         corr_mode
     ):
 
-        active_term = meta_args.active_term
+        active_term = meta_inputs.active_term
 
-        data = base_args.data
-        model = base_args.model
-        weights = base_args.weights
-        flags = base_args.flags
-        antenna1 = base_args.a1
-        antenna2 = base_args.a2
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        gains = base_args.gains
-        params = term_args.params[active_term]
-        t_map_arr = base_args.t_map_arr[0]  # We only need the gain mappings.
-        f_map_arr_g = base_args.f_map_arr[0]
-        f_map_arr_p = base_args.f_map_arr[1]
-        d_map_arr = base_args.d_map_arr
+        data = ms_inputs.DATA
+        model = ms_inputs.MODEL_DATA
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        time_maps = mapping_inputs.time_maps
+        freq_maps = mapping_inputs.freq_maps
+        param_freq_maps = mapping_inputs.param_freq_maps
+        dir_maps = mapping_inputs.dir_maps
+
+        gains = chain_inputs.gains
+        params = chain_inputs.params[active_term]
 
         jhj = upsampled_imdry.jhj
         jhr = upsampled_imdry.jhr
 
-        _, n_chan, n_dir, n_corr = model.shape
+        n_row, n_chan, n_dir, n_corr = model.shape
 
         jhj[:] = 0
         jhr[:] = 0
 
         n_tint, n_fint, n_ant, n_gdir, n_param = jhr.shape
         n_int = n_tint*n_fint
 
@@ -291,15 +343,15 @@
             jhj_tifi = jhj[ti, fi]
 
             for row_ind in range(rs, re):
 
                 row = get_row(row_ind, row_map)
                 a1_m, a2_m = antenna1[row], antenna2[row]
 
-                rm_t = t_map_arr[row_ind, active_term]
+                rm_t = time_maps[active_term][row_ind]
 
                 for f in range(fs, fe):
 
                     if flags[row, f]:  # Skip flagged data points.
                         continue
 
                     # Apply row weights in the BDA case, otherwise a no-op.
@@ -308,27 +360,27 @@
 
                     lop_pq_arr[:] = 0
                     rop_pq_arr[:] = 0
                     lop_qp_arr[:] = 0
                     rop_qp_arr[:] = 0
                     v_pq[:] = 0
 
-                    rm_f = f_map_arr_p[f, active_term]
+                    rm_f = param_freq_maps[active_term][f]
 
                     for d in range(n_dir):
 
                         set_identity(lop_pq)
                         set_identity(lop_qp)
 
                         # Construct a small contiguous gain array. This makes
                         # the single term case fractionally slower.
                         for gi in range(n_gains):
-                            d_m = d_map_arr[gi, d]  # Broadcast dir.
-                            t_m = t_map_arr[row_ind, gi]
-                            f_m = f_map_arr_g[f, gi]
+                            d_m = dir_maps[gi][d]  # Broadcast dir.
+                            t_m = time_maps[gi][row_ind]
+                            f_m = freq_maps[gi][f]
 
                             gain = gains[gi][t_m, f_m]
 
                             iunpack(gains_p[gi], gain[a1_m, d_m])
                             iunpack(gains_q[gi], gain[a2_m, d_m])
 
                         m = model[row, f, d]
@@ -355,15 +407,15 @@
 
                             g_p = gains_p[g]
                             v1ct_imul_v2(g_p, lop_pq, lop_pq)
 
                             g_q = gains_q[g]
                             v1ct_imul_v2(g_q, lop_qp, lop_qp)
 
-                        out_d = d_map_arr[active_term, d]
+                        out_d = dir_maps[active_term][d]
 
                         iunpack(lop_pq_arr[out_d], lop_pq)
                         iadd(rop_pq_arr[out_d], rop_pq)
 
                         iunpack(lop_qp_arr[out_d], lop_qp)
                         iadd(rop_qp_arr[out_d], rop_qp)
 
@@ -411,20 +463,20 @@
                                                wr_qp,
                                                jhr_tifi[a2_m, d],
                                                jhj_tifi[a2_m, d])
         return
     return impl
 
 
-@generated_jit(nopython=True,
-               fastmath=True,
-               parallel=True,
-               cache=True,
-               nogil=True)
 def compute_update(native_imdry, corr_mode):
+    raise NotImplementedError
+
+
+@overload(compute_update, jit_options=PARALLEL_JIT_OPTIONS)
+def nb_compute_update(native_imdry, corr_mode):
 
     # We want to dispatch based on this field so we need its type.
     jhj = native_imdry[native_imdry.fields.index('jhj')]
 
     generalised = jhj.ndim == 6
     inversion_buffer = inversion_buffer_factory(generalised=generalised)
     invert = invert_factory(corr_mode, generalised=generalised)
@@ -455,49 +507,80 @@
                            jhr[t, f, a, d],
                            update[t, f, a, d],
                            buffers)
 
     return impl
 
 
-@generated_jit(nopython=True, fastmath=True, parallel=False, cache=True,
-               nogil=True)
-def finalize_update(base_args, term_args, meta_args, native_imdry, lambda_sq,
-                    loop_idx, corr_mode):
+def finalize_update(
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    lambda_sq,
+    corr_mode
+):
+    raise NotImplementedError
 
-    set_identity = factories.set_identity_factory(corr_mode)
 
-    if corr_mode.literal_value == 4:
-        def impl(base_args, term_args, meta_args, native_imdry, lambda_sq,
-                 loop_idx, corr_mode):
+@overload(finalize_update, jit_options=JIT_OPTIONS)
+def nb_finalize_update(
+    mapping_inputs,
+    chain_inputs,
+    meta_inputs,
+    native_imdry,
+    loop_idx,
+    lambda_sq,
+    corr_mode
+):
 
-            active_term = meta_args.active_term
+    set_identity = factories.set_identity_factory(corr_mode)
 
-            gain = base_args.gains[active_term]
-            gain_flags = base_args.gain_flags[active_term]
-            f_map_arr_p = base_args.f_map_arr[1, :, active_term]
-            d_map_arr = base_args.d_map_arr[active_term, :]
+    if corr_mode.literal_value == 4:
+        def impl(
+            mapping_inputs,
+            chain_inputs,
+            meta_inputs,
+            native_imdry,
+            loop_idx,
+            lambda_sq,
+            corr_mode
+        ):
+
+            dd_term = meta_inputs.dd_term
+            active_term = meta_inputs.active_term
+            pinned_directions = meta_inputs.pinned_directions
+
+            gain = chain_inputs.gains[active_term]
+            gain_flags = chain_inputs.gain_flags[active_term]
+            params = chain_inputs.params[active_term]
 
-            params = term_args.params[active_term]
+            param_freq_map = mapping_inputs.param_freq_maps[active_term]
+            dir_map = mapping_inputs.dir_maps[active_term]
 
             update = native_imdry.update
 
             update /= 2
             params += update
 
             n_time, n_freq, n_ant, n_dir, _ = gain.shape
 
+            if dd_term:
+                for pd in pinned_directions:
+                    params[..., pd, :] = 0
+
             for t in range(n_time):
                 for f in range(n_freq):
                     lsq = lambda_sq[f]
                     for a in range(n_ant):
                         for d in range(n_dir):
 
-                            f_m = f_map_arr_p[f]
-                            d_m = d_map_arr[d]
+                            f_m = param_freq_map[f]
+                            d_m = dir_map[d]
                             fl = gain_flags[t, f, a, d]
 
                             if fl == 1:
                                 set_identity(gain[t, f, a, d])
                             else:
                                 rm = params[t, f_m, a, d_m, 0]
 
@@ -582,7 +665,38 @@
             jhr[0] += (dh_3 * r_3).real
 
     else:
         raise ValueError("Rotation measure can only be solved for with four "
                          "correlation data.")
 
     return factories.qcjit(impl)
+
+
+@njit(**JIT_OPTIONS)
+def rm_params_to_gains(
+    params,
+    gains,
+    lambda_sq,
+    param_freq_map
+):
+
+    n_time, n_freq, n_ant, n_dir, n_corr = gains.shape
+
+    for t in range(n_time):
+        for f in range(n_freq):
+            lsq = lambda_sq[f]
+            f_m = param_freq_map[f]
+            for a in range(n_ant):
+                for d in range(n_dir):
+
+                    g = gains[t, f, a, d]
+                    rm = params[t, f_m, a, d, 0]
+
+                    beta = lsq*rm
+
+                    cos_beta = np.cos(beta)
+                    sin_beta = np.sin(beta)
+
+                    g[0] = cos_beta
+                    g[1] = -sin_beta
+                    g[2] = sin_beta
+                    g[3] = cos_beta
```

### Comparing `quartical-0.1.9/quartical/logging/__init__.py` & `quartical-0.2.0/quartical/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/scheduling/__init__.py` & `quartical-0.2.0/quartical/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/statistics/logging.py` & `quartical-0.2.0/quartical/statistics/logging.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,92 +1,74 @@
 import os
 import re
 import numpy as np
-import dask.array as da
 from loguru import logger
 from columnar import columnar
 
 
 # Some hex codes for reused colours.
 colours = {
     "green": "23D18B",
     "yellow": "F5F543",
     "orange": "FF8000",
     "red": "F14C4C",
     "grey": "A0A0A0"
 }
 
 
-def embed_stats_logging(stats_xds_list):
-    """Embeds the chisq logging into the dask graph."""
-
-    stats_log_xds_list = []
-
-    for sxds in stats_xds_list:
-
-        pre = sxds.PRESOLVE_CHISQ.data
-        post = sxds.POSTSOLVE_CHISQ.data
-
-        # This is dirty trick - we need to loop the logging into the graph.
-        # To do so, we resassign the post values (which are unchanged) to
-        # ensure that the logging code is called. TODO: Better way?
-        post = da.map_blocks(
-            log_chisq, pre, post, sxds.attrs, dtype=np.float32
-        )
-
-        stats_log_xds_list.append(
-            sxds.assign(
-                {"POSTSOLVE_CHISQ": (("t_chunk", "f_chunk"), post)}
-            )
-        )
-
-    return stats_log_xds_list
-
-
-def log_chisq(pre, post, attrs, block_info=None):
+def log_chisq(pre, post, attrs, block_id=None):
     """Logs an info message per chunk containing chunk and chisq info.
 
     Args:
         pre: A numpy.ndarray contatining pre-solve chisq values.
         post: A numpy.ndarray contatining post-solve chisq values.
         attrs: xarray.Dataset attrs that contatain useful metadata.
         block_info: A dummy kwarg that tells dask to give us block info.
 
     Returns:
         post: An exact copy of the input - this is used to ensure the logging
             is embedded. TODO: Improve?
     """
 
     # Get the chink info (from the first arg), and pull out the location.
-    t_chunk, f_chunk = block_info[0]['chunk-location']
+    t_chunk, f_chunk, _ = block_id
 
     ddid = attrs.get("DATA_DESC_ID", "?")
     scan = attrs.get("SCAN_NUMBER", "?")
     field = attrs.get("FIELD_ID", "?")
 
     msg = "\n    "
 
     msg += f"FLD: {field} SPW: {ddid} SCN: {scan} "
     msg += f"T_CHUNK: {t_chunk} "
     msg += f"F_CHUNK: {f_chunk} "
 
-    if pre.item() > post.item():
-        colour = colours['green']
-    elif pre.item() <= post.item():
-        colour = colours['red']
+    pre = pre.item()
+    post = post.item()
+
+    if np.isfinite(pre) and np.isfinite(post):
+        fractional_change = (post - pre) / pre
+    else:
+        fractional_change = np.nan
+
+    if np.isfinite(fractional_change):
+        if np.abs(fractional_change) < 1e-12:  # Slightly numb to jitter.
+            colour = colours['yellow']
+        elif fractional_change < 0:
+            colour = colours['green']
+        elif fractional_change > 0:
+            colour = colours['red']
     else:
         colour = colours['grey']
 
     co, cc = f"<fg #{colour}>", f"</fg #{colour}>"
-    msg += f"{co}CHISQ: {pre.item():.2f} -> {post.item():.2f}{cc}"
+    msg += f"{co}CHISQ: {pre:.2f} -> {post:.2f}{cc}"
 
     logger.opt(colors=True).info(msg)
 
-    return post.copy()
-
 
 def log_summary_stats(stats_xds_list):
 
     tables = []
 
     n_sxds = len(stats_xds_list)
     group_size = 6
@@ -118,14 +100,15 @@
             t_coords, f_coords = np.meshgrid(t_coords, f_coords)
             t_coords, f_coords = t_coords.ravel(), f_coords.ravel()
 
             frame[t_coords, f_coords] = chisq[t_coords, f_coords]
 
             attrs = [sxds.attrs.get(f, "?") for f in attr_fields]
 
+            # TODO: Chi-squared values of zero disappear here.
             data.append([f"{v:.2f}" if v else "" for v in frame.ravel()])
             headers.append(fmt.format(*attrs))
 
         data = [list(x) for x in zip(ids, *data)]
 
         try:
             columns, _ = os.get_terminal_size()
```

### Comparing `quartical-0.1.9/quartical/utils/dask.py` & `quartical-0.2.0/quartical/utils/dask.py`

 * *Files identical despite different names*

### Comparing `quartical-0.1.9/quartical/utils/intervals.py` & `quartical-0.2.0/quartical/utils/intervals.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import numpy as np
-from numba import jit, types
+from numba import njit, types
 from numba.extending import overload
+from quartical.utils.numba import JIT_OPTIONS
 
 
 model_schema = ("rowlike", "chan", "ant", "dir", "corr")
 data_schema = ("rowlike", "chan", "ant", "corr")
 gain_schema = ("rowlike", "chan", "ant", "dir", "corr")
 
 
-# @jit(nopython=True, fastmath=False, parallel=False, cache=True, nogil=True)
+# NOTE: None of this code is in use any more and can likely be deleted.
+
+# @njit(**JIT_OPTIONS)
 # def column_to_tifiac(in_col, t_map, f_map, ant1_col, ant2_col, n_ti, n_fi,
 #                      n_a):
 #     """Go from a column-like input to a (ti, fi, a, c) output."""
 
 #     n_row = in_col.shape[0]
 #     n_chan = in_col.shape[1]
 #     n_corr = in_col.shape[-1]
@@ -61,15 +64,15 @@
 # def tifiac_inner_loop_cmplx(out_arr, in_col, t_m, f_m, row, chan, a1_m,
 #                             a2_m):
 
 #     out_arr[t_m, f_m, a1_m, :] += in_col[row, chan, :]
 #     out_arr[t_m, f_m, a2_m, :] += in_col[row, chan, :].conjugate()
 
 
-@jit(nopython=True, fastmath=False, parallel=False, cache=True, nogil=True)
+@njit(**JIT_OPTIONS)
 def rfc_to_tfac(in_col, ant1_col, ant2_col, utime_ind, n_ut, n_a):
     """Accumulate a (r, f, c) column into (t, f, a, c) array."""
 
     n_row, n_chan, n_corr = in_col.shape
 
     out_dtype = get_output_dtype(in_col)
 
@@ -126,15 +129,15 @@
 
     if isinstance(in_col.dtype, types.Boolean):
         return lambda in_col: np.int32
     else:
         return lambda in_col: in_col.dtype
 
 
-# @jit(nopython=True, fastmath=False, parallel=False, cache=True, nogil=True)
+# @njit(**JIT_OPTIONS)
 # def rfdc_to_tfadc(in_col, ant1_col, ant2_col, utime_ind, n_ut, n_a):
 #     """Accumulate a (r, f, d, c) column into (t, f, a, d, c) array."""
 
 #     n_row, n_chan, n_dir, n_corr = in_col.shape
 
 #     out_arr = np.zeros((n_ut.item(), n_chan, n_a, n_dir, n_corr),
 #                        dtype=in_col.dtype)
@@ -155,15 +158,15 @@
 #                         in_col[row, chan, d, c]
 #                     out_arr[t_m, chan, a2_m, d, c] += \
 #                         in_col[row, chan, d, c].conjugate()
 
 #     return out_arr
 
 
-@jit(nopython=True, fastmath=False, parallel=False, cache=True, nogil=True)
+@njit(**JIT_OPTIONS)
 def rfdc_to_abs_tfadc(in_col, ant1_col, ant2_col, utime_ind, n_ut, n_a):
     """Accumulate (r, f, d, c) column into abs**2 (t, f, a, d, c) array."""
 
     n_row, n_chan, n_dir, n_corr = in_col.shape
 
     out_arr = np.zeros((n_ut.item(), n_chan, n_a, n_dir, n_corr),
                        dtype=in_col.real.dtype)
@@ -186,15 +189,15 @@
 
                     out_arr[t_m, chan, a1_m, d, c] += abs_val
                     out_arr[t_m, chan, a2_m, d, c] += abs_val
 
     return out_arr
 
 
-@jit(nopython=True, fastmath=False, parallel=False, cache=True, nogil=True)
+@njit(**JIT_OPTIONS)
 def tfx_to_tifix(in_arr, t_map, f_map):
     """Sum a (t, f, ...) array into a (ti, fi, ...) array."""
 
     in_arr_shape = in_arr.shape
 
     n_time = in_arr_shape[0]
     n_chan = in_arr_shape[1]
```

### Comparing `quartical-0.1.9/quartical/utils/maths.py` & `quartical-0.2.0/quartical/utils/maths.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numba as nb
 import numpy as np
-from numba import jit
-import math
+from numba import njit
+from quartical.utils.numba import JIT_OPTIONS
 
 
 @nb.vectorize([nb.float64(nb.complex128), nb.float32(nb.complex64)])
 def cabs2(x):
     """Fast abs^2 for complex numbers which returns a contiguous array."""
     return x.real**2 + x.imag**2
 
@@ -40,15 +40,15 @@
 
     if not np.all((arr/net_gcd - np.round(arr/net_gcd)) < 1e-3):
         raise ValueError(f"No GCD was found for {arr}.")
 
     return net_gcd
 
 
-@jit(nopython=True, fastmath=True, parallel=False, cache=True, nogil=True)
+@njit(**JIT_OPTIONS)
 def mean_for_index(arr, inds):
 
     sums = np.zeros(np.max(inds) + 1, dtype=arr.dtype)
     counts = np.zeros_like(sums)
 
     for i in range(arr.size):
         ind = inds[i]
```

### Comparing `quartical-0.1.9/quartical/weights/robust.py` & `quartical-0.2.0/quartical/weights/robust.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import numpy as np
-from numba import generated_jit, jit
+from numba import njit
+from numba.extending import overload
+from quartical.utils.numba import coerce_literal, JIT_OPTIONS
 import quartical.gains.general.factories as factories
 from quartical.gains.general.generics import compute_residual
 
 
-qcgjit = generated_jit(nopython=True,
-                       fastmath=True,
-                       cache=True,
-                       nogil=True)
-
-qcjit = jit(nopython=True,
-            fastmath=True,
-            cache=True,
-            nogil=True)
+@njit(**JIT_OPTIONS)
+def update_icovariance(residuals, flags, etas, icovariance, mode):
+    return update_icovariance_impl(residuals, flags, etas, icovariance, mode)
 
 
-@qcgjit
-def update_icovariance(residuals, flags, etas, icovariance, mode):
+def update_icovariance_impl(residuals, flags, etas, icovariance, mode):
+    raise NotImplementedError
+
+
+@overload(update_icovariance_impl, jit_options=JIT_OPTIONS)
+def nb_update_icovariance_impl(residuals, flags, etas, icovariance, mode):
 
     update_covariance_inner = update_covariance_inner_factory(mode)
 
     def impl(residuals, flags, etas, icovariance, mode):
 
         n_row, n_chan, n_corr = residuals.shape
 
@@ -72,19 +72,28 @@
             r0 = unpack(res)
             r0c = unpackc(res)
 
             cov[0] += (r0 * eta * r0c).real
     else:
         raise ValueError("Unsupported number of correlations.")
 
-    return qcjit(impl)
+    return factories.qcjit(impl)
 
 
-@qcgjit
+@njit(**JIT_OPTIONS)
 def update_etas(residuals, flags, etas, icovariance, dof, mode):
+    return update_etas_impl(residuals, flags, etas, icovariance, dof, mode)
+
+
+def update_etas_impl(residuals, flags, etas, icovariance, dof, mode):
+    raise NotImplementedError
+
+
+@overload(update_etas_impl, jit_options=JIT_OPTIONS)
+def nb_update_etas_impl(residuals, flags, etas, icovariance, dof, mode):
 
     update_etas_inner = update_etas_inner_factory(mode)
 
     def impl(residuals, flags, etas, icovariance, dof, mode):
 
         n_row, n_chan, n_corr = residuals.shape
 
@@ -129,18 +138,18 @@
             r0c = unpackc(res)
             ic0 = unpack(icov)
 
             return (r0 * ic0 * r0c).real
     else:
         raise ValueError("Unsupported number of correlations.")
 
-    return qcjit(impl)
+    return factories.qcjit(impl)
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def digamma(x):
 
     result = 0
     while x <= 6:
         result -= 1/x  # Recurrence relation, gamma(x) = gamma(x+1) - 1/x
         x += 1
     result += np.log(x) - 1/(2*x)
@@ -150,20 +159,20 @@
     for c in coeffs:
         result += c*ix
         ix *= ix
 
     return result
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def dof_variable(dof):
     return np.log(dof) - digamma(dof)
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def dof_constant(etas, flags, dof, n_corr):
 
     n_row, n_chan = etas.shape
 
     n_unflagged = n_row * n_chan
 
     constant = 0
@@ -178,15 +187,15 @@
 
     if n_unflagged:
         constant /= n_unflagged
 
     return constant + 1 + digamma(dof + n_corr) - np.log(dof + n_corr)
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def compute_dof(etas, flags, dof, n_corr):
 
     constant = dof_constant(etas, flags, dof, n_corr)
 
     left = 1
     right = 30
 
@@ -202,15 +211,15 @@
             right = mid
         else:
             left = mid
 
     return mid
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def mean_weight(weights, flags):
 
     n_row, n_chan, n_corr = weights.shape
 
     mean = np.zeros(n_corr, dtype=weights.dtype)
 
     n_unflagged = n_row * n_chan
@@ -226,65 +235,120 @@
 
     if n_unflagged:
         mean /= n_unflagged
 
     return mean
 
 
-@qcjit
+@njit(**JIT_OPTIONS)
 def update_weights(weights, etas, icovariance):
 
     n_row, n_chan, n_corr = weights.shape
 
     for r in range(n_row):
         for f in range(n_chan):
             for c in range(n_corr):
 
                 weights[r, f, c] = etas[r, f] * icovariance[c]
 
 
-@qcgjit
-def robust_reweighting(base_args, meta_args, etas, icovariance, dof, mode):
-
-    def impl(base_args, meta_args, etas, icovariance, dof, mode):
-        model = base_args.model
-        data = base_args.data
-        a1 = base_args.a1
-        a2 = base_args.a2
-        weights = base_args.weights
-        flags = base_args.flags
-        t_map_arr = base_args.t_map_arr[0]  # Ignore parameter mappings.
-        f_map_arr = base_args.f_map_arr[0]  # Ignore parameter mappings.
-        d_map_arr = base_args.d_map_arr
-        gains = base_args.gains
-        row_map = base_args.row_map
-        row_weights = base_args.row_weights
-
-        residuals = compute_residual(data,
-                                     model,
-                                     gains,
-                                     a1,
-                                     a2,
-                                     t_map_arr,
-                                     f_map_arr,
-                                     d_map_arr,
-                                     row_map,
-                                     row_weights,
-                                     mode)
+@njit(**JIT_OPTIONS)
+def robust_reweighting(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    etas,
+    icovariance,
+    dof,
+    corr_mode
+):
+    return robust_reweighting_impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        etas,
+        icovariance,
+        dof,
+        corr_mode
+    )
+
+
+def robust_reweighting_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    etas,
+    icovariance,
+    dof,
+    corr_mode
+):
+    raise NotImplementedError
+
+
+@overload(robust_reweighting_impl, jit_options=JIT_OPTIONS)
+def nb_robust_reweighting_impl(
+    ms_inputs,
+    mapping_inputs,
+    chain_inputs,
+    etas,
+    icovariance,
+    dof,
+    corr_mode
+):
+
+    coerce_literal(nb_robust_reweighting_impl, ["corr_mode"])
+
+    def impl(
+        ms_inputs,
+        mapping_inputs,
+        chain_inputs,
+        etas,
+        icovariance,
+        dof,
+        corr_mode
+    ):
+        model = ms_inputs.MODEL_DATA
+        data = ms_inputs.DATA
+        antenna1 = ms_inputs.ANTENNA1
+        antenna2 = ms_inputs.ANTENNA2
+        weights = ms_inputs.WEIGHT
+        flags = ms_inputs.FLAG
+        row_map = ms_inputs.ROW_MAP
+        row_weights = ms_inputs.ROW_WEIGHTS
+
+        t_map_arr = mapping_inputs.time_maps
+        f_map_arr = mapping_inputs.freq_maps
+        d_map_arr = mapping_inputs.dir_maps
+
+        gains = chain_inputs.gains
+
+        residuals = compute_residual(
+            data,
+            model,
+            gains,
+            antenna1,
+            antenna2,
+            t_map_arr,
+            f_map_arr,
+            d_map_arr,
+            row_map,
+            row_weights,
+            corr_mode
+        )
 
         # First reweighting - we have already calibrated with MS weights.
         # This tries to approximate what that means in terms of initial values.
         if np.all(icovariance == 0):
             icovariance[:] = mean_weight(weights, flags)
-            update_etas(residuals, flags, etas, icovariance, dof, mode)
+            update_etas(residuals, flags, etas, icovariance, dof, corr_mode)
 
-        update_icovariance(residuals, flags, etas, icovariance, mode)
+        update_icovariance(residuals, flags, etas, icovariance, corr_mode)
 
-        dof = compute_dof(etas, flags, dof, mode)
+        dof = compute_dof(etas, flags, dof, corr_mode)
 
-        update_etas(residuals, flags, etas, icovariance, dof, mode)
+        update_etas(residuals, flags, etas, icovariance, dof, corr_mode)
 
         update_weights(weights, etas, icovariance)
 
         return dof
 
     return impl
```

### Comparing `quartical-0.1.9/quartical/weights/weights.py` & `quartical-0.2.0/quartical/weights/weights.py`

 * *Files identical despite different names*

