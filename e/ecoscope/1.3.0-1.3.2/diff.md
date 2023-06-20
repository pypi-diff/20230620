# Comparing `tmp/ecoscope-1.3.0.tar.gz` & `tmp/ecoscope-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoscope-1.3.0.tar", last modified: Mon May 22 13:50:35 2023, max compression
+gzip compressed data, was "ecoscope-1.3.2.tar", last modified: Tue Jun 20 06:55:45 2023, max compression
```

## Comparing `ecoscope-1.3.0.tar` & `ecoscope-1.3.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.230748 ecoscope-1.3.0/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-22 06:13:31.000000 ecoscope-1.3.0/LICENSE
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-22 13:50:35.230748 ecoscope-1.3.0/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-22 06:13:31.000000 ecoscope-1.3.0/README.rst
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.222747 ecoscope-1.3.0/ecoscope/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/__init__.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/analysis/
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/analysis/UD/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/UD/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/UD/etd_range.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/astronomy.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3881 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/percentile.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/proximity.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2735 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/analysis/speed.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/base/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/_dataclasses.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25180 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/base/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/contrib/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/basemaps.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/foliumap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/contrib/legend.txt
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/io/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    33272 2023-05-22 06:30:31.000000 ecoscope-1.3.0/ecoscope/io/earthranger.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/raster.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/io/utils.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.226748 ecoscope-1.3.0/ecoscope/mapping/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/mapping/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/mapping/map.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.230748 ecoscope-1.3.0/ecoscope/plotting/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/plotting/__init__.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/plotting/plot.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-05-22 06:13:31.000000 ecoscope-1.3.0/ecoscope/version.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.222747 ecoscope-1.3.0/ecoscope.egg-info/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/PKG-INFO
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/SOURCES.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/dependency_links.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-22 13:48:35.000000 ecoscope-1.3.0/ecoscope.egg-info/not-zip-safe
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      284 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/requires.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-05-22 13:50:35.000000 ecoscope-1.3.0/ecoscope.egg-info/top_level.txt
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-22 06:13:31.000000 ecoscope-1.3.0/pyproject.toml
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-05-22 13:50:35.230748 ecoscope-1.3.0/setup.cfg
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1940 2023-05-22 06:13:31.000000 ecoscope-1.3.0/setup.py
-drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-05-22 13:50:35.230748 ecoscope-1.3.0/tests/
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_base.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6955 2023-05-22 06:17:05.000000 ecoscope-1.3.0/tests/test_earthranger_io.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ecodataframe.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ecograph.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ecomap.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_eetools.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_geofence.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_immobility.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_seasons.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_speed.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_ud.py
--rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-22 06:13:31.000000 ecoscope-1.3.0/tests/test_utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.180349 ecoscope-1.3.2/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1553 2023-05-22 06:13:31.000000 ecoscope-1.3.2/LICENSE
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-06-20 06:55:45.180349 ecoscope-1.3.2/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2935 2023-05-22 06:13:31.000000 ecoscope-1.3.2/README.rst
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.116339 ecoscope-1.3.2/ecoscope/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3744 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/__init__.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope/analysis/
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope/analysis/UD/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      105 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/UD/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     7011 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/UD/etd_range.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      375 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1027 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/astronomy.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    15978 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3849 2023-06-16 19:26:49.000000 ecoscope-1.3.2/ecoscope/analysis/geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2955 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3208 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/percentile.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2147 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/proximity.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3505 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/analysis/seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2725 2023-06-16 14:29:12.000000 ecoscope-1.3.2/ecoscope/analysis/speed.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope/base/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      602 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/base/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1776 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/base/_dataclasses.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    25126 2023-06-16 20:17:33.000000 ecoscope-1.3.2/ecoscope/base/base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6650 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/base/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.176348 ecoscope-1.3.2/ecoscope/contrib/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       60 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    10988 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/basemaps.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)   112572 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/foliumap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2197 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/contrib/legend.txt
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.176348 ecoscope-1.3.2/ecoscope/io/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      272 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    33370 2023-06-08 07:55:39.000000 ecoscope-1.3.2/ecoscope/io/earthranger.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    12171 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6620 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/raster.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2225 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/io/utils.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.176348 ecoscope-1.3.2/ecoscope/mapping/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      141 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/mapping/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    17821 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/mapping/map.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.180349 ecoscope-1.3.2/ecoscope/plotting/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      376 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/plotting/__init__.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)    14348 2023-05-22 06:13:31.000000 ecoscope-1.3.2/ecoscope/plotting/plot.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       22 2023-06-16 20:24:07.000000 ecoscope-1.3.2/ecoscope/version.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.148344 ecoscope-1.3.2/ecoscope.egg-info/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     3671 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/PKG-INFO
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1322 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        1 2023-05-22 13:48:35.000000 ecoscope-1.3.2/ecoscope.egg-info/not-zip-safe
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      289 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/requires.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)        9 2023-06-20 06:55:45.000000 ecoscope-1.3.2/ecoscope.egg-info/top_level.txt
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      591 2023-05-22 06:13:31.000000 ecoscope-1.3.2/pyproject.toml
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)       38 2023-06-20 06:55:45.180349 ecoscope-1.3.2/setup.cfg
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1945 2023-06-16 18:21:45.000000 ecoscope-1.3.2/setup.py
+drwxrwxr-x   0 gitonga   (1000) gitonga   (1000)        0 2023-06-20 06:55:45.180349 ecoscope-1.3.2/tests/
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6554 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_base.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     6955 2023-05-24 09:30:01.000000 ecoscope-1.3.2/tests/test_earthranger_io.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     4840 2023-06-16 18:01:57.000000 ecoscope-1.3.2/tests/test_ecodataframe.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     5098 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_ecograph.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      285 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_ecomap.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     2907 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_eetools.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1876 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_geofence.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      790 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_immobility.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      862 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_seasons.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      306 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_speed.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)     1877 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_ud.py
+-rw-rw-r--   0 gitonga   (1000) gitonga   (1000)      329 2023-05-22 06:13:31.000000 ecoscope-1.3.2/tests/test_utils.py
```

### Comparing `ecoscope-1.3.0/LICENSE` & `ecoscope-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/PKG-INFO` & `ecoscope-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.3.0
+Version: 1.3.2
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.3.0/README.rst` & `ecoscope-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/__init__.py` & `ecoscope-1.3.2/ecoscope/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/UD/etd_range.py` & `ecoscope-1.3.2/ecoscope/analysis/UD/etd_range.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/astronomy.py` & `ecoscope-1.3.2/ecoscope/analysis/astronomy.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/ecograph.py` & `ecoscope-1.3.2/ecoscope/analysis/ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/geofence.py` & `ecoscope-1.3.2/ecoscope/analysis/geofence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import collections
 import dataclasses
 import typing
 
 import geopandas as gpd
 import pandas as pd
