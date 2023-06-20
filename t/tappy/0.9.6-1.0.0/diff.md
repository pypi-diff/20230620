# Comparing `tmp/tappy-0.9.6.tar.gz` & `tmp/tappy-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tappy-0.9.6.tar", last modified: Thu Jul 14 02:21:17 2022, max compression
+gzip compressed data, was "tappy-1.0.0.tar", last modified: Tue Jun 20 15:23:45 2023, max compression
```

## Comparing `tappy-0.9.6.tar` & `tappy-1.0.0.tar`

### file list

```diff
@@ -1,135 +1,141 @@
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.878642 tappy-0.9.6/
--rw-rw-r--   0 tim       (1000) tim       (1000)      105 2022-06-27 02:03:47.000000 tappy-0.9.6/.deepsource.toml
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.862641 tappy-0.9.6/.github/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.866642 tappy-0.9.6/.github/workflows/
--rw-rw-r--   0 tim       (1000) tim       (1000)      472 2022-07-04 12:00:17.000000 tappy-0.9.6/.github/workflows/clean-workflow-runs.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     1713 2022-07-11 17:14:29.000000 tappy-0.9.6/.github/workflows/python-package.yml
--rw-rw-r--   0 tim       (1000) tim       (1000)     2402 2022-06-02 19:32:09.000000 tappy-0.9.6/.pre-commit-config.yaml
--rw-rw-r--   0 tim       (1000) tim       (1000)       50 2022-04-05 13:33:48.000000 tappy-0.9.6/AUTHORS.rst
--rw-r--r--   0 tim       (1000) tim       (1000)      745 2022-04-05 13:32:14.000000 tappy-0.9.6/BADGES.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      456 2022-07-14 02:19:20.000000 tappy-0.9.6/CHANGELOG.md
--rw-r--r--   0 tim       (1000) tim       (1000)     3123 2022-07-03 23:02:05.000000 tappy-0.9.6/CONTRIBUTING.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     1482 2022-07-03 23:02:18.000000 tappy-0.9.6/LICENSE.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      207 2022-07-14 02:17:58.000000 tappy-0.9.6/MANIFEST.in
--rw-rw-r--   0 tim       (1000) tim       (1000)     4966 2022-07-14 02:21:17.878642 tappy-0.9.6/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3622 2022-06-06 00:30:11.000000 tappy-0.9.6/README.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)        6 2022-07-14 02:19:20.000000 tappy-0.9.6/VERSION
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.866642 tappy-0.9.6/dist/
--rw-rw-r--   0 tim       (1000) tim       (1000)    33849 2022-04-17 02:20:35.000000 tappy-0.9.6/dist/tappy-0.9.3.tar.gz
--rw-rw-r--   0 tim       (1000) tim       (1000)    33839 2022-04-17 02:58:32.000000 tappy-0.9.6/dist/tappy-0.9.4.tar.gz
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.866642 tappy-0.9.6/docs/
--rw-rw-r--   0 tim       (1000) tim       (1000)     2538 2022-06-12 00:06:46.000000 tappy-0.9.6/docs/CompareTidalFilters.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)    14579 2022-04-05 12:03:23.000000 tappy-0.9.6/docs/Comparison_of_subtraction.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    13684 2022-04-05 12:04:00.000000 tappy-0.9.6/docs/Comparison_of_tidal_filters_large.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    12734 2022-04-05 12:04:28.000000 tappy-0.9.6/docs/Comparison_of_tidal_filters_small.png
--rw-rw-r--   0 tim       (1000) tim       (1000)      462 2022-06-02 19:34:03.000000 tappy-0.9.6/docs/FillMissing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     1074 2022-06-02 19:34:03.000000 tappy-0.9.6/docs/HarmonicAnalysis.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-04-05 13:36:55.000000 tappy-0.9.6/docs/Makefile
--rw-rw-r--   0 tim       (1000) tim       (1000)    11237 2022-04-05 12:05:55.000000 tappy-0.9.6/docs/Missing.png
--rw-rw-r--   0 tim       (1000) tim       (1000)    16497 2022-06-27 02:03:47.000000 tappy-0.9.6/docs/TappyUsersGuide.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)     3233 2022-06-12 00:06:46.000000 tappy-0.9.6/docs/TidalScience.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-04-05 15:46:46.000000 tappy-0.9.6/docs/authors.rst
--rw-r--r--   0 tim       (1000) tim       (1000)     9573 2022-06-09 03:45:34.000000 tappy-0.9.6/docs/conf.py
--rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-04-05 15:46:22.000000 tappy-0.9.6/docs/contributing.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)      527 2022-06-02 19:34:03.000000 tappy-0.9.6/docs/index.rst
--rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-04-05 15:46:53.000000 tappy-0.9.6/docs/license.rst
--rw-rw-r--   0 tim       (1000) tim       (1000)       27 2022-04-05 15:41:05.000000 tappy-0.9.6/docs/readme.rst
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/example/
--rwxrwxr-x   0 tim       (1000) tim       (1000)      850 2022-06-27 02:03:47.000000 tappy-0.9.6/example/example.sh
--rw-rw-r--   0 tim       (1000) tim       (1000)     2065 2022-04-01 22:29:05.000000 tappy-0.9.6/example/mayport_florida_8720220_con_noaa.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      954 2022-04-01 22:29:05.000000 tappy-0.9.6/example/mayport_florida_8720220_con_tappy.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    33481 2022-06-27 02:03:47.000000 tappy-0.9.6/example/mayport_florida_8720220_data.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      634 2022-06-27 02:03:47.000000 tappy-0.9.6/example/mayport_florida_8720220_data_def.txt
--rwxrwxr-x   0 tim       (1000) tim       (1000)      854 2022-06-12 00:06:51.000000 tappy-0.9.6/example/process_grace.py
--rw-rw-r--   0 tim       (1000) tim       (1000)      635 2022-06-27 02:03:47.000000 tappy-0.9.6/example/sparse.def
--rw-rw-r--   0 tim       (1000) tim       (1000)      662 2022-06-27 02:03:47.000000 tappy-0.9.6/example/tidesandcurrents.def
--rw-rw-r--   0 tim       (1000) tim       (1000)     2066 2022-04-01 22:29:05.000000 tappy-0.9.6/example/tridentpier_florida_8721604_con_noaa.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)      953 2022-04-01 22:29:05.000000 tappy-0.9.6/example/tridentpier_florida_8721604_con_tappy.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)    14490 2022-04-01 22:29:05.000000 tappy-0.9.6/example/tridentpier_florida_8721604_data.txt.gz
--rw-rw-r--   0 tim       (1000) tim       (1000)      955 2022-06-27 02:03:47.000000 tappy-0.9.6/example/tridentpier_florida_8721604_datetime.txt.def
--rw-r--r--   0 tim       (1000) tim       (1000)      650 2022-07-14 02:19:20.000000 tappy-0.9.6/pyproject.toml
--rw-r--r--   0 tim       (1000) tim       (1000)     1878 2022-07-14 02:21:17.878642 tappy-0.9.6/setup.cfg
--rw-rw-r--   0 tim       (1000) tim       (1000)      698 2022-07-14 01:14:46.000000 tappy-0.9.6/setup.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.862641 tappy-0.9.6/src/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/src/tappy/
--rw-rw-r--   0 tim       (1000) tim       (1000)        0 2022-07-14 02:12:37.000000 tappy-0.9.6/src/tappy/__init__.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    86394 2022-07-14 01:21:01.000000 tappy-0.9.6/src/tappy/tappy.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/src/tappy/tappy_lib/
--rw-rw-r--   0 tim       (1000) tim       (1000)      251 2022-07-04 11:57:10.000000 tappy-0.9.6/src/tappy/tappy_lib/__init__.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)     2643 2022-06-12 00:06:46.000000 tappy-0.9.6/src/tappy/tappy_lib/filter.py
--rw-rw-r--   0 tim       (1000) tim       (1000)    40408 2022-06-12 00:06:46.000000 tappy-0.9.6/src/tappy/tappy_lib/parameter_database.py
--rwxrwxr-x   0 tim       (1000) tim       (1000)    15295 2022-07-04 00:48:11.000000 tappy-0.9.6/src/tappy/tappy_lib/sparser.py
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/src/tappy.egg-info/
--rw-rw-r--   0 tim       (1000) tim       (1000)     4966 2022-07-14 02:21:16.000000 tappy-0.9.6/src/tappy.egg-info/PKG-INFO
--rw-rw-r--   0 tim       (1000) tim       (1000)     3563 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/SOURCES.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/dependency_links.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)       43 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/entry_points.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        1 2022-07-03 18:20:26.000000 tappy-0.9.6/src/tappy.egg-info/not-zip-safe
--rw-rw-r--   0 tim       (1000) tim       (1000)      226 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/requires.txt
--rw-rw-r--   0 tim       (1000) tim       (1000)        6 2022-07-14 02:21:17.000000 tappy-0.9.6/src/tappy.egg-info/top_level.txt
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.870642 tappy-0.9.6/tests/
-drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2022-07-14 02:21:17.878642 tappy-0.9.6/tests/output_ts/
--rw-rw-r--   0 tim       (1000) tim       (1000)     2413 2022-04-01 22:29:05.000000 tappy-0.9.6/tests/output_ts/constituents.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31114 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2MN6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31139 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2MS6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31089 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30606 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_2SM2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31149 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_2SM6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31560 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_J1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30221 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_K1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    29590 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_M2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30959 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_M3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30698 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_M4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31021 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_M6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31618 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_M8.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30841 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_MK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30806 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_MN4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31258 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_MO3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30884 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_MS4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30446 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_MSf.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30050 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_N2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30958 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_NO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30493 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_O1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31009 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_OO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30878 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30244 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_S2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31326 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_S4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31482 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_S6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31053 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_SK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    30580 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_eta2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2MN6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2MS6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:20.000000 tappy-0.9.6/tests/output_ts/outts_ff_2SM2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_2SM6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28899 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_J1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_K1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_M2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:21.000000 tappy-0.9.6/tests/output_ts/outts_ff_M3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_M4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_M6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_M8.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28886 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_MK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-0.9.6/tests/output_ts/outts_ff_MN4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28912 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_MO3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_MS4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_MSf.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_N2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:23.000000 tappy-0.9.6/tests/output_ts/outts_ff_NO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_O1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_OO1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_Q1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_S2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-0.9.6/tests/output_ts/outts_ff_S4.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_S6.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_SK3.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_eta2.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ff_ups1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    21576 2022-04-01 22:29:05.000000 tappy-0.9.6/tests/output_ts/outts_filtered_transform.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    19317 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_original.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    21918 2022-04-01 22:29:05.000000 tappy-0.9.6/tests/output_ts/outts_total_prediction.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    29591 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_total_tidal_components.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)    31026 2022-07-03 20:09:25.000000 tappy-0.9.6/tests/output_ts/outts_ups1.dat
--rw-rw-r--   0 tim       (1000) tim       (1000)      412 2022-06-27 02:03:47.000000 tappy-0.9.6/tests/predict_def.out
--rw-rw-r--   0 tim       (1000) tim       (1000)      588 2022-06-27 02:03:47.000000 tappy-0.9.6/tests/sparse.def
--rwxrwxr-x   0 tim       (1000) tim       (1000)     3416 2022-07-04 11:57:12.000000 tappy-0.9.6/tests/test_tappy.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.868431 tappy-1.0.0/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      102 2023-06-17 22:12:09.000000 tappy-1.0.0/.deepsource.toml
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.848431 tappy-1.0.0/.github/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.848431 tappy-1.0.0/.github/workflows/
+-rw-rw-r--   0 tim       (1000) tim       (1000)      501 2023-06-19 23:00:36.000000 tappy-1.0.0/.github/workflows/clean-workflow-runs.yml
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2121 2023-06-17 22:12:09.000000 tappy-1.0.0/.github/workflows/python-package.yml
+-rw-r--r--   0 tim       (1000) tim       (1000)      349 2023-03-05 18:49:58.000000 tappy-1.0.0/.gitignore
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2651 2023-06-19 23:00:36.000000 tappy-1.0.0/.pre-commit-config.yaml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       50 2022-04-05 13:33:48.000000 tappy-1.0.0/AUTHORS.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)      960 2022-09-28 02:52:38.000000 tappy-1.0.0/BADGES.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1019 2023-06-20 15:23:00.000000 tappy-1.0.0/CHANGELOG.md
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1191 2023-01-26 23:43:13.000000 tappy-1.0.0/CITATION.cff
+-rw-r--r--   0 tim       (1000) tim       (1000)     3123 2022-07-03 23:02:05.000000 tappy-1.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     1482 2022-07-03 23:02:18.000000 tappy-1.0.0/LICENSE.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10085 2023-06-20 15:23:45.868431 tappy-1.0.0/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     8641 2023-06-10 05:29:49.000000 tappy-1.0.0/README.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-06-20 15:23:00.000000 tappy-1.0.0/VERSION
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.852431 tappy-1.0.0/docs/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2538 2022-06-12 00:06:46.000000 tappy-1.0.0/docs/CompareTidalFilters.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14579 2022-04-05 12:03:23.000000 tappy-1.0.0/docs/Comparison_of_subtraction.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    13684 2022-04-05 12:04:00.000000 tappy-1.0.0/docs/Comparison_of_tidal_filters_large.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    12734 2022-04-05 12:04:28.000000 tappy-1.0.0/docs/Comparison_of_tidal_filters_small.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)      462 2022-06-02 19:34:03.000000 tappy-1.0.0/docs/FillMissing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     1074 2022-06-02 19:34:03.000000 tappy-1.0.0/docs/HarmonicAnalysis.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     5712 2022-04-05 13:36:55.000000 tappy-1.0.0/docs/Makefile
+-rw-rw-r--   0 tim       (1000) tim       (1000)    11237 2022-04-05 12:05:55.000000 tappy-1.0.0/docs/Missing.png
+-rw-rw-r--   0 tim       (1000) tim       (1000)    16493 2022-10-06 12:58:35.000000 tappy-1.0.0/docs/TappyUsersGuide.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3233 2022-06-12 00:06:46.000000 tappy-1.0.0/docs/TidalScience.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       55 2022-04-05 15:46:46.000000 tappy-1.0.0/docs/authors.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     5207 2023-06-19 22:50:20.000000 tappy-1.0.0/docs/citation.txt
+-rw-r--r--   0 tim       (1000) tim       (1000)      232 2023-05-13 04:20:03.000000 tappy-1.0.0/docs/command_line.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)     9549 2023-01-22 03:38:20.000000 tappy-1.0.0/docs/conf.py
+-rw-r--r--   0 tim       (1000) tim       (1000)       60 2022-04-05 15:46:22.000000 tappy-1.0.0/docs/contributing.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3385 2023-06-19 23:00:17.000000 tappy-1.0.0/docs/create_citations.sh
+-rw-r--r--   0 tim       (1000) tim       (1000)      191 2023-05-13 04:13:00.000000 tappy-1.0.0/docs/function_summary.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)      563 2022-11-06 21:06:34.000000 tappy-1.0.0/docs/index.rst
+-rw-r--r--   0 tim       (1000) tim       (1000)       79 2022-04-05 15:46:53.000000 tappy-1.0.0/docs/license.rst
+-rw-rw-r--   0 tim       (1000) tim       (1000)       27 2022-04-05 15:41:05.000000 tappy-1.0.0/docs/readme.rst
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.856431 tappy-1.0.0/example/
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      847 2022-10-06 12:58:35.000000 tappy-1.0.0/example/example.sh
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2065 2022-04-01 22:29:05.000000 tappy-1.0.0/example/mayport_florida_8720220_con_noaa.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      954 2022-04-01 22:29:05.000000 tappy-1.0.0/example/mayport_florida_8720220_con_tappy.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    33480 2022-10-06 12:58:35.000000 tappy-1.0.0/example/mayport_florida_8720220_data.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      632 2022-10-06 12:58:35.000000 tappy-1.0.0/example/mayport_florida_8720220_data_def.txt
+-rwxrwxr-x   0 tim       (1000) tim       (1000)      825 2023-01-22 03:38:20.000000 tappy-1.0.0/example/process_grace.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)      633 2022-10-06 12:58:35.000000 tappy-1.0.0/example/sparse.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)      660 2022-10-06 12:58:35.000000 tappy-1.0.0/example/tidesandcurrents.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2066 2022-04-01 22:29:05.000000 tappy-1.0.0/example/tridentpier_florida_8721604_con_noaa.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      953 2022-04-01 22:29:05.000000 tappy-1.0.0/example/tridentpier_florida_8721604_con_tappy.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)    14490 2022-04-01 22:29:05.000000 tappy-1.0.0/example/tridentpier_florida_8721604_data.txt.gz
+-rw-rw-r--   0 tim       (1000) tim       (1000)      949 2022-10-06 12:58:35.000000 tappy-1.0.0/example/tridentpier_florida_8721604_datetime.txt.def
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2618 2023-06-20 15:23:00.000000 tappy-1.0.0/pyproject.toml
+-rw-rw-r--   0 tim       (1000) tim       (1000)       38 2023-06-20 15:23:45.868431 tappy-1.0.0/setup.cfg
+-rw-rw-r--   0 tim       (1000) tim       (1000)      509 2023-03-01 21:51:24.000000 tappy-1.0.0/setup.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.848431 tappy-1.0.0/src/
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.856431 tappy-1.0.0/src/tappy/
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2023-01-22 03:38:20.000000 tappy-1.0.0/src/tappy/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    13822 2023-06-18 18:19:37.000000 tappy-1.0.0/src/tappy/analysis.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     3670 2023-06-19 01:07:24.000000 tappy-1.0.0/src/tappy/prediction.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     3935 2023-06-19 02:59:26.000000 tappy-1.0.0/src/tappy/tappy.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.856431 tappy-1.0.0/src/tappy/tappy_lib/
+-rw-rw-r--   0 tim       (1000) tim       (1000)        0 2023-06-19 21:42:08.000000 tappy-1.0.0/src/tappy/tappy_lib/__init__.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     2501 2023-06-19 04:26:22.000000 tappy-1.0.0/src/tappy/tappy_lib/filter.py
+-rw-rw-r--   0 tim       (1000) tim       (1000)    40384 2023-01-22 03:38:20.000000 tappy-1.0.0/src/tappy/tappy_lib/parameter_database.py
+-rwxrwxr-x   0 tim       (1000) tim       (1000)    15147 2023-06-19 22:50:21.000000 tappy-1.0.0/src/tappy/tappy_lib/sparser.py
+-rwxr-xr-x   0 tim       (1000) tim       (1000)    73991 2023-06-19 22:50:21.000000 tappy-1.0.0/src/tappy/utils.py
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.856431 tappy-1.0.0/src/tappy.egg-info/
+-rw-rw-r--   0 tim       (1000) tim       (1000)    10085 2023-06-20 15:23:45.000000 tappy-1.0.0/src/tappy.egg-info/PKG-INFO
+-rw-rw-r--   0 tim       (1000) tim       (1000)     3680 2023-06-20 15:23:45.000000 tappy-1.0.0/src/tappy.egg-info/SOURCES.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        1 2023-06-20 15:23:45.000000 tappy-1.0.0/src/tappy.egg-info/dependency_links.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)       43 2023-06-20 15:23:45.000000 tappy-1.0.0/src/tappy.egg-info/entry_points.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)      200 2023-06-20 15:23:45.000000 tappy-1.0.0/src/tappy.egg-info/requires.txt
+-rw-rw-r--   0 tim       (1000) tim       (1000)        6 2023-06-20 15:23:45.000000 tappy-1.0.0/src/tappy.egg-info/top_level.txt
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.860431 tappy-1.0.0/tests/
+-rw-rw-r--   0 tim       (1000) tim       (1000)   320926 2022-07-16 12:57:52.000000 tappy-1.0.0/tests/8720218.csv
+-rw-rw-r--   0 tim       (1000) tim       (1000)   232070 2022-07-16 13:06:15.000000 tappy-1.0.0/tests/8720218_wl.csv
+drwxrwxr-x   0 tim       (1000) tim       (1000)        0 2023-06-20 15:23:45.868431 tappy-1.0.0/tests/output_ts/
+-rw-rw-r--   0 tim       (1000) tim       (1000)     2413 2022-04-01 22:29:05.000000 tappy-1.0.0/tests/output_ts/constituents.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31114 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_2MN6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31139 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_2MS6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31089 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_2Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30606 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_2SM2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31149 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_2SM6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31560 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_J1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30221 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_K1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    29590 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_M2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30959 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_M3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30698 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_M4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31021 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_M6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31618 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_M8.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30841 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_MK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30806 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_MN4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31258 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_MO3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30884 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_MS4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30446 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_MSf.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30050 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_N2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30958 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_NO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30493 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_O1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31009 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_OO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30878 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30244 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_S2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31326 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_S4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31482 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_S6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31053 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_SK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    30580 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_eta2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_ff_2MN6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_ff_2MS6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_ff_2Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:20.000000 tappy-1.0.0/tests/output_ts/outts_ff_2SM2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_ff_2SM6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28899 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_ff_J1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_ff_K1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_ff_M2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:21.000000 tappy-1.0.0/tests/output_ts/outts_ff_M3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_ff_M4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28802 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_ff_M6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28799 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_ff_M8.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28886 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_ff_MK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:22.000000 tappy-1.0.0/tests/output_ts/outts_ff_MN4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28912 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_ff_MO3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28813 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_ff_MS4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_ff_MSf.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28812 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_ff_N2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:23.000000 tappy-1.0.0/tests/output_ts/outts_ff_NO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_ff_O1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_ff_OO1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28918 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_ff_Q1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_ff_S2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:24.000000 tappy-1.0.0/tests/output_ts/outts_ff_S4.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    17853 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_ff_S6.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28900 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_ff_SK3.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28911 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_ff_eta2.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    28904 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_ff_ups1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21576 2022-04-01 22:29:05.000000 tappy-1.0.0/tests/output_ts/outts_filtered_transform.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    19317 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_original.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    21918 2022-04-01 22:29:05.000000 tappy-1.0.0/tests/output_ts/outts_total_prediction.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    29591 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_total_tidal_components.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)    31026 2022-07-03 20:09:25.000000 tappy-1.0.0/tests/output_ts/outts_ups1.dat
+-rw-rw-r--   0 tim       (1000) tim       (1000)      410 2022-10-06 12:58:35.000000 tappy-1.0.0/tests/predict_def.out
+-rw-rw-r--   0 tim       (1000) tim       (1000)      586 2022-10-06 12:58:35.000000 tappy-1.0.0/tests/sparse.def
+-rwxrwxr-x   0 tim       (1000) tim       (1000)     3332 2023-06-19 22:50:21.000000 tappy-1.0.0/tests/test_tappy.py
```

### Comparing `tappy-0.9.6/.github/workflows/python-package.yml` & `tappy-1.0.0/.github/workflows/python-package.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,64 +1,69 @@
-# This workflow will install Python dependencies, run tests and lint with a variety of Python versions
-# For more information see: https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
+---
+# This workflow will install Python dependencies, run tests and lint with
+# a variety of Python versions For more information see:
+# https://help.github.com/actions/language-and-framework-guides/using-python-with-github-actions
 
 
-name: Python package
+name: Tests
 
 
-on:
-  push:
-    branches: [ main ]
-  pull_request:
-    branches: [ main ]
-  workflow_dispatch:
+on:  # yamllint disable-line rule:truthy
+    push:
+        branches: [main]
+    pull_request:
+        branches: [main]
+    workflow_dispatch:
 
 
 jobs:
