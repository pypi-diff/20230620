# Comparing `tmp/rt_range-0.3.0.tar.gz` & `tmp/rt_range-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rt_range-0.3.0.tar", last modified: Mon Jun 19 21:31:40 2023, max compression
+gzip compressed data, was "rt_range-0.3.1.tar", last modified: Tue Jun 20 08:44:17 2023, max compression
```

## Comparing `rt_range-0.3.0.tar` & `rt_range-0.3.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-19 21:31:29.000000 rt_range-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-19 21:31:40.632707 rt_range-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-19 21:31:29.000000 rt_range-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-19 21:31:29.000000 rt_range-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 21:31:40.632707 rt_range-0.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.628707 rt_range-0.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.628707 rt_range-0.3.0/src/rt_range/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range/ethernet/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/eth_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range/ethernet/ncom/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/ncom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/ncom/batch_s.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/ncom/ncom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range/ethernet/rcom/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/extended_range_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/lane_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rt_packet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/rt_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-19 21:31:29.000000 rt_range-0.3.0/src/rt_range/ethernet/status_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/src/rt_range.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-19 21:31:40.000000 rt_range-0.3.0/src/rt_range.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 21:31:40.632707 rt_range-0.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_eth_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_ncom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rcom_extended_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rcom_lane.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rcom_wrapped_ncom.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-19 21:31:29.000000 rt_range-0.3.0/test/test_rt_packet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 08:44:03.000000 rt_range-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-20 08:44:17.370065 rt_range-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-06-20 08:44:03.000000 rt_range-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-20 08:44:03.000000 rt_range-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 08:44:17.374065 rt_range-0.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.366064 rt_range-0.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/src/rt_range/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/src/rt_range/ethernet/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/eth_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/src/rt_range/ethernet/ncom/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/ncom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9357 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/ncom/batch_s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/ncom/ncom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/src/rt_range/ethernet/rcom/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/rcom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/rcom/extended_range_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/rcom/lane_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/rt_packet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/rt_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-06-20 08:44:03.000000 rt_range-0.3.1/src/rt_range/ethernet/status_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/src/rt_range.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-06-20 08:44:17.000000 rt_range-0.3.1/src/rt_range.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-06-20 08:44:17.000000 rt_range-0.3.1/src/rt_range.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 08:44:17.000000 rt_range-0.3.1/src/rt_range.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 08:44:17.000000 rt_range-0.3.1/src/rt_range.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 08:44:17.000000 rt_range-0.3.1/src/rt_range.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 08:44:17.370065 rt_range-0.3.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-06-20 08:44:03.000000 rt_range-0.3.1/test/test_eth_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-20 08:44:03.000000 rt_range-0.3.1/test/test_ncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-20 08:44:03.000000 rt_range-0.3.1/test/test_rcom_extended_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-06-20 08:44:03.000000 rt_range-0.3.1/test/test_rcom_lane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-06-20 08:44:03.000000 rt_range-0.3.1/test/test_rcom_wrapped_ncom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-06-20 08:44:03.000000 rt_range-0.3.1/test/test_rt_packet.py
```

### Comparing `rt_range-0.3.0/LICENSE.txt` & `rt_range-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/PKG-INFO` & `rt_range-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt_range
-Version: 0.3.0
+Version: 0.3.1
 Summary: OxTS RT-Range data parsing utility
 License: MIT License
         
         Copyright (c) 2023 Sheetlar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `rt_range-0.3.0/README.md` & `rt_range-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/common.py` & `rt_range-0.3.1/src/rt_range/common.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/eth_parser.py` & `rt_range-0.3.1/src/rt_range/ethernet/eth_parser.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/ncom/batch_s.py` & `rt_range-0.3.1/src/rt_range/ethernet/ncom/batch_s.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     ],
     20: [
         Field('differential_corrections_age', Short),
         Field('station_ID_byte_0', Byte),
         Field('station_ID_byte_1', Byte),
         Field('station_ID_byte_2', Byte),
         Field('station_ID_byte_3', Byte),
-        Field('reserved', UByte),
+        Field('reserved', UShort),
     ],
     21: [
         Field('disk_space_remaining', Long, unit='kB'),
         Field('current_data_file_size', Long, unit='kB'),
     ],
     22: [
         Field('time_mismatch_counter', UShort),
```

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/ncom/ncom.py` & `rt_range-0.3.1/src/rt_range/ethernet/ncom/ncom.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/rcom/extended_range_packet.py` & `rt_range-0.3.1/src/rt_range/ethernet/rcom/extended_range_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/rcom/lane_packet.py` & `rt_range-0.3.1/src/rt_range/ethernet/rcom/lane_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py` & `rt_range-0.3.1/src/rt_range/ethernet/rcom/wrapped_ncom_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/rt_packet.py` & `rt_range-0.3.1/src/rt_range/ethernet/rt_packet.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/rt_types.py` & `rt_range-0.3.1/src/rt_range/ethernet/rt_types.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range/ethernet/status_definitions.py` & `rt_range-0.3.1/src/rt_range/ethernet/status_definitions.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/src/rt_range.egg-info/PKG-INFO` & `rt_range-0.3.1/src/rt_range.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rt-range
-Version: 0.3.0
+Version: 0.3.1
 Summary: OxTS RT-Range data parsing utility
 License: MIT License
         
         Copyright (c) 2023 Sheetlar
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `rt_range-0.3.0/src/rt_range.egg-info/SOURCES.txt` & `rt_range-0.3.1/src/rt_range.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/test/test_eth_parser.py` & `rt_range-0.3.1/test/test_eth_parser.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/test/test_ncom.py` & `rt_range-0.3.1/test/test_ncom.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/test/test_rcom_extended_range.py` & `rt_range-0.3.1/test/test_rcom_extended_range.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/test/test_rcom_lane.py` & `rt_range-0.3.1/test/test_rcom_lane.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/test/test_rcom_wrapped_ncom.py` & `rt_range-0.3.1/test/test_rcom_wrapped_ncom.py`

 * *Files identical despite different names*

### Comparing `rt_range-0.3.0/test/test_rt_packet.py` & `rt_range-0.3.1/test/test_rt_packet.py`

 * *Files identical despite different names*