-import pygeos
+import shapely
 
 import ecoscope
 
 
 class Region(collections.UserDict):
     def __init__(self, geometry: typing.Any, unique_id: str = None, region_name: str = None):
         super().__init__(
@@ -71,16 +71,16 @@
 
         Returns
         -------
             ecoscope.base.EcoDataFrame
 
         """
         trajectory = trajectory.copy()
-        trajectory["start_point"] = pygeos.get_point(trajectory.geometry.values.data, 0)
-        trajectory["end_point"] = pygeos.get_point(trajectory.geometry.values.data, 1)
+        trajectory["start_point"] = shapely.get_point(trajectory.geometry, 0)
+        trajectory["end_point"] = shapely.get_point(trajectory.geometry, 1)
 
         def apply_func(fence):
             geofence = fence.geometry
             traj = trajectory.loc[trajectory.intersects(geofence)].copy()
             traj["segment_geometry"] = traj["geometry"]
             traj.set_geometry(traj.intersection(geofence), inplace=True)
             traj = traj.explode(index_parts=False)
@@ -94,15 +94,15 @@
             traj["warn_level"] = fence.warn_level
 
             # Determine containment of the subject before and after the crossing
             for index, colname in enumerate(["start_region_ids", "end_region_ids"]):
                 traj[colname] = (
                     geocrossing_profile.region_df.sjoin(
                         gpd.GeoDataFrame(
-                            geometry=pygeos.get_point(traj["segment_geometry"].values.data, index),
+                            geometry=shapely.get_point(traj["segment_geometry"], index),
                             index=traj.index,
                             crs=4326,
                         ),
                         predicate="contains",
                     )
                     .set_index("index_right")["unique_id"]
                     .groupby(level=0)
```

### Comparing `ecoscope-1.3.0/ecoscope/analysis/immobility.py` & `ecoscope-1.3.2/ecoscope/analysis/immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/percentile.py` & `ecoscope-1.3.2/ecoscope/analysis/percentile.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/proximity.py` & `ecoscope-1.3.2/ecoscope/analysis/proximity.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/seasons.py` & `ecoscope-1.3.2/ecoscope/analysis/seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/analysis/speed.py` & `ecoscope-1.3.2/ecoscope/analysis/speed.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typing
 
 import geopandas as gpd
 import mapclassify
 import pandas as pd
-import pygeos
+import shapely
 
 import ecoscope.base
 
 
 class SpeedDataFrame(ecoscope.base.EcoDataFrame):
     @classmethod
     def from_trajectory(
@@ -31,15 +31,15 @@
                 trajectory.geometry.values,
                 index=pd.Index(
                     pd.cut(x=trajectory.speed_kmhr, bins=bins, labels=speed_colors, include_lowest=True),
                     name="speed_colour",
                 ),
             )
             .groupby(level=0)
-            .apply(lambda gs: pygeos.multilinestrings(gs.values.data)),
+            .apply(lambda gs: shapely.multilinestrings(gs)),
             crs=trajectory.crs,
         )
         speed_df.reset_index(drop=False, inplace=True)
         speed_df["label"] = _speedmap_labels(bins)
         speed_df.sort_values("speed_colour", inplace=True)
 
         return speed_df
```

### Comparing `ecoscope-1.3.0/ecoscope/base/__init__.py` & `ecoscope-1.3.2/ecoscope/base/__init__.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/base/_dataclasses.py` & `ecoscope-1.3.2/ecoscope/base/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/base/base.py` & `ecoscope-1.3.2/ecoscope/base/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import warnings
 
 import astroplan
 import astropy
 import geopandas as gpd
 import numpy as np
 import pandas as pd
-import pygeos
 from pyproj import Geod
+import shapely
 
 from ecoscope.analysis import astronomy
 from ecoscope.base._dataclasses import (
     RelocsCoordinateFilter,
     RelocsDateRangeFilter,
     RelocsDistFilter,
     RelocsSpeedFilter,
@@ -475,15 +475,15 @@
                 "groupby_col": gdf.groupby_col,
                 "segment_start": gdf.fixtime,
                 "segment_end": gdf._fixtime,
                 "timespan_seconds": track_properties.timespan_seconds,
                 "dist_meters": track_properties.dist_meters,
                 "speed_kmhr": track_properties.speed_kmhr,
                 "heading": track_properties.heading,
-                "geometry": pygeos.linestrings(coords),
+                "geometry": shapely.linestrings(coords),
                 "junk_status": gdf.junk_status,
             },
             crs=4326,
             index=gdf.index,
         )
         gdf.drop(["fixtime", "_fixtime", "_geometry"], axis=1, inplace=True)
         extra_cols = gdf.columns.difference(df.columns)
@@ -558,16 +558,16 @@
             valid_i = (start_i == end_i) | (times == traj["segment_start"].iloc[start_i])
 
             traj = traj.iloc[start_i[valid_i]].reset_index(drop=True)
             times = times[valid_i]
 
             return gpd.GeoDataFrame(
                 {"fixtime": times},
-                geometry=pygeos.line_interpolate_point(
-                    traj["geometry"].values.data,
+                geometry=shapely.line_interpolate_point(
+                    traj["geometry"].values,
                     (times - traj["segment_start"]) / (traj["segment_end"] - traj["segment_start"]),
                     normalized=True,
                 ),
                 crs=traj.crs,
             )
 
         return Relocations.from_gdf(self.groupby("groupby_col").apply(f).reset_index(level=0))
@@ -578,17 +578,15 @@
         Returns
         -------
         ecoscope.base.Relocations
         """
 
         def f(traj):
             traj.crs = self.crs
-            points = np.concatenate(
-                [pygeos.get_point(traj.geometry.values.data, 0), pygeos.get_point(traj.geometry.values.data, 1)]
-            )
+            points = np.concatenate([shapely.get_point(traj.geometry, 0), shapely.get_point(traj.geometry, 1)])
             times = np.concatenate([traj["segment_start"], traj["segment_end"]])
 
             return (
                 gpd.GeoDataFrame(
                     {"fixtime": times},
                     geometry=points,
                     crs=traj.crs,
```

### Comparing `ecoscope-1.3.0/ecoscope/base/utils.py` & `ecoscope-1.3.2/ecoscope/base/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/contrib/basemaps.py` & `ecoscope-1.3.2/ecoscope/contrib/basemaps.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/contrib/foliumap.py` & `ecoscope-1.3.2/ecoscope/contrib/foliumap.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/contrib/legend.txt` & `ecoscope-1.3.2/ecoscope/contrib/legend.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/io/earthranger.py` & `ecoscope-1.3.2/ecoscope/io/earthranger.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,14 +595,17 @@
             df.loc[~df["geojson"].isna(), "geojson"]
         )["geometry"]
         df.set_crs(4326, inplace=True)
 
         df.sort_values("time", inplace=True)
         return df
 
+    def get_patrol_types(self):
+        return pd.DataFrame(self._get("activity/patrols/types"))
+
     def get_patrols(self, since=None, until=None, patrol_type=None, status=None, **addl_kwargs):
         """
         Parameters
         ----------
         since:
             lower date range
         until:
```

### Comparing `ecoscope-1.3.0/ecoscope/io/eetools.py` & `ecoscope-1.3.2/ecoscope/io/eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/io/raster.py` & `ecoscope-1.3.2/ecoscope/io/raster.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/io/utils.py` & `ecoscope-1.3.2/ecoscope/io/utils.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/mapping/map.py` & `ecoscope-1.3.2/ecoscope/mapping/map.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope/plotting/plot.py` & `ecoscope-1.3.2/ecoscope/plotting/plot.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/ecoscope.egg-info/PKG-INFO` & `ecoscope-1.3.2/ecoscope.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecoscope
-Version: 1.3.0
+Version: 1.3.2
 Summary: Standard Analytical Reporting Framework for Conservation
 Home-page: http://github.com/wildlife-dynamics/ecoscope
 Author: Jake Wall
 Author-email: walljcg@gmail.com
 License: MIT
 Platform: Posix; MacOS X; Windows
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `ecoscope-1.3.0/ecoscope.egg-info/SOURCES.txt` & `ecoscope-1.3.2/ecoscope.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/pyproject.toml` & `ecoscope-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/setup.py` & `ecoscope-1.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,16 +27,16 @@
     "networkx",
     "numba",
     "numexpr",
     "numpy<=1.22",
     "pandas",
     "plotly",
     "pyarrow",
-    "pygeos",
     "pyproj",
+    "pytest-mock",
     "rasterio",
     "scikit-image",
     "scikit-learn",
     "scipy",
     "selenium",
     "shapely",
     "tqdm",
```

### Comparing `ecoscope-1.3.0/tests/test_base.py` & `ecoscope-1.3.2/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_earthranger_io.py` & `ecoscope-1.3.2/tests/test_earthranger_io.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_ecodataframe.py` & `ecoscope-1.3.2/tests/test_ecodataframe.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_ecograph.py` & `ecoscope-1.3.2/tests/test_ecograph.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_eetools.py` & `ecoscope-1.3.2/tests/test_eetools.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_geofence.py` & `ecoscope-1.3.2/tests/test_geofence.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_immobility.py` & `ecoscope-1.3.2/tests/test_immobility.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_seasons.py` & `ecoscope-1.3.2/tests/test_seasons.py`

 * *Files identical despite different names*

### Comparing `ecoscope-1.3.0/tests/test_ud.py` & `ecoscope-1.3.2/tests/test_ud.py`

 * *Files identical despite different names*