-  test:
+    test:
 
-    runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: [ '3.7', '3.8', '3.9', '3.10' ]
-
-    steps:
-      - uses: actions/checkout@v3
-        with:
-          submodules: recursive
-
-      - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
-        with:
-          python-version: ${{ matrix.python-version }}
-
-      - name: Install dependencies
-        run: |
-          sudo apt-get update
-          sudo apt-get install gdal-bin libgdal-dev libgdal-doc proj-bin
-          python -m pip install --upgrade pip
-          python -m pip install flake8 pytest pytest-cov pytest-mpl
-          python -m pip install coverage[toml]
-          python -m pip install coveralls
-          python -m pip install -e .
-
-      - name: Test with pytest
-        run: |
-          python -m pytest --cov --mpl
-
-      - name: Coveralls
-        uses: AndreMiras/coveralls-python-action@develop
-        with:
-          github-token: ${{ secrets.GITHUB_TOKEN }}
-          flag-name: run-${{ matrix.test_number }}
-          parallel: true
-
-  finish:
-    needs: test
-    runs-on: ubuntu-latest
-    steps:
-      - name: Coveralls Finished
-        uses: AndreMiras/coveralls-python-action@develop
-        with:
-          github-token: ${{ secrets.GITHUB_TOKEN }}
-          parallel-finished: true
+        runs-on: ubuntu-latest
+        strategy:
+            fail-fast: false
+            matrix:
+                python-version: ['3.8', '3.9', '3.10', '3.11']
+
+        steps:
+            - uses: actions/checkout@v3
+              with:
+                  submodules: recursive
+
+            - name: Set up Python ${{ matrix.python-version }}
+              uses: actions/setup-python@v4
+              with:
+                  python-version: ${{ matrix.python-version }}
+
+            - name: Install dependencies
+              run: |
+                  sudo apt-get update
+                  sudo apt-get install gdal-bin libgdal-dev proj-bin
+                  python -m pip install --upgrade pip
+                  python -m pip install flake8 pytest pytest-cov pytest-mpl
+                  python -m pip install coverage[toml]
+                  python -m pip install coveralls
+                  python -m pip install -e .
+
+            - name: Test with pytest
+              run: |
+                  python -m pytest --cov --mpl
+
+            - name: Upload coverage data to coveralls.io
+              run: coveralls --service=github
+              env:
+                  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+                  COVERALLS_FLAG_NAME: ${{ matrix.test-name }}
+                  COVERALLS_PARALLEL: true
+
+    coveralls:
+        name: Indicate completion to coveralls.io
+        needs: test
+        runs-on: ubuntu-latest
+        container: python:3-slim
+        steps:
+            - name: Finished
+              run: |
+                  pip3 install --upgrade coveralls
+                  coveralls --service=github --finish
+              env:
+                  GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `tappy-0.9.6/BADGES.rst` & `tappy-1.0.0/BADGES.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,29 @@
 .. image:: https://github.com/timcera/tappy/actions/workflows/python-package.yml/badge.svg
+    :alt: Tests
     :target: https://github.com/timcera/tappy/actions/workflows/python-package.yml
     :height: 20
 
-.. image:: https://coveralls.io/repos/timcera/tappy/badge.png?branch=master
+.. image:: https://img.shields.io/coveralls/github/timcera/tappy
+    :alt: Test Coverage
     :target: https://coveralls.io/r/timcera/tappy?branch=master
     :height: 20
 
 .. image:: https://img.shields.io/pypi/v/tappy.svg
     :alt: Latest release
-    :target: https://pypi.python.org/pypi/tappy
+    :target: https://pypi.python.org/pypi/tappy/
+    :height: 20
 
-.. image:: http://img.shields.io/badge/license-BSD-lightgrey.svg
+.. image:: https://img.shields.io/pypi/l/tappy.svg
     :alt: BSD-3 clause license
     :target: https://pypi.python.org/pypi/tappy/
+    :height: 20
 
-.. image:: http://img.shields.io/pypi/dd/tappy.svg
+.. image:: https://img.shields.io/pypi/dd/tappy.svg
     :alt: tappy downloads
     :target: https://pypi.python.org/pypi/tappy/
+    :height: 20
+
+.. image:: https://img.shields.io/pypi/pyversions/tappy
+    :alt: PyPI - Python Version
+    :target: https://pypi.org/project/tappy/
+    :height: 20
```

