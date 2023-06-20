# Comparing `tmp/garmin-fit-sdk-21.107.0.tar.gz` & `tmp/garmin-fit-sdk-21.115.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/fit-python-sdk/fit-python-sdk/dist/tmpsvcgut40/garmin-fit-sdk-21.107.0.tar", last modified: Tue Feb 21 23:15:47 2023, max compression
+gzip compressed data, was "/home/runner/work/fit-python-sdk/fit-python-sdk/dist/tmpjpncssxq/garmin-fit-sdk-21.115.0.tar", last modified: Tue Jun 20 16:43:52 2023, max compression
```

## Comparing `garmin-fit-sdk-21.107.0.tar` & `garmin-fit-sdk-21.115.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/
--rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/fit.py
--rw-r--r--   0 runner    (1001) docker     (122)   694557 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/profile.py
--rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     6790 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/crc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (122)    30552 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)     3340 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/bitstream.py
--rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/accumulator.py
--rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk/hr_mesg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      804 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/.github/workflows/run_tests.yml
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/tests/
--rw-r--r--   0 runner    (1001) docker     (122)    11160 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (122)   328393 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/data_expand_hr_mesgs.py
--rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_hr_mesg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/tests/fits/
--rw-r--r--   0 runner    (1001) docker     (122)    90970 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/fits/WithGearChangeData.fit
--rw-r--r--   0 runner    (1001) docker     (122)    25121 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/fits/HrmPluginTestActivity.fit
--rw-r--r--   0 runner    (1001) docker     (122)    94199 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/fits/ActivityDevFields.fit
--rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (122)    36149 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/data.py
--rw-r--r--   0 runner    (1001) docker     (122)    20099 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (122)      509 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5565 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_bitstream.py
--rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/tests/test_crc_calculator.py
--rw-r--r--   0 runner    (1001) docker     (122)     8653 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      187 2023-02-21 23:15:33.000000 garmin-fit-sdk-21.107.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     8750 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      926 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       21 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-02-21 23:15:46.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     8750 2023-02-21 23:15:47.000000 garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      187 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/.github/workflows/run_tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      804 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      560 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       21 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     9022 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      926 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     8928 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/
+-rw-r--r--   0 runner    (1001) docker     (122)     6512 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/hr_mesg_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)   724926 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/profile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3850 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/fit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2304 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31129 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6790 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1223 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3340 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/bitstream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2261 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/crc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1859 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/garmin_fit_sdk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)    11160 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2065 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_hr_mesg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 16:43:52.000000 garmin-fit-sdk-21.115.0/tests/fits/
+-rw-r--r--   0 runner    (1001) docker     (122)    25121 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/fits/HrmPluginTestActivity.fit
+-rw-r--r--   0 runner    (1001) docker     (122)    94199 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/fits/ActivityDevFields.fit
+-rw-r--r--   0 runner    (1001) docker     (122)    90970 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/fits/WithGearChangeData.fit
+-rw-r--r--   0 runner    (1001) docker     (122)     5565 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_bitstream.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22488 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5222 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1316 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1716 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_crc_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (122)      509 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    37052 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1011 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/test_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (122)   328393 2023-06-20 16:43:37.000000 garmin-fit-sdk-21.115.0/tests/data_expand_hr_mesgs.py
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/fit.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/fit.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 BASE_TYPE = {
     "ENUM": 0x00,
     "SINT8": 0x01,
     "UINT8": 0x02,
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/profile.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 Profile = {
     'version': {
         'major': 21,
-        'minor': 107,
+        'minor': 115,
         'patch': 0,
         'type': "Release"
     },
     'common_fields': {
         'part_index': 250,
         'timestamp': 253,
         'message_index': 254
@@ -4997,14 +4997,42 @@
             'units': "",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        38: {
+            'num': 38,
+            'name': "end_position_lat",
+            'type': "sint32",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "semicircles",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        39: {
+            'num': 39,
+            'name': "end_position_long",
+            'type': "sint32",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "semicircles",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         41: {
             'num': 41,
             'name': "avg_stroke_count",
             'type': "uint32",
             'array': "false",
             'scale': [10],
             'offset': [0],
@@ -5767,14 +5795,28 @@
             'units': "percent",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        110: {
+            'num': 110, # Sport name from associated sport mesg
+            'name': "sport_profile_name",
+            'type': "string",
+            'array': "true",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         111: {
             'num': 111,
             'name': "sport_index",
             'type': "uint8",
             'array': "false",
             'scale': [1],
             'offset': [0],
@@ -6439,14 +6481,70 @@
             'units': "Flow",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        194: {
+            'num': 194, # Average SPO2 for the monitoring session
+            'name': "avg_spo2",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "percent",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        195: {
+            'num': 195, # Average stress for the monitoring session
+            'name': "avg_stress",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "percent",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        197: {
+            'num': 197, # Standard deviation of R-R interval (SDRR) - Heart rate variability measure most useful for wellness users.
+            'name': "sdrr_hrv",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "mS",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        198: {
+            'num': 198, # Root mean square successive difference (RMSSD) - Heart rate variability measure most useful for athletes
+            'name': "rmssd_hrv",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "mS",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         199: {
             'num': 199, # fractional part of total_ascent
             'name': "total_fractional_ascent",
             'type': "uint8",
             'array': "false",
             'scale': [100],
             'offset': [0],
@@ -9446,14 +9544,28 @@
             'units': "mm",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        87: {
+            'num': 87, # Supports larger cycle sizes needed for paddlesports. Max cycle size: 655.35
+            'name': "cycle_length16",
+            'type': "uint16",
+            'array': "false",
+            'scale': [100],
+            'offset': [0],
+            'units': "m",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         91: {
             'num': 91, # Includes atmospheric pressure
             'name': "absolute_pressure",
             'type': "uint32",
             'array': "false",
             'scale': [1],
             'offset': [0],
@@ -9614,14 +9726,28 @@
             'units': "",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        116: {
+            'num': 116, # Current Stress value
+            'name': "current_stress",
+            'type': "uint16",
+            'array': "false",
+            'scale': [100],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         117: {
             'num': 117,
             'name': "ebike_travel_range",
             'type': "uint16",
             'array': "false",
             'scale': [1],
             'offset': [0],
@@ -10139,14 +10265,28 @@
                 'components': [],
                 'has_components': False,
                 'map':[
                     { 'num': 0, 'name': "event", 'raw_value': 56, 'value_name': "dive_alert" },
                 ],
                },
                {
+                'name': "auto_activity_detect_duration", 
+                'type': "uint16",
+                'array': "",
+                'scale': [1],
+                'offset': [0],
+                'units': ["min"],
+                'bits': [],
+                'components': [],
+                'has_components': False,
+                'map':[
+                    { 'num': 0, 'name': "event", 'raw_value': 54, 'value_name': "auto_activity_detect" },
+                ],
+               },
+               {
                 'name': "radar_threat_alert",  # The first byte is the radar_threat_level_max, the second byte is the radar_threat_count, third bytes is the average approach speed, and the 4th byte is the max approach speed
                 'type': "uint32",
                 'array': "",
                 'scale': [1, 1, 10, 10, ],
                 'offset': [0, 0, 0, 0, ],
                 'units': ["", "", "", "", ],
                 'bits': [8,8,8,8,],
@@ -10266,14 +10406,56 @@
             'units': "",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        14: {
+            'num': 14, # Activity Type associated with an auto_activity_detect event
+            'name': "activity_type",
+            'type': "activity_type",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        15: {
+            'num': 15, # Timestamp of when the event started
+            'name': "start_timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "s",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': [{
+                'name': "auto_activity_detect_start_timestamp",  # Auto Activity Detect Start Timestamp.
+                'type': "date_time",
+                'array': "",
+                'scale': [1],
+                'offset': [0],
+                'units': ["s"],
+                'bits': [],
+                'components': [],
+                'has_components': False,
+                'map':[
+                    { 'num': 0, 'name': "event", 'raw_value': 54, 'value_name': "auto_activity_detect" },
+                ],
+               },
+               ]
+            },
         21: {
             'num': 21, # Do not populate directly. Autogenerated by decoder for threat_alert subfield components.
             'name': "radar_threat_level_max",
             'type': "radar_threat_level_type",
             'array': "false",
             'scale': [1],
             'offset': [0],
@@ -15599,14 +15781,28 @@
     },
 },
         26: {
         'num': "26",
         'name': "workout",
         'messages_key': "workout_mesgs",
         'fields': {
+        254: {
+            'num': 254,
+            'name': "message_index",
+            'type': "message_index",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
         4: {
             'num': 4,
             'name': "sport",
             'type': "sport",
             'array': "false",
             'scale': [1],
             'offset': [0],
@@ -17168,14 +17364,28 @@
             'units': "",
             'bits': [],
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
+        13: {
+            'num': 13,
+            'name': "bmi",
+            'type': "uint16",
+            'array': "false",
+            'scale': [10],
+            'offset': [0],
+            'units': "kg/m^2",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
     },
 },
         51: {
         'num': "51",
         'name': "blood_pressure",
         'messages_key': "blood_pressure_mesgs",
         'fields': {
@@ -17865,14 +18075,126 @@
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
     },
 },
+        211: {
+        'num': "211",
+        'name': "monitoring_hr_data",
+        'messages_key': "monitoring_hr_data_mesgs",
+        'fields': {
+        253: {
+            'num': 253, # Must align to logging interval, for example, time must be 00:00:00 for daily log.
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "s",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0, # 7-day rolling average
+            'name': "resting_heart_rate",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "bpm",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        1: {
+            'num': 1, # RHR for today only. (Feeds into 7-day average)
+            'name': "current_day_resting_heart_rate",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "bpm",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
+        269: {
+        'num': "269",
+        'name': "spo2_data",
+        'messages_key': "spo2_data_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "s",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0,
+            'name': "reading_spo2",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "percent",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        1: {
+            'num': 1,
+            'name': "reading_confidence",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        2: {
+            'num': 2, # Mode when data was captured
+            'name': "mode",
+            'type': "spo2_measurement_type",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
         132: {
         'num': "132",
         'name': "hr",
         'messages_key': "hr_mesgs",
         'fields': {
         253: {
             'num': 253,
@@ -17991,14 +18313,133 @@
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
     },
 },
+        229: {
+        'num': "229",
+        'name': "max_met_data",
+        'messages_key': "max_met_data_mesgs",
+        'fields': {
+        0: {
+            'num': 0, # Time maxMET and vo2 were calculated
+            'name': "update_time",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        2: {
+            'num': 2,
+            'name': "vo2_max",
+            'type': "uint16",
+            'array': "false",
+            'scale': [10],
+            'offset': [0],
+            'units': "mL/kg/min",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        5: {
+            'num': 5,
+            'name': "sport",
+            'type': "sport",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        6: {
+            'num': 6,
+            'name': "sub_sport",
+            'type': "sub_sport",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        8: {
+            'num': 8,
+            'name': "max_met_category",
+            'type': "max_met_category",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        9: {
+            'num': 9, # Indicates if calibrated data was used in the calculation
+            'name': "calibrated_data",
+            'type': "bool",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        12: {
+            'num': 12, # Indicates if the estimate was obtained using a chest strap or wrist heart rate
+            'name': "hr_source",
+            'type': "max_met_heart_rate_source",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        13: {
+            'num': 13, # Indidcates if the estimate was obtained using onboard GPS or connected GPS
+            'name': "speed_source",
+            'type': "max_met_speed_source",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
         145: {
         'num': "145",
         'name': "memo_glob",
         'messages_key': "memo_glob_mesgs",
         'fields': {
         250: {
             'num': 250, # Sequence number of memo blocks
@@ -18082,14 +18523,49 @@
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
     },
 },
+        275: {
+        'num': "275",
+        'name': "sleep_level",
+        'messages_key': "sleep_level_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "s",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0,
+            'name': "sleep_level",
+            'type': "sleep_level",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
         82: {
         'num': "82",
         'name': "ant_channel_id",
         'messages_key': "ant_channel_id_mesgs",
         'fields': {
         0: {
             'num': 0,
@@ -19006,14 +19482,252 @@
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
     },
 },
+        290: {
+        'num': "290", # Array of heart beat intervals
+        'name': "beat_intervals",
+        'messages_key': "beat_intervals_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0, # Milliseconds past date_time
+            'name': "timestamp_ms",
+            'type': "uint16",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        1: {
+            'num': 1, # Array of millisecond times between beats
+            'name': "time",
+            'type': "uint16",
+            'array': "true",
+            'scale': [1],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
+        370: {
+        'num': "370",
+        'name': "hrv_status_summary",
+        'messages_key': "hrv_status_summary_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0, # 7 day RMSSD average over sleep
+            'name': "weekly_average",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        1: {
+            'num': 1, # Last night RMSSD average over sleep
+            'name': "last_night_average",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        2: {
+            'num': 2, # 5 minute high RMSSD value over sleep
+            'name': "last_night_5_min_high",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        3: {
+            'num': 3, # 3 week baseline, upper boundary of low HRV status
+            'name': "baseline_low_upper",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        4: {
+            'num': 4, # 3 week baseline, lower boundary of balanced HRV status
+            'name': "baseline_balanced_lower",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        5: {
+            'num': 5, # 3 week baseline, upper boundary of balanced HRV status
+            'name': "baseline_balanced_upper",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        6: {
+            'num': 6,
+            'name': "status",
+            'type': "hrv_status",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
+        371: {
+        'num': "371",
+        'name': "hrv_value",
+        'messages_key': "hrv_value_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0, # 5 minute RMSSD
+            'name': "value",
+            'type': "uint16",
+            'array': "false",
+            'scale': [128],
+            'offset': [0],
+            'units': "ms",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
+        297: {
+        'num': "297",
+        'name': "respiration_rate",
+        'messages_key': "respiration_rate_mesgs",
+        'fields': {
+        253: {
+            'num': 253,
+            'name': "timestamp",
+            'type': "date_time",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        0: {
+            'num': 0, # Breaths * 100 /min, -300 indicates invalid, -200 indicates large motion, -100 indicates off wrist
+            'name': "respiration_rate",
+            'type': "sint16",
+            'array': "false",
+            'scale': [100],
+            'offset': [0],
+            'units': "breaths/min",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
         319: {
         'num': "319",
         'name': "tank_update",
         'messages_key': "tank_update_mesgs",
         'fields': {
         253: {
             'num': 253,
@@ -19132,14 +19846,217 @@
             'components': [],
             'is_accumulated': False,
             'has_components': False,
 			'sub_fields': []
             },
     },
 },
+        346: {
+        'num': "346",
+        'name': "sleep_assessment",
+        'messages_key': "sleep_assessment_mesgs",
+        'fields': {
+        0: {
+            'num': 0, # Average of awake_time_score and awakenings_count_score. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "combined_awake_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        1: {
+            'num': 1, # Score that evaluates the total time spent awake between sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "awake_time_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        2: {
+            'num': 2, # Score that evaluates the number of awakenings that interrupt sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "awakenings_count_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        3: {
+            'num': 3, # Score that evaluates the amount of deep sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "deep_sleep_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        4: {
+            'num': 4, # Score that evaluates the quality of sleep based on sleep stages, heart-rate variability and possible awakenings during the night. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "sleep_duration_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        5: {
+            'num': 5, # Score that evaluates the amount of light sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "light_sleep_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        6: {
+            'num': 6, # Total score that summarizes the overall quality of sleep, combining sleep duration and quality. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "overall_sleep_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        7: {
+            'num': 7, # Score that evaluates the quality of sleep based on sleep stages, heart-rate variability and possible awakenings during the night. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "sleep_quality_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        8: {
+            'num': 8, # Score that evaluates stress and recovery during sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "sleep_recovery_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        9: {
+            'num': 9, # Score that evaluates the amount of REM sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "rem_sleep_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        10: {
+            'num': 10, # Score that evaluates the amount of restlessness during sleep. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "sleep_restlessness_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        11: {
+            'num': 11, # The number of awakenings during sleep.
+            'name': "awakenings_count",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        14: {
+            'num': 14, # Score that evaluates the sleep interruptions. If valid: 0 (worst) to 100 (best). If unknown: FIT_UINT8_INVALID.
+            'name': "interruptions_score",
+            'type': "uint8",
+            'array': "false",
+            'scale': [1],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+        15: {
+            'num': 15, # Excludes stress during awake periods in the sleep window
+            'name': "average_stress_during_sleep",
+            'type': "uint16",
+            'array': "false",
+            'scale': [100],
+            'offset': [0],
+            'units': "",
+            'bits': [],
+            'components': [],
+            'is_accumulated': False,
+            'has_components': False,
+			'sub_fields': []
+            },
+    },
+},
         105: {
         'num': "105",
         'name': "pad",
         'messages_key': "pad_mesgs",
         'fields': {
     },
 },
@@ -19243,27 +20160,36 @@
         '201': 'exd_data_field_configuration',
         '202': 'exd_data_concept_configuration',
         '206': 'field_description',
         '207': 'developer_data_id',
         '208': 'magnetometer_data',
         '209': 'barometer_data',
         '210': 'one_d_sensor_calibration',
+        '211': 'monitoring_hr_data',
         '216': 'time_in_zone',
         '225': 'set',
         '227': 'stress_level',
+        '229': 'max_met_data',
         '258': 'dive_settings',
         '259': 'dive_gas',
         '262': 'dive_alarm',
         '264': 'exercise_title',
         '268': 'dive_summary',
+        '269': 'spo2_data',
+        '275': 'sleep_level',
         '285': 'jump',
+        '290': 'beat_intervals',
+        '297': 'respiration_rate',
         '312': 'split',
         '317': 'climb_pro',
         '319': 'tank_update',
         '323': 'tank_summary',
+        '346': 'sleep_assessment',
+        '370': 'hrv_status_summary',
+        '371': 'hrv_value',
         '375': 'device_aux_battery_info',
         '393': 'dive_apnea_alarm',
         '0xFF00': 'mfg_range_min', # 0xFF00 - 0xFFFE reserved for manufacturer specific messages
         '0xFFFE': 'mfg_range_max', # 0xFF00 - 0xFFFE reserved for manufacturer specific messages
         },
     'checksum': {
         '0': 'clear', # Allows clear of checksum for flash memory where can only write 1 to 0 without erasing sector.
@@ -19745,14 +20671,24 @@
         '69': 'bouldering', # Climbing
         '70': 'hiit', # High Intensity Interval Training
         '73': 'amrap', # HIIT
         '74': 'emom', # HIIT
         '75': 'tabata', # HIIT
         '84': 'pickleball', # Racket
         '85': 'padel', # Racket
+        '110': 'fly_canopy', # Flying
+        '111': 'fly_paraglide', # Flying
+        '112': 'fly_paramotor', # Flying
+        '113': 'fly_pressurized', # Flying
+        '114': 'fly_navigate', # Flying
+        '115': 'fly_timer', # Flying
+        '116': 'fly_altimeter', # Flying
+        '117': 'fly_wx', # Flying
+        '118': 'fly_vfr', # Flying
+        '119': 'fly_ifr', # Flying
         '254': 'all',
         },
     'sport_event': {
         '0': 'uncategorized',
         '1': 'geocaching',
         '2': 'fitness',
         '3': 'recreation',
@@ -19858,14 +20794,15 @@
         '36': 'calibration', # start/stop/marker
         '42': 'front_gear_change', # marker
         '43': 'rear_gear_change', # marker
         '44': 'rider_position_change', # marker
         '45': 'elev_high_alert', # Group 0. Start / stop when in alert condition.
         '46': 'elev_low_alert', # Group 0. Start / stop when in alert condition.
         '47': 'comm_timeout', # marker
+        '54': 'auto_activity_detect', # marker
         '56': 'dive_alert', # marker
         '57': 'dive_gas_switched', # marker
         '71': 'tank_pressure_reserve', # marker
         '72': 'tank_pressure_critical', # marker
         '73': 'tank_lost', # marker
         '75': 'radar_threat_alert', # start/stop/marker
         '76': 'tank_battery_low', # marker
@@ -20192,14 +21129,17 @@
         '139': 'kinetic_sports',
         '140': 'decathlon_byte',
         '141': 'tq_systems',
         '142': 'tag_heuer',
         '143': 'keiser_fitness',
         '144': 'zwift_byte',
         '145': 'porsche_ep',
+        '146': 'blackbird',
+        '147': 'meilan_byte',
+        '148': 'ezon',
         '255': 'development',
         '257': 'healthandlife',
         '258': 'lezyne',
         '259': 'scribe_labs',
         '260': 'zwift',
         '261': 'watteam',
         '262': 'recon',
@@ -20259,14 +21199,16 @@
         '316': 'vasa',
         '317': 'race_republic',
         '318': 'fazua',
         '319': 'oreka_training',
         '320': 'lsec', # Lishun Electric & Communication
         '321': 'lululemon_studio',
         '322': 'shanyue',
+        '323': 'spinning_mda',
+        '324': 'hilldating',
         '5759': 'actigraphcorp',
         },
     'garmin_product': {
         '1': 'hrm1',
         '2': 'axh01', # AXH01 HRM chipset
         '3': 'axb01',
         '4': 'axb02',
@@ -20513,14 +21455,15 @@
         '3113': 'fr945',
         '3121': 'edge_530',
         '3122': 'edge_830',
         '3126': 'instinct_esports',
         '3134': 'fenix5s_plus_apac',
         '3135': 'fenix5x_plus_apac',
         '3142': 'edge_520_plus_apac',
+        '3143': 'descent_t1',
         '3144': 'fr235l_asia',
         '3145': 'fr245_asia',
         '3163': 'vivo_active3m_apac',
         '3192': 'gen3_bsm', # gen3 bike speed sensor
         '3193': 'gen3_bcm', # gen3 bike cadence sensor
         '3218': 'vivo_smart4_asia',
         '3224': 'vivoactive4_small',
@@ -20600,14 +21543,15 @@
         '3813': 'edge_130_plus_asia',
         '3823': 'approach_s12',
         '3872': 'enduro_asia',
         '3837': 'venusq_asia',
         '3843': 'edge_1040',
         '3850': 'marq_golfer_asia',
         '3851': 'venu2_plus',
+        '3865': 'gnss',
         '3869': 'fr55',
         '3888': 'instinct_2',
         '3905': 'fenix7s',
         '3906': 'fenix7',
         '3907': 'fenix7x',
         '3908': 'fenix7s_apac',
         '3909': 'fenix7_apac',
@@ -20629,40 +21573,52 @@
         '3993': 'fr255_small',
         ' 4001': 'approach_g12_asia',
         '4002': 'approach_s42_asia',
         '4005': 'descent_g1',
         '4017': 'venu2_plus_asia',
         '4024': 'fr955',
         '4033': 'fr55_asia',
+        '4061': 'edge_540',
+        '4062': 'edge_840',
         '4063': 'vivosmart_5',
         '4071': 'instinct_2_asia',
         '4105': 'marq_gen2', # Adventurer, Athlete, Captain, Golfer
         '4115': 'venusq2',
         '4116': 'venusq2music',
         '4124': 'marq_gen2_aviator',
         '4125': 'd2_air_x10',
         '4130': 'hrm_pro_plus',
         '4132': 'descent_g1_asia',
         '4135': 'tactix7',
         '4155': 'instinct_crossover',
         '4169': 'edge_explore2',
+        '4233': 'approach_s70',
+        '4257': 'fr265_large',
+        '4258': 'fr265_small',
         '4265': 'tacx_neo_smart', # Neo Smart, Tacx
         '4266': 'tacx_neo2_smart', # Neo 2 Smart, Tacx
         '4267': 'tacx_neo2_t_smart', # Neo 2T Smart, Tacx
         '4268': 'tacx_neo_smart_bike', # Neo Smart Bike, Tacx
         '4269': 'tacx_satori_smart', # Satori Smart, Tacx
         '4270': 'tacx_flow_smart', # Flow Smart, Tacx
         '4271': 'tacx_vortex_smart', # Vortex Smart, Tacx
         '4272': 'tacx_bushido_smart', # Bushido Smart, Tacx
         '4273': 'tacx_genius_smart', # Genius Smart, Tacx
         '4274': 'tacx_flux_flux_s_smart', # Flux/Flux S Smart, Tacx
         '4275': 'tacx_flux2_smart', # Flux 2 Smart, Tacx
         '4276': 'tacx_magnum', # Magnum, Tacx
         '4305': 'edge_1040_asia',
+        '4312': 'epix_gen2_pro_42',
+        '4313': 'epix_gen2_pro_47',
+        '4314': 'epix_gen2_pro_51',
+        '4315': 'fr965',
         '4341': 'enduro2',
+        '4375': 'fenix7_pro_solar',
+        '4394': 'instinct_2x',
+        '4442': 'descent_t2',
         '10007': 'sdm4', # SDM4 footpod
         '10014': 'edge_remote',
         '20533': 'tacx_training_app_win',
         '20534': 'tacx_training_app_mac',
         '20565': 'tacx_training_app_mac_catalyst',
         '20119': 'training_center',
         '30045': 'tacx_training_app_android',
@@ -21533,14 +22489,18 @@
         '1': 'kilogram',
         '2': 'pound',
         },
     'set_type': {
         '0': 'rest',
         '1': 'active',
         },
+    'max_met_category': {
+        '0': 'generic',
+        '1': 'cycling',
+        },
     'exercise_category': {
         '0': 'bench_press',
         '1': 'calf_raise',
         '2': 'cardio',
         '3': 'carry',
         '4': 'chop',
         '5': 'core',
@@ -22938,14 +23898,27 @@
         '1': 'time', # Alarm when a certain time has transpired
         '2': 'speed', # Alarm when a certain ascent or descent rate is exceeded
         },
     'dive_backlight_mode': {
         '0': 'at_depth',
         '1': 'always_on',
         },
+    'sleep_level': {
+        '0': 'unmeasurable',
+        '1': 'awake',
+        '2': 'light',
+        '3': 'deep',
+        '4': 'rem',
+        },
+    'spo2_measurement_type': {
+        '0': 'off_wrist',
+        '1': 'spot_check',
+        '2': 'continuous_check',
+        '3': 'periodic',
+        },
     'ccr_setpoint_switch_mode': {
         '0': 'manual', # User switches setpoints manually
         '1': 'automatic', # Switch automatically based on depth
         },
     'dive_gas_mode': {
         '0': 'open_circuit',
         '1': 'closed_circuit_diluent',
@@ -22994,14 +23967,30 @@
         },
     'radar_threat_level_type': {
         '0': 'threat_unknown',
         '1': 'threat_none',
         '2': 'threat_approaching',
         '3': 'threat_approaching_fast',
         },
+    'max_met_speed_source': {
+        '0': 'onboard_gps',
+        '1': 'connected_gps',
+        '2': 'cadence',
+        },
+    'max_met_heart_rate_source': {
+        '0': 'whr', # Wrist Heart Rate Monitor
+        '1': 'hrm', # Chest Strap Heart Rate Monitor
+        },
+    'hrv_status': {
+        '0': 'none',
+        '1': 'poor',
+        '2': 'low',
+        '3': 'unbalanced',
+        '4': 'balanced',
+        },
     'no_fly_time_mode': {
         '0': 'standard', # Standard Diver Alert Network no-fly guidance
         '1': 'flat_24_hours', # Flat 24 hour no-fly guidance
         },
         },
     'mesg_num' : {
         'FILE_ID': 0,
@@ -23080,23 +24069,32 @@
         'EXERCISE_TITLE': 264,
         'SCHEDULE': 28,
         'TOTALS': 33,
         'WEIGHT_SCALE': 30,
         'BLOOD_PRESSURE': 51,
         'MONITORING_INFO': 103,
         'MONITORING': 55,
+        'MONITORING_HR_DATA': 211,
+        'SPO2_DATA': 269,
         'HR': 132,
         'STRESS_LEVEL': 227,
+        'MAX_MET_DATA': 229,
         'MEMO_GLOB': 145,
+        'SLEEP_LEVEL': 275,
         'ANT_CHANNEL_ID': 82,
         'ANT_RX': 80,
         'ANT_TX': 81,
         'EXD_SCREEN_CONFIGURATION': 200,
         'EXD_DATA_FIELD_CONFIGURATION': 201,
         'EXD_DATA_CONCEPT_CONFIGURATION': 202,
         'DIVE_SUMMARY': 268,
         'HRV': 78,
+        'BEAT_INTERVALS': 290,
+        'HRV_STATUS_SUMMARY': 370,
+        'HRV_VALUE': 371,
+        'RESPIRATION_RATE': 297,
         'TANK_UPDATE': 319,
         'TANK_SUMMARY': 323,
+        'SLEEP_ASSESSMENT': 346,
         'PAD': 105,
     }
 }
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/util.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 from datetime import datetime, timezone
 
 FIT_EPOCH_S = 631065600
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/stream.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 import os
 from enum import Enum
 from io import BufferedReader, BytesIO
 from struct import unpack
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/__init__.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 from garmin_fit_sdk.accumulator import Accumulator
 from garmin_fit_sdk.bitstream import BitStream
 from garmin_fit_sdk.crc_calculator import CrcCalculator
 from garmin_fit_sdk.decoder import Decoder
 from garmin_fit_sdk.fit import BASE_TYPE, BASE_TYPE_DEFINITIONS
 from garmin_fit_sdk.hr_mesg_utils import expand_heart_rates
 from garmin_fit_sdk.profile import Profile
 from garmin_fit_sdk.stream import Stream
 from garmin_fit_sdk.util import FIT_EPOCH_S, convert_timestamp_to_datetime
 
-__version__ = '21.107.0'
+__version__ = '21.115.0'
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/crc_calculator.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/crc_calculator.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 _CRC_TABLE = [
     0x0000, 0xCC01, 0xD801, 0x1400, 0xF001, 0x3C00, 0x2800, 0xE401,
     0xA001, 0x6C00, 0x7800, 0xB401, 0x5000, 0x9C01, 0x8801, 0x4400
 ]
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/decoder.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/decoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,29 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 import copy
 
 from . import Accumulator, BitStream, CrcCalculator
 from . import fit as FIT
 from . import hr_mesg_utils, util
 from .profile import Profile
 from .stream import Endianness, Stream
 
 _CRCSIZE = 2
+_COMPRESSED_HEADER_MASK = 0x80
 _MESG_DEFINITION_MASK = 0x40
 _MESG_HEADER_MASK = 0x00
 _LOCAL_MESG_NUM_MASK = 0x0F
 _DEV_DATA_MASK = 0x20
 
 
 class Decoder:
@@ -51,14 +52,15 @@
         self._fields_with_subfields = []
         self._fields_to_expand = []
 
         self._mesg_listener = None
         self._apply_scale_and_offset = True
         self._convert_timestamps_to_datetimes = True
         self._convert_types_to_strings = True
+        self._enable_crc_check = True
         self._expand_sub_fields = True
         self._expand_components = True
         self._merge_heart_rates = True
 
 
     def is_fit(self):
         '''Returns whether the file is a valid fit file.'''
@@ -103,22 +105,24 @@
             return False
 
         return True
 
     def read(self, apply_scale_and_offset = True,
                 convert_datetimes_to_dates = True,
                 convert_types_to_strings = True,
+                enable_crc_check = True,
                 expand_sub_fields = True,
                 expand_components = True,
                 merge_heart_rates = True,
                 mesg_listener = None):
         '''Reads the entire contents of the fit file and returns the decoded messages'''
         self._apply_scale_and_offset = apply_scale_and_offset
         self._convert_timestamps_to_datetimes = convert_datetimes_to_dates
         self._convert_types_to_strings = convert_types_to_strings
+        self._enable_crc_check = enable_crc_check
         self._expand_sub_fields = expand_sub_fields
         self._expand_components = expand_components
         self._merge_heart_rates = merge_heart_rates
         self._mesg_listener = mesg_listener
 
         self._local_mesg_defs = {}
         self._developer_data_defs = {}
@@ -148,32 +152,38 @@
 
     def __decode_next_file(self):
         position = self._stream.position()
 
         if self.is_fit() is False:
             self.__raise_error("The file is not a fit file.")
 
-        self._stream.set_crc_calculator(CrcCalculator())
+        crc_calculator = CrcCalculator() if self._enable_crc_check is True else None
+        self._stream.set_crc_calculator(crc_calculator)
 
         file_header = self.read_file_header(False)
 
         # Read data definitions and messages
         while self._stream.position() < (position + file_header.header_size + file_header.data_size):
             self.__decode_next_record()
 
-        # Check the CRC
-        calculated_crc = self._stream.get_crc_caclulator().get_crc()
+
+        self._stream.set_crc_calculator(None)
         crc = self._stream.read_unint_16()
 
-        if crc != calculated_crc:
-            self.__raise_error("CRC Error")
+        if crc_calculator is not None:
+            calculated_crc = crc_calculator.get_crc()
+            if crc != calculated_crc:
+                self.__raise_error("CRC Error")
 
     def __decode_next_record(self):
         record_header = self._stream.peek_byte()
 
+        if record_header & _COMPRESSED_HEADER_MASK == _COMPRESSED_HEADER_MASK:
+            self.__decode_compressed_timestamp_message()
+
         if record_header & _MESG_DEFINITION_MASK == _MESG_HEADER_MASK:
             self.__decode_message()
 
         if record_header & _MESG_DEFINITION_MASK == _MESG_DEFINITION_MASK:
             self.__decode_mesg_def()
 
     def __decode_mesg_def(self):
@@ -309,14 +319,16 @@
 
         # Append decoded message
         self._messages[messages_key].append(message)
 
         if self._mesg_listener is not None:
             self._mesg_listener(mesg_def['global_mesg_num'], message)
 
+    def __decode_compressed_timestamp_message(self):
+        self.__raise_error("Compressed timestamp messages are not currently supported")
 
     def __read_message(self, mesg_def):
         message = {}
         raw_values = self.__read_raw_values(mesg_def["message_size"], mesg_def["struct_format_string"])
 
         index = 0
         for field in mesg_def['field_definitions']:
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/bitstream.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/bitstream.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 from . import fit as FIT
 
 
 class BitStream:
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/accumulator.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/accumulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 class AccumulatedField:
     '''A class that accumulates a value for a particular field.
         Attributes:
             _accumulated_value: Resulting accumulated value
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk/hr_mesg_utils.py` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk/hr_mesg_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 ###########################################################################################
 # Copyright 2023 Garmin International, Inc.
 # Licensed under the Flexible and Interoperable Data Transfer (FIT) Protocol License; you
 # may not use this file except in compliance with the Flexible and Interoperable Data
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 # ****WARNING****  This file is auto-generated!  Do NOT edit this file.
-# Profile Version = 21.107Release
-# Tag = production/release/21.107.00-0-geade151
+# Profile Version = 21.115Release
+# Tag = production/release/21.115.00-0-gfe0a7f8
 ############################################################################################
 
 
 from datetime import datetime
 
 from . import util
```

### Comparing `garmin-fit-sdk-21.107.0/.github/workflows/publish.yml` & `garmin-fit-sdk-21.115.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/.github/workflows/run_tests.yml` & `garmin-fit-sdk-21.115.0/.github/workflows/run_tests.yml`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/test_stream.py` & `garmin-fit-sdk-21.115.0/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/test_accumulator.py` & `garmin-fit-sdk-21.115.0/tests/test_accumulator.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/data_expand_hr_mesgs.py` & `garmin-fit-sdk-21.115.0/tests/data_expand_hr_mesgs.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/test_hr_mesg_utils.py` & `garmin-fit-sdk-21.115.0/tests/test_hr_mesg_utils.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/fits/WithGearChangeData.fit` & `garmin-fit-sdk-21.115.0/tests/fits/WithGearChangeData.fit`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/fits/HrmPluginTestActivity.fit` & `garmin-fit-sdk-21.115.0/tests/fits/HrmPluginTestActivity.fit`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/fits/ActivityDevFields.fit` & `garmin-fit-sdk-21.115.0/tests/fits/ActivityDevFields.fit`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/test_util.py` & `garmin-fit-sdk-21.115.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/test_errors.py` & `garmin-fit-sdk-21.115.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/data.py` & `garmin-fit-sdk-21.115.0/tests/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,14 +42,28 @@
     fit_file_short_new = bytearray([
         0x0E, 0x20, 0x8B, 0x08, 0x24, 0x00, 0x00, 0x00, 0x2E, 0x46, 0x49, 0x54, 0x8E, 0xA3,  # File Header
         0x40, 0x00, 0x00, 0x00, 0x00, 0x04, 0x00, 0x01, 0x00, 0x01, 0x02, 0x84, 0x04, 0x04, 0x86, 0x08, 0x0A, 0x07, # Message Definition
         0x00, 0x04, 0x01, 0x00, 0x00, 0xCA, 0x9A, 0x3B, 0x61, 0x62, 0x63, 0x64, 0x65, 0x66, 0x67, 0x68, 0x69, 0x00, # Message
         0x5D, 0xF2  # CRC
     ])
 
+    fit_file_short_compressed_timestamp = bytearray([
+        0x0E, 0x20, 0x8B, 0x08, 0x24, 0x00, 0x00, 0x00, 0x2E, 0x46, 0x49, 0x54, 0x8E, 0xA3, # File Header
+        0x40, 0x00, 0x00, 0x00, 0x00, 0x04, 0x00, 0x01, 0x00, 0x01, 0x02, 0x84, 0x04, 0x04, 0x86, 0x08, 0x0A, 0x07, # Message Definition
+        0x80, 0x04, 0x01, 0x00, 0x00, 0xCA, 0x9A, 0x3B, 0x61, 0x62, 0x63, 0x64, 0x65, 0x66, 0x67, 0x68, 0x69, 0x00, # Message
+        0x5D, 0xF2
+    ])
+
+    fit_file_short_new_invalid_crc = bytearray([
+        0x0E, 0x20, 0x8B, 0x08, 0x24, 0x00, 0x00, 0x00, 0x2E, 0x46, 0x49, 0x54, 0x8E, 0xA3,  # File Header
+        0x40, 0x00, 0x00, 0x00, 0x00, 0x04, 0x00, 0x01, 0x00, 0x01, 0x02, 0x84, 0x04, 0x04, 0x86, 0x08, 0x0A, 0x07, # Message Definition
+        0x00, 0x04, 0x01, 0x00, 0x00, 0xCA, 0x9A, 0x3B, 0x61, 0x62, 0x63, 0x64, 0x65, 0x66, 0x67, 0x68, 0x69, 0x00, # Message
+        0xFF, 0xFF  # CRC
+    ])
+
     fit_file_short_none_array = bytearray([
         0x0E, 0x20, 0x8B, 0x08, 0x24, 0x00, 0x00, 0x00, 0x2E, 0x46, 0x49, 0x54, 0x8E, 0xA3,  # File Header
         0x40, 0x00, 0x00, 0x00, 0x00, 0x04, 0x00, 0x01, 0x00, 0x01, 0x02, 0x84, 0x04, 0x04, 0x86, 0x08, 0x0A, 0x07, # Message Definition
         0x00, 0x04, 0x01, 0x00, 0x00, 0xCA, 0x9A, 0x3B, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, 0x00, # Message
         0x6C, 0x15  # CRC
     ])
```

### Comparing `garmin-fit-sdk-21.107.0/tests/test_decoder.py` & `garmin-fit-sdk-21.115.0/tests/test_decoder.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Transfer (FIT) Protocol License.
 ###########################################################################################
 
 
 from datetime import datetime, timezone
 
 import pytest
-from garmin_fit_sdk import Decoder, Stream
+from garmin_fit_sdk import Decoder, Stream, CrcCalculator
 
 from tests.data import Data
 
 
 class TestCheckIntegrity:
     '''Set of tests verify that the decoder class correctly tests the integrity of one or more fit files.'''
     @pytest.mark.parametrize(
@@ -90,14 +90,23 @@
         '''Tests that the decoder successfully reads fit files and returns the correct number of messages.'''
         stream = Stream.from_byte_array(data)
         decoder = Decoder(stream)
         messages, errors = decoder.read()
         assert len(errors) == 0
         assert decoder.get_num_messages() == num_messages
 
+    def test_compressed_timestamp_message_should_throw(self):
+        '''Tests that the decoder should throw an error when reading a message with a compressed timestamp'''
+        stream = Stream.from_byte_array(Data.fit_file_short_compressed_timestamp)
+        decoder = Decoder(stream)
+        messages, errors = decoder.read()
+
+        assert len(errors) == 1
+        assert "Compressed timestamp messages are not currently supported" in str(errors[0])
+
     def test_read_incorrect_field_def_size(self):
         '''Tests that the decoder doesn't break when reading a message with an incorrect field definition size.'''
         stream = Stream.from_byte_array(Data.fit_file_short_with_wrong_field_def_size)
         decoder = Decoder(stream)
         messages, errors = decoder.read(convert_datetimes_to_dates=False)
 
         assert len(errors) == 0
@@ -247,14 +256,57 @@
 
     @pytest.mark.parametrize(
         "option_status",
         [
             (True),
             (False),
             (None)
+        ], ids=["Set to True", "Set to False", "Default should have CRC calculations enabled"]
+    )
+    def test_enable_crc_options(self, mocker, option_status):
+        '''Tests enabling and disabling CRC calculation when decoding a FIT file.'''
+        spy_add_bytes = mocker.spy(CrcCalculator, "add_bytes")
+        spy_get_crc = mocker.spy(CrcCalculator, "get_crc")
+
+        stream = Stream.from_byte_array(Data.fit_file_short)
+        decoder = Decoder(stream)
+
+        if option_status is not None:
+            messages, errors = decoder.read(enable_crc_check=option_status)
+        else:
+            messages, errors = decoder.read()
+
+        assert len(errors) == 0
+
+        assert spy_add_bytes.call_count == 0 if option_status is False else spy_add_bytes.call_count > 0
+        assert spy_get_crc.call_count == 0 if option_status is False else spy_get_crc.call_count > 0
+
+    @pytest.mark.parametrize(
+        "option_status, data, expected_error_status",
+        [
+            (True, Data.fit_file_short_new, False),
+            (True, Data.fit_file_short_new_invalid_crc, True),
+            (False, Data.fit_file_short_new, False),
+            (False, Data.fit_file_short_new_invalid_crc, False),
+        ], ids=["With CRC | Valid File", "With CRC | Invalid File", "Without CRC | Valid File", "Without CRC | Invalid File"]
+    )
+    def test_enable_crc_options_errors_returned(self, option_status, data, expected_error_status):
+        '''Tests if errors are returned when decoding a file when CRC calculations are enabled or disabled.'''
+        stream = Stream.from_byte_array(data)
+        decoder = Decoder(stream)
+        messages, errors = decoder.read(enable_crc_check=option_status)
+
+        assert len(errors) == 0 if expected_error_status is False else len(errors) > 0
+
+    @pytest.mark.parametrize(
+        "option_status",
+        [
+            (True),
+            (False),
+            (None)
         ], ids=["Set to True", "Set to False", "Default should expand sub fields"]
     )
     def test_expand_sub_fields_options(self, option_status):
         '''Tests the validity of expanding sub fields of messages decoded from a fit file'''
         stream = Stream.from_file('tests/fits/WithGearChangeData.fit')
         decoder = Decoder(stream)
         if option_status is not None:
```

### Comparing `garmin-fit-sdk-21.107.0/tests/test_bitstream.py` & `garmin-fit-sdk-21.115.0/tests/test_bitstream.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/tests/test_crc_calculator.py` & `garmin-fit-sdk-21.115.0/tests/test_crc_calculator.py`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/README.md` & `garmin-fit-sdk-21.115.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 The Read method accepts an optional options object that can be used to customize how field data is represented in the decoded messages. All options are enabled by default. Disabling options may speed up file decoding. Options may also be enabled or disable based on how the decoded data will be used.
 
 ```py
 messages, errors = read(
             apply_scale_and_offset = True,
             convert_datetimes_to_dates = True,
             convert_types_to_strings = True,
+            enable_crc_check = True,
             expand_sub_fields = True,
             expand_components = True,
             merge_heart_rates = True,
             mesg_listener = None)
 ```
 #### mesg_listener
 Optional callback function that can be used to inspect or manipulate messages after they are fully decoded and all the options have been applied. The message is mutable and we be returned from the Read method in the messages dictionary.
@@ -104,14 +105,16 @@
 ```
 When false the raw field value is used.
 ```py
 {
   'altitude': 10435 ## raw value store in file
 }
 ```
+#### enable_crc_check: true | false
+When true the CRC of the file is calculated when decoding a FIT file and then validated with the CRC found in the file. Disabling the CRC calculation will improve the performance of the read method.
 #### expand_sub_fields: true | false
 When true subfields are created for fields as defined in the FIT Profile.
 ```py
 {
   'event': 'rear_gear_change',
   'data': 16717829,
   'gear_change_data':16717829 ## Sub Field of data when event == 'rear_gear_change'
```

### Comparing `garmin-fit-sdk-21.107.0/setup.cfg` & `garmin-fit-sdk-21.115.0/setup.cfg`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = garmin-fit-sdk
-version = 21.107.0
+version = 21.115.0
 author = Garmin International, Inc.
 url = https://github.com/garmin/fit-python-sdk
 description = Garmin FIT Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = garmin, fit sdk, fit
 license_files = LICENSE.txt
```

### Comparing `garmin-fit-sdk-21.107.0/PKG-INFO` & `garmin-fit-sdk-21.115.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-fit-sdk
-Version: 21.107.0
+Version: 21.115.0
 Summary: Garmin FIT Python SDK
 Home-page: https://github.com/garmin/fit-python-sdk
 Author: Garmin International, Inc.
 License: UNKNOWN
 Keywords: garmin,fit sdk,fit
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -72,14 +72,15 @@
 The Read method accepts an optional options object that can be used to customize how field data is represented in the decoded messages. All options are enabled by default. Disabling options may speed up file decoding. Options may also be enabled or disable based on how the decoded data will be used.
 
 ```py
 messages, errors = read(
             apply_scale_and_offset = True,
             convert_datetimes_to_dates = True,
             convert_types_to_strings = True,
+            enable_crc_check = True,
             expand_sub_fields = True,
             expand_components = True,
             merge_heart_rates = True,
             mesg_listener = None)
 ```
 #### mesg_listener
 Optional callback function that can be used to inspect or manipulate messages after they are fully decoded and all the options have been applied. The message is mutable and we be returned from the Read method in the messages dictionary.
@@ -116,14 +117,16 @@
 ```
 When false the raw field value is used.
 ```py
 {
   'altitude': 10435 ## raw value store in file
 }
 ```
+#### enable_crc_check: true | false
+When true the CRC of the file is calculated when decoding a FIT file and then validated with the CRC found in the file. Disabling the CRC calculation will improve the performance of the read method.
 #### expand_sub_fields: true | false
 When true subfields are created for fields as defined in the FIT Profile.
 ```py
 {
   'event': 'rear_gear_change',
   'data': 16717829,
   'gear_change_data':16717829 ## Sub Field of data when event == 'rear_gear_change'
```

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/SOURCES.txt` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `garmin-fit-sdk-21.107.0/garmin_fit_sdk.egg-info/PKG-INFO` & `garmin-fit-sdk-21.115.0/garmin_fit_sdk.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-fit-sdk
-Version: 21.107.0
+Version: 21.115.0
 Summary: Garmin FIT Python SDK
 Home-page: https://github.com/garmin/fit-python-sdk
 Author: Garmin International, Inc.
 License: UNKNOWN
 Keywords: garmin,fit sdk,fit
 Platform: UNKNOWN
 Requires-Python: >=3.6
@@ -72,14 +72,15 @@
 The Read method accepts an optional options object that can be used to customize how field data is represented in the decoded messages. All options are enabled by default. Disabling options may speed up file decoding. Options may also be enabled or disable based on how the decoded data will be used.
 
 ```py
 messages, errors = read(
             apply_scale_and_offset = True,
             convert_datetimes_to_dates = True,
             convert_types_to_strings = True,
+            enable_crc_check = True,
             expand_sub_fields = True,
             expand_components = True,
             merge_heart_rates = True,
             mesg_listener = None)
 ```
 #### mesg_listener
 Optional callback function that can be used to inspect or manipulate messages after they are fully decoded and all the options have been applied. The message is mutable and we be returned from the Read method in the messages dictionary.
@@ -116,14 +117,16 @@
 ```
 When false the raw field value is used.
 ```py
 {
   'altitude': 10435 ## raw value store in file
 }
 ```
+#### enable_crc_check: true | false
+When true the CRC of the file is calculated when decoding a FIT file and then validated with the CRC found in the file. Disabling the CRC calculation will improve the performance of the read method.
 #### expand_sub_fields: true | false
 When true subfields are created for fields as defined in the FIT Profile.
 ```py
 {
   'event': 'rear_gear_change',
   'data': 16717829,
   'gear_change_data':16717829 ## Sub Field of data when event == 'rear_gear_change'
```