### Comparing `tappy-0.9.6/CONTRIBUTING.rst` & `tappy-1.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/LICENSE.txt` & `tappy-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/CompareTidalFilters.rst` & `tappy-1.0.0/docs/CompareTidalFilters.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/Comparison_of_subtraction.png` & `tappy-1.0.0/docs/Comparison_of_subtraction.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/Comparison_of_tidal_filters_large.png` & `tappy-1.0.0/docs/Comparison_of_tidal_filters_large.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/Comparison_of_tidal_filters_small.png` & `tappy-1.0.0/docs/Comparison_of_tidal_filters_small.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/HarmonicAnalysis.rst` & `tappy-1.0.0/docs/HarmonicAnalysis.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/Makefile` & `tappy-1.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/Missing.png` & `tappy-1.0.0/docs/Missing.png`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/TappyUsersGuide.rst` & `tappy-1.0.0/docs/TappyUsersGuide.rst`

 * *Files 1% similar despite different names*

```diff
@@ -81,24 +81,24 @@
 
    <tr>
 
 .. raw:: html
 
    <td>
 
-You need to specify the separator between 
+You need to specify the separator between
 =========================================
 
-the integer part and the decimal 
+the integer part and the decimal
 ================================
 
-part of real numbers, even if you only 
+part of real numbers, even if you only
 ======================================
 
-have integers in your data file. 
+have integers in your data file.
 ================================
 
 decimal_sep = “.” # TAPPy needs the variables ‘year’, ‘month’, # ‘day’,
 ‘hour’, ‘minute’, ‘water_level’. # Any other variable name can be used
 as a # placeholder. parse = [ integer(‘state’, exact=3),
 integer_as_string(‘station’, exact=4), positive_integer(‘year’,
 exact=4), positive_integer(‘month’, exact=2), positive_integer(‘day’,
```

### Comparing `tappy-0.9.6/docs/TidalScience.rst` & `tappy-1.0.0/docs/TidalScience.rst`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/docs/conf.py` & `tappy-1.0.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # tappy documentation build configuration file, created by
 # sphinx-quickstart on Wed Nov  6 14:04:36 2013.
 #
 # This file is execfile()d with the current directory set to its containing dir.
 #
 # Note that not all possible configuration values are present in this
```

### Comparing `tappy-0.9.6/docs/index.rst` & `tappy-1.0.0/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 
    readme
    TappyUsersGuide
    FillMissing
    CompareTidalFilters
    HarmonicAnalysis
    TidalScience
+   command_line
+   function_summary
    contributing
    authors
    license
 
 Other Projects
 --------------
 http://timcera.bitbucket.io
```

### Comparing `tappy-0.9.6/example/example.sh` & `tappy-1.0.0/example/example.sh`

 * *Files 24% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 
 # Read from compressed file.  Use default 'sparse.def' parsing definition file.
 ../tappy.py tridentpier_florida_8721604_data.txt.gz
 
 # Output
 ../tappy.py --outputts mayport_florida_8720220_data.txt mayport_florida_8720220_data_def.txt
 
-# Test defining date as a single value.  Look at 
-# tridentpier_florida_8721604_datetime.txt.def for an explanation of what 
+# Test defining date as a single value.  Look at
+# tridentpier_florida_8721604_datetime.txt.def for an explanation of what
 # is going on.
-../tappy.py tridentpier_florida_8721604_datetime.txt.gz 
+../tappy.py tridentpier_florida_8721604_datetime.txt.gz
```

### Comparing `tappy-0.9.6/example/mayport_florida_8720220_con_noaa.txt` & `tappy-1.0.0/example/mayport_florida_8720220_con_noaa.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/example/mayport_florida_8720220_con_tappy.txt` & `tappy-1.0.0/example/mayport_florida_8720220_con_tappy.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/example/mayport_florida_8720220_data.txt` & `tappy-1.0.0/example/mayport_florida_8720220_data.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Station Date       Time      WL    Sigma I L 
+Station Date       Time      WL    Sigma I L
 8720220 01/01/2000 00:00   0.563   0.008 0 0
 8720220 01/01/2000 01:00   0.204   0.008 0 0
 8720220 01/01/2000 02:00  -0.050   0.005 0 0
 8720220 01/01/2000 03:00  -0.119   0.005 0 0
 8720220 01/01/2000 04:00   0.028   0.002 0 0
 8720220 01/01/2000 05:00   0.231   0.005 0 0
 8720220 01/01/2000 06:00   0.513   0.004 0 0
```

### Comparing `tappy-0.9.6/example/mayport_florida_8720220_data_def.txt` & `tappy-1.0.0/example/mayport_florida_8720220_data_def.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # You need to specify the separator between the integer part and the decimal
 # part of real numbers, even if you only have integers in your data file.
 decimal_sep = "."
 
 
 # TAPPy needs the variables 'year', 'month', 'day', 'hour', 'minute', 'water_level'.
 # Any other variable name can be used as a placeholder.
-parse = [ 
+parse = [
           integer('state', exact=3),
           integer_as_string('station', exact=4),
           positive_integer('day'),
           positive_integer('month'),
           positive_integer('year'),
           positive_integer('hour'),
           positive_integer('dummy'),
           real('water_level'),
          ]
-
```

### Comparing `tappy-0.9.6/example/process_grace.py` & `tappy-1.0.0/example/process_grace.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import datetime
 import string
 
 import scipy as N
 
 filename = "mayport_florida_8720220_data.txt"
 
-fp = open(filename, "r")
+fp = open(filename)
 fp.readline()
 elevation = []
 dates = []
 for line in fp:
     words = string.split(line)
     elevation.append(float(words[3]))
```

### Comparing `tappy-0.9.6/example/sparse.def` & `tappy-1.0.0/example/sparse.def`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # You need to specify the separator between the integer part and the decimal
 # part of real numbers, even if you only have integers in your data file.
 decimal_sep = "."
 
 
 # TAPPy needs the variables 'year', 'month', 'day', 'hour', 'minute', 'water_level'.
 # Any other variable name can be used as a placeholder.
-parse = [ 
+parse = [
           integer('state', exact=3),
           integer_as_string('station', exact=4),
           positive_integer('day'),
           positive_integer('month'),
           positive_integer('year'),
           positive_integer('hour'),
           positive_integer('minute'),
           real('water_level'),
          ]
-
```

### Comparing `tappy-0.9.6/example/tidesandcurrents.def` & `tappy-1.0.0/example/tidesandcurrents.def`

 * *Files 18% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # You need to specify the separator between the integer part and the decimal
 # part of real numbers, even if you only have integers in your data file.
 decimal_sep = "."
 
 
 # TAPPy needs the variables 'year', 'month', 'day', 'hour', 'minute', 'water_level'.
 # Any other variable name can be used as a placeholder.
-parse = [ 
+parse = [
           integer('state', exact=3),
           integer_as_string('station', exact=4),
           positive_integer('year', exact=4),
           positive_integer('month', exact=2),
           positive_integer('day', exact=2),
           positive_integer('hour'),
           positive_integer('minute'),
           real('water_level'),
          ]
-
```

### Comparing `tappy-0.9.6/example/tridentpier_florida_8721604_con_noaa.txt` & `tappy-1.0.0/example/tridentpier_florida_8721604_con_noaa.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/example/tridentpier_florida_8721604_con_tappy.txt` & `tappy-1.0.0/example/tridentpier_florida_8721604_con_tappy.txt`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/example/tridentpier_florida_8721604_data.txt.gz` & `tappy-1.0.0/example/tridentpier_florida_8721604_data.txt.gz`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/example/tridentpier_florida_8721604_datetime.txt.def` & `tappy-1.0.0/example/tridentpier_florida_8721604_datetime.txt.def`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 
 # You need to specify the separator between the integer part and the decimal
 # part of real numbers, even if you only have integers in your data file.
 decimal_sep = "."
 
 
-# TAPPy needs the variables 
-#   'datetime': a single integer or real listing time units after a origin 
-#    OR 
-#   'year', 'month', 'day', 'hour', optional['minute', 'second'] 
+# TAPPy needs the variables
+#   'datetime': a single integer or real listing time units after a origin
+#    OR
+#   'year', 'month', 'day', 'hour', optional['minute', 'second']
 #    AND
 #   'water_level').
 
 # Any other variable name can be used as a placeholder.
 
 # integer_as_datetime and real_as_datetime require an origin and unit
 
-parse = [ 
+parse = [
           integer_as_datetime('datetime', origin=datetime.datetime(1999,12,31,23), unit='hours'),
           integer('state', exact=3),
           integer_as_string('station', exact=4),
           positive_integer('toss_day'),
           positive_integer('toss_month'),
           positive_integer('toss_year'),
           positive_integer('toss_hour'),
           positive_integer('toss_minute'),
           real('water_level'),
          ]
-
```

### Comparing `tappy-0.9.6/src/tappy/tappy.py` & `tappy-1.0.0/src/tappy/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """
 NAME:
     tappy.py
 
 SYNOPSIS:
     tappy.py [options] filename
@@ -38,69 +37,76 @@
 #    along with this program; if not, write to the Free Software
 #    Foundation, Inc., 675 Mass Ave, Cambridge, MA 02139, USA.
 
 
 """
 import datetime
 import operator
-import os
-import os.path
-
-# ===imports======================
 import sys
+from pathlib import Path
 
 import astronomia.calendar as cal
-import mando
 import numpy as np
-import six
 from numpy import pad
 from scipy.optimize import leastsq
+from toolbox_utils import tsutils
 
 from tappy.tappy_lib import sparser
 from tappy.tappy_lib.parameter_database import _master_speed_dict, letter_to_factor_map
 
-# ===globals======================
 modname = "tappy"
 
-# --option args--
 debug_p = 0
-# opt_b=None  #string arg, default is undefined
 
-# ---other---
 deg2rad = np.pi / 180.0
 rad2deg = 180.0 / np.pi
 
 
 # ===utilities====================
 def msg(txt):
+    """Print a message to stdout."""
     sys.stdout.write(txt)
     sys.stdout.flush()
 
 
 def debug(ftn, txt):
+    """Print a debug message to stdout."""
     if debug_p:
         sys.stdout.write(f"{modname}.{ftn}:{txt}\n")
         sys.stdout.flush()
 
 
 def fatal(ftn, txt):
-    msg = f"{modname}.{ftn}:FATAL:{txt}\n"
-    raise SystemExit(msg)
+    """Print a fatal error message to stdout and exit."""
+    lmsg = f"{modname}.{ftn}:FATAL:{txt}\n"
+    raise SystemExit(lmsg)
 
 
 def usage():
+    """Print the usage message to stdout."""
     print(__doc__)
 
 
 def interpolate(data, start, stop, iavg):
-    """
-    Linearly interpolate across a section of a vector.  A function used by
-    zone_calculations.
-    """
+    """Linearly interpolate across a section of a vector.
+
+    A function used by zone_calculations.
 
+    Parameters
+    ----------
+    data : array
+        The data to be interpolated.
+    start : int
+        The starting index of the section to be interpolated.
+    stop : int
+        The ending index of the section to be interpolated.
+    iavg : int
+        The number of points to average on either side of the section to be
+        interpolated.
+    """
     ssl = slice(0, start) if start < iavg else slice(start - iavg, start)
     if stop > (len(data) - iavg):
         stop_sl = slice(stop + 1, len(data))
     else:
         stop_sl = slice(stop + 1, stop + iavg)
 
     deltay = np.average(data[stop_sl]) - np.average(data[ssl])
@@ -108,19 +114,29 @@
     m = deltay / numx
     b = np.average(data[ssl]) - m * (start - 1)
     for i in range(start, stop + 1):
         data[i] = m * i + b
 
 
 def zone_calculations(zftn, data, mask, limit=25):
-    """
-    Apply the supplied function across the patches (zones) of missing
-    values in the input vector data.  Used to fill missing or bad data.
-    """
+    """Apply a function across the patches (zones) of missing values.
 
+    Used to fill missing or bad data.
+
+    Parameters
+    ----------
+    zftn : function
+        The function to be applied to the data.
+    data : array
+        The data to be processed.
+    mask : array
+        A boolean array with True values where the data is missing or bad.
+    limit : int
+        The maximum number of points to be processed by the function.
+    """
     start = None
     stop = None
     for index, val in enumerate(mask):
         if val and not start:
             start = index
         if not val and start:
             stop = index - 1
@@ -189,14 +205,29 @@
 # ====================================
 class Util:
     def __init__(self, r, phase):
         self.r = r
         self.phase = phase
 
     def sum_signals(self, skey_list, hours, speed_dict, amp=None, phase=None):
+        """Sum the signals for a list of constituents.
+
+        Parameters
+        ----------
+        skey_list : list
+            A list of the constituents to be summed.
+        hours : array
+            A time-series of hours to be summed.
+        speed_dict : dict
+            A dictionary of the constituent speeds.
+        amp : array
+            The amplitudes of the constituents.
+        phase : array
+            The phases of the constituents.
+        """
         fpss = open("/tmp/ss.log", "w")
         fpss.write(f"{hours.shape}")
         total = np.zeros(len(hours), dtype="f")
         if isinstance(hours[0], datetime.datetime):
             hours = self.dates2jd(hours)
             hours = (hours - hours[0]) * 24
         for i in skey_list:
@@ -233,22 +264,32 @@
             ]
             jd = np.array(jd).flatten()
         else:
             jd = dates
         return jd
 
     def write_file(self, x, y, fname="-"):
+        """Write the data to a file.
+
+        Parameters
+        ----------
+        x : array
+            The time-series of dates.
+        y : array
+            The time-series of water levels.
+        """
         fp = open("/tmp/tap.log", "w")
         fp.write(f"{x}")
         fp.write(f"{y}")
         fp.write(f"{y.shape}")
         fp.write(fname)
         if isinstance(y, dict):
             for key in list(y.keys()):
-                nfname = f"{os.path.splitext(fname)[-2]}_{key}.dat"
+                fname = Path(fname)
+                nfname = fname.with_name(f"{fname.stem}_{key}.dat")
                 self.write_file(x, y[key], fname=nfname)
         elif fname == "-":
             print("Datetime,water_level")
             for d, v in zip(x, y):
                 print(f"{d.isoformat()},{v}")
         else:
             fpo = open(fname, "w")
@@ -328,15 +369,15 @@
         (zeta, nu, nup, nupp, kap_p, ii, R, Q, T, jd, s, h, Nv, p, p1) = package
         speed_dict = {}
 
         # Set data into speed_dict depending on length of time series
         # Required length of time series depends on Raleigh criteria to
         # differentiate beteen constituents of simmilar speed.
         #  Key is tidal constituent name from Schureman
-        #    speed is how fast the constiuent moves in radians/hour
+        #    speed is how fast the constituent moves in radians/hour
         #    VAU is V+u taken from Schureman
         #    FF is the node factor from Schureman
 
         # TASK has the following constituents
         #  MSN6       87.4238337
         self.tidal_dict = {}
 
@@ -521,17 +562,17 @@
             "ospeed": 14.4920521 * deg2rad,
             "VAU": T - s + h + zeta + nu,  # term A71 in Schureman
             "FF": node_factor_144(ii),
         }
         self.tidal_dict["NO1"] = {
             "ospeed": 14.496693984 * deg2rad,
             "VAU": T - s + h - 90 * deg2rad + zeta - nu + Q,
-            # 2.307**0.5 factor was missed in Darwin's analysis and the wrong
-            # factor was used for M1 for many years.  Indicates the importance
-            # of M1 and NO1.  As with many constituents listed here, I have
+            # 2.307**0.5 factor was missed in Darwin's  and the wrong
+            # factor was used for M1 for many years.  Indicates how unimportant
+            # M1 and NO1 are!  As with many constituents listed here, I have
             # included them for completeness rather than necessity.
             "FF": (
                 self.tidal_dict["O1"]["FF"]
                 * (2.31 + 1.435 * np.cos(2.0 * kap_p)) ** 0.5
                 / 2.307**0.5
             ),
         }
@@ -714,15 +755,15 @@
         self.tidal_dict["psi1"] = {
             "ospeed": 15.0821352 * deg2rad,
             "VAU": T + 2 * h - p1 - 90 * deg2rad,
             "FF": np.ones(length)
             #'psi1': [1, 'AAAZZYA', [1, 1, 1, 0, 0, -1, 1]],
         }
 
-        # Can calculate the speed at the begining of the time series.
+        # Can calculate the speed at the beginning of the time series.
         # Doesn't really matter unless analyzing tides in 5000 C.E.,  because the speeds do change.
         (
             zetatoss,
             nutoss,
             nuptoss,
             nupptoss,
             kap_ptoss,
@@ -792,15 +833,15 @@
                 self.tidal_dict[key]["VAU"] = np.mod(self.tidal_dict[key]["VAU"], 360)[
                     0
                 ]
             except IndexError:
                 self.tidal_dict[key]["VAU"] = np.mod(self.tidal_dict[key]["VAU"], 360)
 
         num_hours = (jd[-1] - jd[0]) * 24
-        numpoint = len(jd) * 0.5 * rayleigh_comp
+        len(jd) * 0.5 * rayleigh_comp
         if num_hours < 13:
             print("Cannot calculate any constituents from this record length")
             sys.exit()
         speed_dict["M2"] = self.tidal_dict["M2"]
         if num_hours >= (24 * rayleigh_comp):
             speed_dict["K1"] = self.tidal_dict["K1"]
         if num_hours >= 25 * rayleigh_comp:
@@ -931,28 +972,25 @@
             # GAM2 from Foreman should go here, but couldn't find comparable
             # constituent information from Schureman
             pass
         # This is what is required to separate NO1 and M1
         if num_hours >= 77554 * rayleigh_comp:
             speed_dict["M1"] = self.tidal_dict["M1"]
 
-        key_list = list(speed_dict.keys())
-        key_list.sort()
+        key_list = sorted(list(speed_dict.keys()))
 
         return (speed_dict, key_list)
 
 
-class tappy(Util):
+class Tappy(Util):
     def __init__(self, **kwds):
         """
         The initialization of the Tappy class.
         """
 
-        ftn = "tappy.__init__"
-
         self.quiet = kwds.pop("quiet")
         self.debug = kwds.pop("debug")
         self.outputts = kwds.pop("outputts")
         self.outputxml = kwds.pop("outputxml")
         self.ephemeris = kwds.pop("ephemeris")
         self.rayleigh = kwds.pop("rayleigh")
         self.print_vau_table = kwds.pop("print_vau_table")
@@ -966,56 +1004,71 @@
 
         # ---instance variables---
         self.speed_dict = {}
         self.elevation = []
         self.dates = []
 
     def open(self, filename, def_filename=None):
+        """Open the water level data file"""
+        # Test to make sure there isn't a definition file in the same directory
+        # as the data file.
+        filename = Path(filename)
+        if def_filename is None:
+            test_filename = filename.with_name(f"{filename.stem}_def{filename.suffix}")
+            if test_filename.exists():
+                def_filename = test_filename
         # Read and parse data filename
-        fp = sparser.ParseFileLineByLine(filename, def_filename=def_filename, mode="r")
-        for line in fp:
-            if "water_level" not in list(line.parsed_dict.keys()):
-                print(
-                    f"Warning: record {line.line_number} did not parse according to the supplied definition file"
-                )
-                continue
-            if "datetime" in list(line.parsed_dict.keys()):
-                self.dates.append(line.parsed_dict["datetime"])
-            elif (
-                "year" in list(line.parsed_dict.keys())
-                and "month" in list(line.parsed_dict.keys())
-                and "day" in list(line.parsed_dict.keys())
-                and "hour" in list(line.parsed_dict.keys())
-            ):
-                line.parsed_dict.setdefault("minute", 0)
-                line.parsed_dict.setdefault("second", 0)
-                self.dates.append(
-                    datetime.datetime(
-                        line.parsed_dict["year"],
-                        line.parsed_dict["month"],
-                        line.parsed_dict["day"],
-                        line.parsed_dict["hour"],
-                        line.parsed_dict["minute"],
-                        line.parsed_dict["second"],
+        if def_filename is None:
+            df = tsutils.common_kwds(filename)
+            self.elevation = df.iloc[:, 0].astype("float64").values
+            self.dates = df.index.to_pydatetime()
+        else:
+            fp = sparser.ParseFileLineByLine(
+                filename, def_filename=def_filename, mode="r"
+            )
+            for line in fp:
+                if "water_level" not in list(line.parsed_dict.keys()):
+                    print(
+                        f"Warning: record {line.line_number} did not parse according to the supplied definition file"
                     )
-                )
-            else:
-                print(
-                    f"Warning: record {line.line_number} did not parse the date and time according to the supplied definition file"
-                )
-                print(
-                    'Requires "year", "month", "day", and "hour" ("minute" and "second" are optional and default to zero) OR a Julian date/time'
-                )
-                continue
-            self.elevation.append(line.parsed_dict["water_level"])
-        if len(self.elevation) == 0:
-            print("No data was found in the input file.")
-            sys.exit()
-        self.elevation = np.array(self.elevation)
-        self.dates = np.array(self.dates)
+                    continue
+                if "datetime" in list(line.parsed_dict.keys()):
+                    self.dates.append(line.parsed_dict["datetime"])
+                elif (
+                    "year" in list(line.parsed_dict.keys())
+                    and "month" in list(line.parsed_dict.keys())
+                    and "day" in list(line.parsed_dict.keys())
+                    and "hour" in list(line.parsed_dict.keys())
+                ):
+                    line.parsed_dict.setdefault("minute", 0)
+                    line.parsed_dict.setdefault("second", 0)
+                    self.dates.append(
+                        datetime.datetime(
+                            line.parsed_dict["year"],
+                            line.parsed_dict["month"],
+                            line.parsed_dict["day"],
+                            line.parsed_dict["hour"],
+                            line.parsed_dict["minute"],
+                            line.parsed_dict["second"],
+                        )
+                    )
+                else:
+                    print(
+                        f"Warning: record {line.line_number} did not parse the date and time according to the supplied definition file"
+                    )
+                    print(
+                        'Requires "year", "month", "day", and "hour" ("minute" and "second" are optional and default to zero) OR a Julian date/time'
+                    )
+                    continue
+                self.elevation.append(line.parsed_dict["water_level"])
+            if len(self.elevation) == 0:
+                print("No data was found in the input file.")
+                sys.exit()
+            self.elevation = np.array(self.elevation)
+            self.dates = np.array(self.dates)
 
     def missing(self, task, dates, elev):
         """
         What to do with the missing values.
         """
 
         if task not in ["fail", "ignore", "fill"]:
@@ -1032,17 +1085,17 @@
         if np.any(interval > datetime.timedelta(seconds=3600)):
             if task == "fail":
                 print("There is a difference of greater than one hour between values")
                 sys.exit()
 
         if task == "fill":
             # Create real dates
-            start = dates[0]
+            dates[0]
             # Dominant interval
-            interval.sort()
+            interval = sorted(interval)
             interval = interval[len(interval) / 2]
 
             dt = dates[0]
             dates_filled = []
             while dt <= (dates[-1] + datetime.timedelta(minutes=1)):
                 dates_filled.append(dt)
                 dt = dt + interval
@@ -1116,15 +1169,14 @@
     def residuals(self, p, ht, t, key_list):
         """
         Used for least squares fit.
         """
 
         H = {}
         phase = {}
-        slope = {}
         for index, key in enumerate(key_list):
             H[key] = p[index]
             phase[key] = p[index + len(key_list)]
             # print('---')
             # print(key)
             # print(self.speed_dict[key]['FF'][:3])
         if len(self.speed_dict[key_list[0]]["FF"]) == len(t):
@@ -1261,17 +1313,16 @@
         if self.linear_trend:
             self.err = ht - (p[-2] * t + p[-1] + sumterm)
         else:
             self.err = ht - (p[-1] + sumterm)
 
         return self.err
 
-    # --------------------------
-
     def constituents(self):
+        """Determine the tidal constituents from the data."""
         difference = self.dates[1:] - self.dates[:-1]
         if np.any(difference < datetime.timedelta(seconds=0)):
             print("Let's do the time warp again!")
             print("The date values reverse - they must be constantly increasing.")
             sys.exit()
 
         p0 = [1.0] * (len(self.speed_dict) * 2 + 2)
@@ -1308,40 +1359,42 @@
                 )
 
         self.fitted_average = p0[-1]
         self.slope = p0[-2]
         # Should probably return something rather than change self.*
 
     def cat_dates(self, dates, len_dates):
+        """Pad the dates array with dates before and after the data."""
         interval = dates[1:] - dates[:-1]
-        interval.sort()
+        interval = sorted(interval)
         interval = interval[len(interval) / 2]
         cnt = np.arange(1, len_dates + 1) * datetime.timedelta(
             minutes=interval.seconds / 60
         )
         bdate = dates[0] - cnt[::-1]
         edate = dates[-1] + cnt
         return np.concatenate((bdate, dates, edate))
 
     def pad_f(self, nelevation, ndates, half_kern):
+        """Pad the filter arrays with values before and after the data."""
         blen = alen = half_kern
 
         nslice = slice(half_kern, -half_kern)
         cndates = self.cat_dates(ndates, half_kern)
 
         if self.pad_filters == "tide":
             tnelevation = np.concatenate(
                 (
                     np.array([np.average(nelevation[0:half_kern])]),
                     nelevation,
                     np.array([np.average(nelevation[-half_kern:])]),
                 )
             )
             interval = ndates[1:] - ndates[:-1]
-            interval.sort()
+            interval = sorted(interval)
             interval = interval[len(interval) / 2]
             deltat = datetime.timedelta(minutes=interval.seconds / 60)
             tndates = np.concatenate(
                 (
                     np.array([ndates[0] - blen * deltat]),
                     ndates,
                     np.array([ndates[-1] + alen * deltat]),
@@ -1361,37 +1414,38 @@
             nelevation = pad.reflect(nelevation, (blen, alen))
         if self.pad_filters == "wrap":
             nelevation = pad.wrap(nelevation, (blen, alen))
 
         return nelevation, cndates, nslice
 
     def delta_diff(self, elev, delta, start_index):
+        """Calculate the difference between the elevation and the elevation delta hours ago."""
         bindex = delta
         if start_index > delta:
             bindex = start_index
         tmpe = elev[bindex:]
         return tmpe - elev[bindex - delta : bindex - delta + len(tmpe)]
 
     def delta_sum(self, elev, delta):
+        """Calculate the sum of the elevation and the elevation delta hours ago."""
         return elev[delta:] + elev[:-delta]
 
     def filters(self, nstype, dates, elevation, pad_type=None):
+        """Apply filters to the data."""
         delta_dt = datetime.timedelta(hours=1)
 
         # For the time being the filters and padding can only work on hourly data.
 
         # Current implementation:
         # Determines the average hourly elevation.
-        interval = dates[1:] - dates[:-1]
-        interval.sort()
+        interval = sorted(dates[1:] - dates[:-1])
 
         dates_filled = dates
         nelevation = elevation
         if np.any(interval < delta_dt):
-
             # Probably the worst way you can get the average for the hour...
 
             dt = dates[0]
             dates_filled = []
             while dt <= (dates[-1] + datetime.timedelta(minutes=1)):
                 dates_filled.append(dt)
                 dt = dt + delta_dt
@@ -1432,21 +1486,20 @@
             import filter
 
             return dates_filled, filter.fft_lowpass(nelevation, 1 / 30.0, 1 / 40.0)
 
         if nstype == "kalman":
             # I threw this in from an example on scipy's web site.  I will keep
             # it here, but I can't see an immediate use for in in tidal
-            # analysis.  It dappens out all frequencies.
+            # analysis.  It dampens out all frequencies.
 
             # Might be able to use it it fill missing values.
 
             # intial parameters
             sz = (len(nelevation),)  # size of array
-            x = -0.37727  # truth value
 
             Q = (max(nelevation) - min(nelevation)) / 10000.0  # process variance
             Q = 1.0e-2
 
             # allocate space for arrays
             xhat = np.zeros(sz)  # a posteri estimate of x
             P = np.zeros(sz)  # a posteri error estimate
@@ -1520,15 +1573,15 @@
             # The Doodson X0 filter is a simple filter designed to damp out
             # the main tidal frequencies. It takes hourly values, 19 values
             # either side of the central one. A weighted average is taken
             # with the following weights
 
             # (1010010110201102112 0 2112011020110100101)/30.
 
-            # In "Data Analaysis and Methods in Oceanography":
+            # In "Data Analysis and Methods in Oceanography":
 
             # "The cosine-Lanczos filter, the transform filter, and the
             # Butterworth filter are often preferred to the Godin filter,
             # to earlier Doodson filter, because of their superior ability
             # to remove tidal period variability from oceanic signals."
 
             kern = [
@@ -1680,19 +1733,17 @@
                 lsfit = leastsq(self.residuals, p0, args=(nelev, ntimes, s_list))
                 slope.append(lsfit[0][-2])
 
             relevation = slope
             return dates_filled[nslice], relevation[nslice]
 
         if nstype == "wavelet":
-            import pylab
             import pywt
 
             for wl in pywt.wavelist():
-
                 w = pywt.Wavelet(wl)
 
                 max_level = pywt.dwt_max_level(len(elevation), w.dec_len)
                 a = pywt.wavedec(elevation, w, level=max_level, mode="sym")
 
                 for i in range(len(a))[1:]:
                     avg = np.average(a[i][:])
@@ -1741,17 +1792,18 @@
                 )
                 constituent_residual[key] = new_elev - everything_but
             relevation = everything_but
             return dates_filled[nslice], relevation[nslice]
 
     def sortbyvalue(self, mydict):
         """Return a list of (key, value) pairs, sorted by value."""
-        return sorted(six.iteritems(mydict), key=operator.itemgetter(1))
+        return sorted(mydict.items(), key=operator.itemgetter(1))
 
     def print_con(self):
+        """Print out the constituents."""
         ndict = {}
         for k in self.key_list:
             ndict[k] = self.speed_dict[k]["speed"]
 
         print("\n#%12s %12s %12s %12s" % ("NAME", "SPEED", "H", "PHASE"))
         print("#%12s %12s %12s %12s" % ("====", "=====", "=", "====="))
         klist = [i[0] for i in self.sortbyvalue(ndict)]
@@ -1779,14 +1831,15 @@
             )
 
         print("\n# AVERAGE (Z0) = ", self.fitted_average)
         if self.linear_trend:
             print("# SLOPE OF REMOVED LINEAR TREND = ", self.slope)
 
     def print_ephemeris_table(self):
+        """Print out the ephemeris table."""
         h_schureman = {
             1600: 279.857,
             1700: 280.624,
             1800: 280.407,
             1900: 280.190,
             2000: 279.973,
         }
@@ -1871,15 +1924,15 @@
             print(" R = ", R * rad2deg)
             print(" Ra = ", Ra * rad2deg)
             print(" log(Ra) = ", np.log10(Ra))
             print(" Q = ", Q * rad2deg)
             print(" log(Q) = ", np.log(Q))
             print(" T = ", T * rad2deg)
 
-        t = tappy(
+        t = Tappy(
             def_filename=None,
             quiet=False,
             debug=False,
             ephemeris=False,
             rayleigh=1.0,
             print_vau_table=False,
             outputts=False,
@@ -1897,15 +1950,15 @@
             + (datetime.datetime(i + 1, 1, 1, 0, 0) - datetime.datetime(i, 1, 1, 0, 0))
             / 2
             for i in range(1900, 2050)
         ]
         package = self.astronomic(t.dates)
         (zeta, nu, nup, nupp, kap_p, ii, R, Q, T, self.jd, s, h, Nv, p, p1) = package
         (speed_dict, key_list) = t.which_constituents(len(t.dates), package)
-        for k in [
+        for k in (
             "J1",
             "K1",
             "K2",
             "L2",
             "M1",
             "M2",
             "M3",
@@ -1913,27 +1966,28 @@
             "M8",
             "O1",
             "OO1",
             "MO3",
             "MO3",
             "Mf",
             "Mm",
-        ]:
-            for i in [1900, 1930]:
+        ):
+            for i in (1900, 1930):
                 print(i, k, speed_dict[k]["FF"][i - 1900])
                 if k == "M2":
                     print(
                         "M2>>",
                         -2.14 * np.sin(Nv[0] * deg2rad) * rad2deg,
                         speed_dict[k]["VAU"],
                     )
         self.print_v_u_table()
 
     def print_v_u_table(self):
-        t = tappy(
+        """Print a table of the v and u values for the constituents."""
+        t = Tappy(
             outputts=False,
             outputxml=False,
             def_filename=None,
             quiet=False,
             debug=False,
             ephemeris=False,
             rayleigh=1.0,
@@ -1950,441 +2004,10 @@
         for d in range(1851, 2001):
             t.dates.append(datetime.datetime(d, 1, 1, 0, 0))
 
         package = self.astronomic(t.dates)
         (zeta, nu, nup, nupp, kap_p, ii, R, Q, T, self.jd, s, h, Nv, p, p1) = package
         (speed_dict, key_list) = self.which_constituents(len(t.dates), package)
 
-        key_list.sort()
+        key_list = sorted(key_list)
         for key in key_list:
             print(key, speed_dict[key]["VAU"])
-
-    def print_node_factor_table(self):
-        pass
-
-
-@mando.command()
-def writeconfig(iniconffile=f"{sys.argv[0]}.ini"):
-    """OVERWRITES an ini style config file that holds all of default the command line options.
-
-    :param iniconffile: the file name of the ini file, defaults to 'script.ini'.
-    """
-
-    mando.writeconfig(iniconffile=iniconffile)
-
-
-@mando.command()
-def prediction(
-    xml_filename, start_date, end_date, interval, include_inferred=True, fname="-"
-):
-    """Prediction based upon earlier constituent analysis saved in IHOTC XML transfer format.
-
-    :param xml_filename: The tidal constituents in IHOTC XML transfer format.
-    :param start_date: The start date as a ISO 8601 string. '2010-01-01T00:00:00'
-    :param end_date: The end date as a ISO 8601 string. '2011-01-01T00:00:00:00'
-    :param interval: The interval as the number of minutes.
-    :param include_inferred: Include the inferred constituents.
-    :param fname: Output filename, default is '-' to print to screen.
-    """
-    import xml.etree.ElementTree as et
-
-    tree = et.parse(xml_filename)
-    root = tree.getroot()
-    rin = {}
-    phasein = {}
-    skey_list = []
-    for constituent in root.getiterator("Harmonic"):
-        inf = constituent.findtext("inferred")
-        if (not include_inferred) and (inf.lower() == "true"):
-            continue
-        nam = constituent.findtext("name")
-        amp = constituent.findtext("amplitude")
-        pha = constituent.findtext("phaseAngle")
-        rin[nam] = float(amp)
-        phasein[nam] = float(pha)
-        skey_list.append(nam)
-
-    u = Util(rin, phasein)
-    u.dates = [datetime.datetime.strptime(start_date, "%Y-%m-%dT%H:%M:%S")]
-    delta = datetime.timedelta(minutes=int(interval))
-    nextdate = u.dates[0] + delta
-    end_date = datetime.datetime.strptime(
-        end_date, "%Y-%m-%dT%H:%M:%S"
-    ) + datetime.timedelta(minutes=1)
-    while nextdate < end_date:
-        u.dates.append(nextdate)
-        nextdate = u.dates[-1] + delta
-
-    package = u.astronomic(u.dates)
-    (zeta, nu, nup, nupp, kap_p, ii, R, Q, T, u.jd, s, h, Nv, p, p1) = package
-
-    # Should change this - runs ONLY to get tidal_dict filled in...
-    (speed_dict, key_list) = u.which_constituents(len(u.dates), package)
-
-    prediction = 0.0
-    try:
-        prediction = rin["Z0"]
-    except KeyError:
-        pass
-
-    try:
-        skey_list.remove("Z0")
-    except ValueError:
-        pass
-
-    calcdates = (
-        np.array(list(range(len(u.dates))), dtype=np.float64) * float(interval) / 60.0
-    )
-    prediction = prediction + u.sum_signals(skey_list, calcdates, u.tidal_dict)
-
-    u.write_file(u.dates, prediction, fname=fname)
-
-
-# =============================
-@mando.command()
-def analysis(
-    data_filename,
-    def_filename=None,
-    config=None,
-    quiet=False,
-    debug=False,
-    outputts=False,
-    outputxml="",
-    ephemeris=False,
-    rayleigh=1.0,
-    print_vau_table=False,
-    missing_data="ignore",
-    linear_trend=False,
-    remove_extreme=False,
-    zero_ts=None,
-    filter=None,
-    pad_filters=None,
-    include_inferred=True,
-    xmlname="A port in a storm",
-    xmlcountry="A man without a country",
-    xmllatitude=0.0,
-    xmllongitude=0.0,
-    xmltimezone="0000",
-    xmlcomments="No comment",
-    xmlunits="m",
-    xmldecimalplaces="full",
-):
-    """Traditional analysis with separately calculated nodal factors.
-     Constituent amplitude units are the same as the input heights.
-     Constituent phases are based in the same time zone as the dates.
-
-    :param data_filename: The time-series of elevations to be analyzed.
-    :param def_filename: Containes the definition string to parse the input
-        data.
-    :param config: Read command line options from config file, override
-        config file entries on the command line.
-    :param quiet: Print nothing to the screen.
-    :param debug: Print debug messages.
-    :param outputts: Output time series for each constituent.
-    :param ephemeris: Print out ephemeris tables.
-    :param rayleigh: The Rayleigh coefficient is used to compare against to
-        determine time series length to differentiate between two
-        frequencies.  [default: default]
-    :param missing_data: What should be done if there is missing data.  One
-        of: fail, ignore, or fill. [default: default]
-    :param linear_trend: Include a linear trend in the least squares fit.
-    :param remove_extreme: Remove values outside of 2 standard deviations
-        before analysis.
-    :param zero_ts: Zero the input time series before constituent analysis
-        by subtracting filtered data. One of: transform,usgs,doodson,boxcar
-    :param filter:  Filter input data set with tide elimination filters. The
-        -o outputts option is implied. Any mix separated by commas and no
-        spaces: transform,usgs,doodson,boxcar
-    :param pad_filters: Pad input data set with values to return same size
-        after filtering.  Realize edge effects are unavoidable.  One of
-        ["tide", "minimum", "maximum", "mean", "median", "reflect", "wrap"]
-    :param include_inferred: Do not incorporate any inferred constituents
-        into the least squares fit.
-    :param print_vau_table: For debugging - will print a table of V and u
-        values to compare against Schureman.
-    :param outputxml: File name to output constituents as IHOTC XML format.
-    :param xmlname: Not used in analysis. Used ONLY to complete the XML
-        file. Name of the station supplying the observations. Defaults to 'A
-        port in a storm'.
-    :param xmlcountry: Not used in analysis. Used ONLY to complete the XML
-        file. Name of the country containing the station. Defaults to 'A man
-        without a country'.
-    :param xmllatitude: Not used in analysis. Used ONLY to complete the XML
-        file. Latitude of the station. Defaults to 0.0.
-    :param xmllongitude: Not used in analysis. Used ONLY to complete the XML
-        file. Longitude of the station. Defaults to 0.0.
-    :param xmltimezone: Not used in analysis. Used ONLY to complete the XML
-        file. Time zone of the station. Defaults to '0000'.
-    :param xmlcomments: Not used in analysis. Used ONLY to complete the XML
-        file. Station comments. Defaults to 'No comment'.
-    :param xmlunits: Not used in analysis. Used ONLY to complete the XML
-        file. Units of the observed water level. Defaults to 'm'.
-    :param xmldecimalplaces: Not used in analysis. Used ONLY to complete the
-        XML file. Format of the observed amplitude and phase. Default
-        depends on length of analysis record.  'full' is the default and
-        means that full accuracy, 'ihotc' is formatted according to IHOTC
-        standard which severly limits the number of decimal places, and if
-        an integer number lists the number of decimal places.
-    """
-
-    if config:
-        mando.readconfig(config)
-
-    x = tappy(
-        outputts=outputts,
-        outputxml=outputxml,
-        quiet=quiet,
-        debug=debug,
-        ephemeris=ephemeris,
-        rayleigh=rayleigh,
-        print_vau_table=print_vau_table,
-        missing_data=missing_data,
-        linear_trend=linear_trend,
-        remove_extreme=remove_extreme,
-        zero_ts=zero_ts,
-        filter=filter,
-        pad_filters=pad_filters,
-        include_inferred=include_inferred,
-    )
-
-    if ephemeris:
-        x.print_ephemeris_table()
-    if print_vau_table:
-        x.print_v_u_table()
-
-    x.open(data_filename, def_filename=def_filename)
-
-    if x.missing_data == "fail":
-        x.dates_filled, x.elevation_filled = x.missing(
-            x.missing_data, x.dates, x.elevation
-        )
-
-    if x.remove_extreme:
-        x.remove_extreme_values()
-
-    package = x.astronomic(x.dates)
-    (
-        x.zeta,
-        x.nu,
-        x.nup,
-        x.nupp,
-        x.kap_p,
-        x.ii,
-        x.R,
-        x.Q,
-        x.T,
-        x.jd,
-        x.s,
-        x.h,
-        x.N,
-        x.p,
-        x.p1,
-    ) = package
-
-    if rayleigh:
-        ray = float(rayleigh)
-    else:
-        ray = 1.0
-    (x.speed_dict, x.key_list) = x.which_constituents(
-        len(x.dates), package, rayleigh_comp=ray
-    )
-    if x.zero_ts:
-        # FIX - have to run the constituents package here in order to have
-        # filters available , and then run AGAIN later on.
-        x.constituents()
-        print(len(x.dates), len(x.elevation))
-        x.dates_filled, x.elevation_filled = x.missing("fill", x.dates, x.elevation)
-        print(len(x.dates_filled), len(x.elevation_filled))
-        x.dates, filtered = x.filters(zero_ts, x.dates_filled, x.elevation_filled)
-        print(len(x.dates), len(filtered))
-        x.elevation = x.elevation_filled - filtered
-        package = x.astronomic(x.dates)
-        (
-            x.zeta,
-            x.nu,
-            x.nup,
-            x.nupp,
-            x.kap_p,
-            x.ii,
-            x.R,
-            x.Q,
-            x.T,
-            x.jd,
-            x.s,
-            x.h,
-            x.N,
-            x.p,
-            x.p1,
-        ) = package
-        (x.speed_dict, x.key_list) = x.which_constituents(
-            len(x.dates), package, rayleigh_comp=ray
-        )
-
-    x.constituents()
-
-    if x.missing_data == "fill":
-        x.dates_filled, x.elevation_filled = x.missing(
-            x.missing_data, x.dates, x.elevation
-        )
-        x.write_file(x.dates_filled, x.elevation_filled, fname="outts_filled.dat")
-
-    if x.filter:
-        for item in x.filter.split(","):
-            if item in [
-                "mstha",
-                "wavelet",
-                "cd",
-                "boxcar",
-                "usgs",
-                "doodson",
-                "lecolazet1",
-                "kalman",
-                "transform",
-            ]:  # 'lecolazet', 'godin', 'sfa']:
-                filtered_dates, result = x.filters(item, x.dates, x.elevation)
-                x.write_file(filtered_dates, result, fname=f"outts_filtered_{item}.dat")
-        (x.speed_dict, x.key_list) = x.which_constituents(
-            len(x.dates), package, rayleigh_comp=ray
-        )
-
-    if not x.quiet:
-        x.print_con()
-
-    if x.outputts:
-        for key in x.key_list:
-            x.write_file(
-                x.dates,
-                x.sum_signals([key], x.dates, x.speed_dict),
-                fname=f"outts_{key}.dat",
-            )
-            x.write_file(x.dates, x.speed_dict[key]["FF"], fname=f"outts_ff_{key}.dat")
-        x.write_file(
-            x.dates,
-            x.sum_signals(x.key_list, x.dates, x.tidal_dict),
-            fname="outts_total_tidal_components.dat",
-        )
-        x.write_file(x.dates, x.elevation, fname="outts_original.dat")
-
-    if x.outputxml:
-        import xml.etree.ElementTree as et
-
-        def indent(elem, level=0):
-            i = f"\n{level * '  '}"
-            if len(elem):
-                if not elem.text or not elem.text.strip():
-                    elem.text = f"{i}  "
-                if not elem.tail or not elem.tail.strip():
-                    elem.tail = i
-                for elem in elem:
-                    indent(elem, level + 1)
-                if not elem.tail or not elem.tail.strip():
-                    elem.tail = i
-            else:
-                if level and (not elem.tail or not elem.tail.strip()):
-                    elem.tail = i
-
-        transfer = et.Element(
-            "Transfer",
-            attrib={
-                "ns0:noNamespaceSchemaLocation": "HC_Schema_V1.xsd",
-                "xmlns:ns0": "http://www.w3.org/2001/XMLSchema-instance",
-            },
-        )
-
-        port = et.SubElement(transfer, "Port")
-
-        name = et.SubElement(port, "name")
-        name.text = xmlname
-
-        country = et.SubElement(port, "country")
-        country.text = xmlcountry
-
-        position = et.SubElement(port, "position")
-
-        latitude = et.SubElement(position, "latitude")
-        latitude.text = str(xmllatitude)
-
-        longitude = et.SubElement(position, "longitude")
-        longitude.text = str(xmllongitude)
-
-        timezone = et.SubElement(port, "timeZone")
-        timezone.text = str(xmltimezone)
-
-        units = et.SubElement(port, "units")
-        units.text = str(xmlunits)
-
-        observationstart = et.SubElement(port, "observationStart")
-        observationstart.text = x.dates[0].isoformat()
-
-        comments = et.SubElement(port, "comments")
-        comments.text = xmlcomments
-
-        observationend = et.SubElement(port, "observationEnd")
-        observationend.text = x.dates[-1].isoformat()
-
-        ndict = {"Z0": 0.0}
-        for k in x.key_list + x.inferred_key_list:
-            ndict[k] = x.tidal_dict[k]["speed"]
-        klist = [i[0] for i in x.sortbyvalue(ndict)]
-
-        if xmldecimalplaces == "ihotc":
-            ampformatstr = "{0:.3f}"
-            phaformatstr = "{0:.1f}"
-            daterange = x.dates[-1] - x.dates[0]
-            if daterange < datetime.timedelta(days=90):
-                ampformatstr = "{0:.2f}"
-                phaformatstr = "{0:.0f}"
-        elif xmldecimalplaces == "full":
-            ampformatstr = "{0}"
-            phaformatstr = ampformatstr
-        else:
-            ampformatstr = f"{{0:.{xmldecimalplaces}f}}"
-            phaformatstr = ampformatstr
-
-        for key in klist:
-            if key in x.key_list:
-                if float(ampformatstr.format(x.r[key])) == 0.0:
-                    continue
-            elif key in x.inferred_key_list:
-                if float(ampformatstr.format(x.inferred_r[key])) == 0.0:
-                    continue
-
-            tmp = et.SubElement(port, "Harmonic")
-
-            hname = et.SubElement(tmp, "name")
-            hname.text = key
-
-            speed = et.SubElement(tmp, "speed")
-            inferred = et.SubElement(tmp, "inferred")
-            phaseangle = et.SubElement(tmp, "phaseAngle")
-            amplitude = et.SubElement(tmp, "amplitude")
-
-            if key in x.key_list:
-                inferred.text = "false"
-                amplitude.text = ampformatstr.format(x.r[key])
-                phaseangle.text = phaformatstr.format(x.phase[key])
-                speed.text = str(x.tidal_dict[key]["speed"] * rad2deg)
-            elif key in x.inferred_key_list:
-                inferred.text = "true"
-                amplitude.text = ampformatstr.format(x.inferred_r[key])
-                phaseangle.text = phaformatstr.format(x.inferred_phase[key])
-                speed.text = str(x.tidal_dict[key]["speed"] * rad2deg)
-            elif key == "Z0":
-                inferred.text = "false"
-                amplitude.text = ampformatstr.format(x.fitted_average)
-                phaseangle.text = phaformatstr.format(0.0)
-                speed.text = "0.0"
-
-        indent(transfer)
-        tree = et.ElementTree(transfer)
-        tree.write(x.outputxml)
-
-
-def main():
-    """Set debug and run mando.main function."""
-    if not os.path.exists("debug_tappy"):
-        sys.tracebacklimit = 0
-    mando.main()
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `tappy-0.9.6/src/tappy/tappy_lib/filter.py` & `tappy-1.0.0/src/tappy/tappy_lib/filter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """
 NAME:
     filter.py
 
 SYNOPSIS:
     filter.py is only an importable library
@@ -32,22 +31,22 @@
 #    or FITNESS FOR A PARTICULAR PURPOSE.  See the GNU General Public License
 #    for more details.
 #
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    675 Mass Ave, Cambridge, MA 02139, USA.
 """
+import sys
 
-# ===imports======================
 import numpy as np
 
-# ===globals======================
+debug_p = False
 modname = "filter"
 
-# ===utilities====================
+
 def msg(txt):
     """Send message to stdout."""
     sys.stdout.write(txt)
     sys.stdout.flush()
 
 
 def debug(ftn, txt):
@@ -64,17 +63,14 @@
 
 
 def usage():
     """Prints the docstring."""
     print(__doc__)
 
 
-# ====================================
-
-
 def fft_lowpass(nelevation, low_bound, high_bound):
     """Performs a low pass filter on the nelevation series.
     low_bound and high_bound specifes the boundary of the filter.
     """
     import numpy.fft as F
 
     if len(nelevation) % 2:
```

### Comparing `tappy-0.9.6/src/tappy/tappy_lib/parameter_database.py` & `tappy-1.0.0/src/tappy/tappy_lib/parameter_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 letter_to_factor_map = {
     "Z": 0,
     "Y": -1,
     "X": -2,
     "W": -3,
     "V": -4,
     "U": -5,
```

### Comparing `tappy-0.9.6/src/tappy/tappy_lib/sparser.py` & `tappy-1.0.0/src/tappy/tappy_lib/sparser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 """
 NAME:
     sparser.py
 
 SYNOPSIS:
     sparser.py [options] filename
@@ -42,18 +41,16 @@
 #    You should have received a copy of the GNU General Public License along
 #    with this program; if not, write to the Free Software Foundation, Inc.,
 #    675 Mass Ave, Cambridge, MA 02139, USA.
 """
 
 import datetime
 import getopt
-import os
-
-# ===imports======================
 import sys
+from pathlib import Path
 
 from pyparsing import *
 
 # ===globals======================
 modname = "sparser"
 __version__ = "0.3"
 
@@ -100,14 +97,15 @@
 
 # Set a default value for decimal_separator.
 decimal_sep = "."
 
 # Extra dictionary
 extra_dict = {}
 
+
 # ====================================
 class DefinitionFileNotFoundError(Exception):
     def __init__(self, def_filename):
         self.value = def_filename
 
     def __str__(self):
         return repr(self.value)
@@ -126,16 +124,15 @@
 def toString(instring, loc, tokenlist):
     """Returns an integer or real as a string."""
     return tokenlist[0]
 
 
 def toDatetime(instring, loc, tokenlist):
     """Returns a datetime object."""
-    global _origin
-    global _unit
+    global _origin, _unit
 
     exec(f"rvar = _origin + datetime.timedelta({_unit}={float(tokenlist[0])})")
     return rvar
 
 
 def isotoDate(instring, loc, tokenlist):
     """Returns a datetime object."""
@@ -145,16 +142,15 @@
 
 
 def integer(
     name, minimum=1, maximum=0, exact=0, sign=Optional(oneOf("- +")), parseAct=toInteger
 ):
     """Appends a skip/integer combination to the parse constructs."""
     lint = Combine(sign + Word(nums, min=minimum, max=maximum, exact=exact))
-    grammar.append(SkipTo(lint))
-    grammar.append(lint.setResultsName(name).setParseAction(parseAct))
+    grammar.extend([SkipTo(lint), lint.setResultsName(name).setParseAction(parseAct)])
 
 
 def positive_integer(name, minimum=1, maximum=0, exact=0):
     """Will only parse a positive integer."""
     integer(name, minimum=minimum, maximum=maximum, exact=exact, sign=Optional("+"))
 
 
@@ -181,16 +177,15 @@
         )
     else:
         lword = Combine(
             sign
             + Word(nums + decimal_sep)
             + Optional(oneOf("E e D d") + Optional(oneOf("- +")) + Word(nums))
         )
-    grammar.append(SkipTo(lword))
-    grammar.append(lword.setResultsName(name).setParseAction(parseAct))
+    grammar.extend([SkipTo(lword), lword.setResultsName(name).setParseAction(parseAct)])
 
 
 def positive_real(name, minimum=1, maximum=0, exact=0):
     """Will only parse a positive real."""
     real(name, minimum=minimum, maximum=maximum, exact=exact, sign=Optional("+"))
 
 
@@ -238,27 +233,25 @@
         + oneOf("T  ")
         + Word(nums)
         + ":"
         + Word(nums)
         + ":"
         + Word(nums)
     )
-    grammar.append(SkipTo(lword))
-    grammar.append(lword.setResultsName(name).setParseAction(parseAct))
+    grammar.extend([SkipTo(lword), lword.setResultsName(name).setParseAction(parseAct)])
 
 
 def real_as_datetime(
     name,
     sign=Optional(oneOf("- +")),
     origin=datetime.datetime(1900, 1, 1),
     unit="days",
     parseAct=toDatetime,
 ):
-    global _origin
-    global _unit
+    global _origin, _unit
     _origin = origin
     _unit = unit
     real(name, sign=Optional("- +"), parseAct=parseAct)
 
 
 def integer_as_datetime(
     name,
@@ -266,16 +259,15 @@
     maximum=0,
     exact=0,
     sign=Optional(oneOf("- +")),
     origin=datetime.datetime(1900, 1, 1),
     unit="days",
     parseAct=toDatetime,
 ):
-    global _origin
-    global _unit
+    global _origin, _unit
     _origin = origin
     _unit = unit
     integer(
         name,
         minimum=minimum,
         maximum=maximum,
         exact=exact,
@@ -283,23 +275,21 @@
         parseAct=parseAct,
     )
 
 
 def qstring(name):
     """Parses a quoted (either double or single quotes) string."""
     quoted_string = sglQuotedString | dblQuotedString
-    grammar.append(SkipTo(quoted_string))
-    grammar.append(quoted_string.setResultsName(name))
+    grammar.extend([SkipTo(quoted_string), quoted_string.setResultsName(name)])
 
 
 def delimited_as_string(name):
     """Parses out any delimited group as a string."""
     wrd = Word(alphanums)
-    grammar.append(SkipTo(wrd))
-    grammar.append(wrd.setResultsName(name))
+    grammar.extend([SkipTo(wrd), wrd.setResultsName(name)])
 
 
 def number_as_real(name, sign=Optional(oneOf("- +")), parseAct=toFloat):
     """Parses any number as a real."""
     real(name, required_decimal=False, sign=Optional(oneOf("- +")), parseAct=toFloat)
 
 
@@ -383,24 +373,26 @@
     """
 
     def __init__(self, filename, def_filename=None, mode="r"):
         """Opens input file, and if available the definition file.  If the
         definition file is available __init__ will then create some pyparsing
         helper variables."""
 
-        filen, _ = os.path.splitext(filename)
+        filen = Path(filename)
+        def_filename = Path(def_filename)
 
         # I use filelike which allows you to open up compressed files and urls
         # as files.  Test to see whether it is available.
         try:
             import filelike
 
             tmp_open = filelike.open
         except ImportError:
             tmp_open = open
+
         self.file = tmp_open(filename, mode)
 
         # Try to maintain a line count
         self.record_number = 0
 
         self.grammar = None
         self.parsedef = None
@@ -424,26 +416,26 @@
         #          integer('hour'),
         #          integer('minute'),
         #          positive_real('water_level'),
         #         ]
 
         self.line_number = 0
 
-        definition_file_one = f"{filen}.def"
-        if os.path.dirname(filen):
-            definition_file_two = f"{os.path.dirname(filen) + os.sep}sparse.def"
+        definition_file_one = filen.with_name(f"{filen.stem}.def")
+        if filen.parent.exists():
+            definition_file_two = filen.with_name("sparse.def")
         else:
             definition_file_two = "sparse.def"
 
-        if os.path.exists(definition_file_two):
+        if definition_file_two.exists():
             self.parsedef = definition_file_two
-        if os.path.exists(definition_file_one):
+        if definition_file_one.exists():
             self.parsedef = definition_file_one
         if def_filename:
-            if os.path.exists(def_filename):
+            if def_filename.exists():
                 self.parsedef = def_filename
             else:
                 raise DefinitionFileNotFoundError(def_filename)
         if self.parsedef:
             exec(open(self.parsedef).read())
             self.grammar = And(grammar[1:] + [restOfLine])
 
@@ -519,24 +511,24 @@
         print(i)
 
 
 # -------------------------
 if __name__ == "__main__":
     ftn = "main"
     opts, pargs = getopt.getopt(
-        sys.argv[1:], "hvd", ["help", "version", "debug", "bb="]
+        sys.argv[1:], "hvd", ("help", "version", "debug", "bb=")
     )
     for opt in opts:
-        if opt[0] in ["-h", "--help"]:
+        if opt[0] in ("-h", "--help"):
             print(f"{modname}: version={__version__}")
             usage()
             sys.exit(0)
-        elif opt[0] in ["-v", "--version"]:
+        elif opt[0] in ("-v", "--version"):
             print(f"{modname}: version={__version__}")
             sys.exit(0)
-        elif opt[0] in ["-d", "--debug"]:
+        elif opt[0] in ("-d", "--debug"):
             debug_p = 1
         elif opt[0] == "--bb":
             opt_b = opt[1]
 
     # ---make the object and run it---
     main(pargs)
```

### Comparing `tappy-0.9.6/src/tappy.egg-info/SOURCES.txt` & `tappy-1.0.0/src/tappy.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 .deepsource.toml
+.gitignore
 .pre-commit-config.yaml
 AUTHORS.rst
 BADGES.rst
 CHANGELOG.md
+CITATION.cff
 CONTRIBUTING.rst
 LICENSE.txt
-MANIFEST.in
 README.rst
 VERSION
 pyproject.toml
-setup.cfg
 setup.py
 .github/workflows/clean-workflow-runs.yml
 .github/workflows/python-package.yml
-dist/tappy-0.9.3.tar.gz
-dist/tappy-0.9.4.tar.gz
 docs/CompareTidalFilters.rst
 docs/Comparison_of_subtraction.png
 docs/Comparison_of_tidal_filters_large.png
 docs/Comparison_of_tidal_filters_small.png
 docs/FillMissing.rst
 docs/HarmonicAnalysis.rst
 docs/Makefile
 docs/Missing.png
 docs/TappyUsersGuide.rst
 docs/TidalScience.rst
 docs/authors.rst
+docs/citation.txt
+docs/command_line.rst
 docs/conf.py
 docs/contributing.rst
+docs/create_citations.sh
+docs/function_summary.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 example/example.sh
 example/mayport_florida_8720220_con_noaa.txt
 example/mayport_florida_8720220_con_tappy.txt
 example/mayport_florida_8720220_data.txt
@@ -40,26 +42,30 @@
 example/sparse.def
 example/tidesandcurrents.def
 example/tridentpier_florida_8721604_con_noaa.txt
 example/tridentpier_florida_8721604_con_tappy.txt
 example/tridentpier_florida_8721604_data.txt.gz
 example/tridentpier_florida_8721604_datetime.txt.def
 src/tappy/__init__.py
+src/tappy/analysis.py
+src/tappy/prediction.py
 src/tappy/tappy.py
+src/tappy/utils.py
 src/tappy.egg-info/PKG-INFO
 src/tappy.egg-info/SOURCES.txt
 src/tappy.egg-info/dependency_links.txt
 src/tappy.egg-info/entry_points.txt
-src/tappy.egg-info/not-zip-safe
 src/tappy.egg-info/requires.txt
 src/tappy.egg-info/top_level.txt
 src/tappy/tappy_lib/__init__.py
 src/tappy/tappy_lib/filter.py
 src/tappy/tappy_lib/parameter_database.py
 src/tappy/tappy_lib/sparser.py
+tests/8720218.csv
+tests/8720218_wl.csv
 tests/predict_def.out
 tests/sparse.def
 tests/test_tappy.py
 tests/output_ts/constituents.dat
 tests/output_ts/outts_2MN6.dat
 tests/output_ts/outts_2MS6.dat
 tests/output_ts/outts_2Q1.dat
```

### Comparing `tappy-0.9.6/tests/output_ts/constituents.dat` & `tappy-1.0.0/tests/output_ts/constituents.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_2MN6.dat` & `tappy-1.0.0/tests/output_ts/outts_2MN6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_2MS6.dat` & `tappy-1.0.0/tests/output_ts/outts_2MS6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_2Q1.dat` & `tappy-1.0.0/tests/output_ts/outts_2Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_2SM2.dat` & `tappy-1.0.0/tests/output_ts/outts_2SM2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_2SM6.dat` & `tappy-1.0.0/tests/output_ts/outts_2SM6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_J1.dat` & `tappy-1.0.0/tests/output_ts/outts_J1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_K1.dat` & `tappy-1.0.0/tests/output_ts/outts_K1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_M2.dat` & `tappy-1.0.0/tests/output_ts/outts_M2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_M3.dat` & `tappy-1.0.0/tests/output_ts/outts_M3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_M4.dat` & `tappy-1.0.0/tests/output_ts/outts_M4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_M6.dat` & `tappy-1.0.0/tests/output_ts/outts_M6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_M8.dat` & `tappy-1.0.0/tests/output_ts/outts_M8.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_MK3.dat` & `tappy-1.0.0/tests/output_ts/outts_MK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_MN4.dat` & `tappy-1.0.0/tests/output_ts/outts_MN4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_MO3.dat` & `tappy-1.0.0/tests/output_ts/outts_MO3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_MS4.dat` & `tappy-1.0.0/tests/output_ts/outts_MS4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_MSf.dat` & `tappy-1.0.0/tests/output_ts/outts_MSf.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_N2.dat` & `tappy-1.0.0/tests/output_ts/outts_N2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_NO1.dat` & `tappy-1.0.0/tests/output_ts/outts_NO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_O1.dat` & `tappy-1.0.0/tests/output_ts/outts_O1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_OO1.dat` & `tappy-1.0.0/tests/output_ts/outts_OO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_Q1.dat` & `tappy-1.0.0/tests/output_ts/outts_Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_S2.dat` & `tappy-1.0.0/tests/output_ts/outts_S2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_S4.dat` & `tappy-1.0.0/tests/output_ts/outts_S4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_S6.dat` & `tappy-1.0.0/tests/output_ts/outts_S6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_SK3.dat` & `tappy-1.0.0/tests/output_ts/outts_SK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_eta2.dat` & `tappy-1.0.0/tests/output_ts/outts_eta2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_2MN6.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_2MN6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_2MS6.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_2MS6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_2Q1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_2Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_2SM2.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_2SM2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_2SM6.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_2SM6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_J1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_J1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_K1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_K1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_M2.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_M2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_M3.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_M3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_M4.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_M4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_M6.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_M6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_M8.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_M8.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_MK3.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_MK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_MN4.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_MN4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_MO3.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_MO3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_MS4.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_MS4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_MSf.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_MSf.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_N2.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_N2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_NO1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_NO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_O1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_O1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_OO1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_OO1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_Q1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_Q1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_S2.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_S2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_S4.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_S4.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_S6.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_S6.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_SK3.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_SK3.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_eta2.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_eta2.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ff_ups1.dat` & `tappy-1.0.0/tests/output_ts/outts_ff_ups1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_filtered_transform.dat` & `tappy-1.0.0/tests/output_ts/outts_filtered_transform.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_original.dat` & `tappy-1.0.0/tests/output_ts/outts_original.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_total_prediction.dat` & `tappy-1.0.0/tests/output_ts/outts_total_prediction.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_total_tidal_components.dat` & `tappy-1.0.0/tests/output_ts/outts_total_tidal_components.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/output_ts/outts_ups1.dat` & `tappy-1.0.0/tests/output_ts/outts_ups1.dat`

 * *Files identical despite different names*

### Comparing `tappy-0.9.6/tests/sparse.def` & `tappy-1.0.0/tests/sparse.def`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 # You need to specify the separator between the integer part and the decimal
 # part of real numbers, even if you only have integers in your data file.
 decimal_sep = "."
 
 # TAPPy needs the variables 'year', 'month', 'day', 'hour', 'minute', 'water_level'.
 # Any other variable name can be used as a placeholder.
-parse = [ 
+parse = [
           positive_integer('year'),
           positive_integer('month'),
           positive_integer('day'),
           positive_integer('hour'),
           positive_integer('minute'),
           positive_integer('unused01'),
           real('water_level'),
          ]
-
```

### Comparing `tappy-0.9.6/tests/test_tappy.py` & `tappy-1.0.0/tests/test_tappy.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,91 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import difflib
 import glob
 import os
-import os.path
 import re
 import shlex
 import shutil
-import string
 import subprocess
 import tempfile
-import unittest
+from pathlib import Path
+from unittest import TestCase
 
 # directory dance to find tappy.py module in directory above
 # test_tappy.py
-file_loc = os.path.abspath(__file__)
-cur_path = os.path.dirname(file_loc)
+file_loc = Path(__file__).resolve()
+cur_path = file_loc.parent
 
-_cwd = os.getcwd()
 
-
-class TappyTest(unittest.TestCase):
+class TappyTest(TestCase):
     def setUp(self):
+        self.cwd = Path.cwd()
         self.tmpdir = tempfile.mkdtemp()
         os.chdir(self.tmpdir)
+        open("debug_tappy", "a").close()
         for files in ["*.dat", "*.xml"]:
             for f in glob.glob(files):
                 os.remove(f)
-        self.con_output1 = subprocess.Popen(
+        ret = subprocess.call(
             [
                 "tappy",
                 "analysis",
-                os.path.join(
-                    _cwd,
-                    "example",
-                    "mayport_florida_8720220_data.txt",
-                ),
+                self.cwd / "example" / "mayport_florida_8720220_data.txt",
                 #        '--zero_ts="transform"',
                 "--outputts",
                 '--outputxml="testout.xml"',
                 #        '--filter="transform"',
                 "--include_inferred",
-            ],
-            stdout=subprocess.PIPE,
+            ]
         )
-        sts = os.waitpid(self.con_output1.pid, 0)[1]
+        print(ret)
 
     def tearDown(self):
+        os.chdir(self.cwd)
         shutil.rmtree(self.tmpdir)
 
     def test_constituents(self):
         os.chdir(self.tmpdir)
         for i in ["M2", "M8"]:
             alines = open(
-                os.path.join(_cwd, "tests", "output_ts", f"outts_{i}.dat")
+                self.cwd / "tests" / "output_ts" / f"outts_{i}.dat"
             ).readlines()
-            blines = open(os.path.join(f"outts_{i}.dat")).readlines()
+            print(Path.cwd())
+            print(glob.glob("*"))
+            blines = open(Path(f"outts_{i}.dat")).readlines()
             d = difflib.Differ()
             result = list(d.compare(alines, blines))
             result = [i for i in result if i[0] in ["+", "-", "?"]]
             print(
                 "".join(result),
             )
             self.assertEqual(result, [])
 
     def test_closure(self):
         os.chdir(self.tmpdir)
-        inputf = os.path.join(_cwd, "example", "mayport_florida_8720220_data.txt")
-        self.con_output1 = subprocess.call(
+        inputf = self.cwd / "example" / "mayport_florida_8720220_data.txt"
+        _ = subprocess.call(
             shlex.split(
                 f"tappy analysis {inputf} --outputxml testout.xml --include_inferred"
             )
         )
-        self.con_output2 = subprocess.call(
+        _ = subprocess.call(
             shlex.split(
-                f"tappy prediction testout.xml 2000-01-01T00:00:00 2000-02-01T00:00:00 60 --fname predict.out"
+                "tappy prediction testout.xml 2000-01-01T00:00:00 2000-02-01T00:00:00 60 --fname predict.out"
             )
         )
-        def_filename = os.path.join(_cwd, "tests", "predict_def.out")
-        self.con_output3 = subprocess.call(
+        def_filename = self.cwd / "tests" / "predict_def.out"
+        _ = subprocess.call(
             shlex.split(
                 f"tappy analysis predict.out --def_filename {def_filename} --outputxml testoutclosure.xml --include_inferred"
             )
         )
+        print(os.getcwd())
+        print(glob.glob("*"))
         alines = open("testout.xml").readlines()
         blines = open("testoutclosure.xml").readlines()
         nalines = []
         for a in alines:
             match = re.search(r"[0-9\.]+", a)
             if match is not None:
                 nalines.append(str(round(float(match.group()), 2)))
```

