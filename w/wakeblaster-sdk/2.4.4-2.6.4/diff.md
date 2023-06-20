# Comparing `tmp/wakeblaster-sdk-2.4.4.tar.gz` & `tmp/wakeblaster-sdk-2.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wakeblaster-sdk-2.4.4.tar", last modified: Thu Mar 18 17:57:02 2021, max compression
+gzip compressed data, was "dist\wakeblaster-sdk-2.6.4.tar", last modified: Tue Jun 20 12:23:26 2023, max compression
```

## Comparing `wakeblaster-sdk-2.4.4.tar` & `wakeblaster-sdk-2.6.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/energytoolbox/
--rw-rw-rw-   0        0        0     5546 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/energytoolbox/flow_case_maker.py
--rw-rw-rw-   0        0        0     3806 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/energytoolbox/tab_file_parser.py
--rw-rw-rw-   0        0        0      561 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.4.4/energytoolbox/util.py
--rw-rw-rw-   0        0        0     5868 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.4.4/energytoolbox/wakeblaster_dependencies.py
--rw-rw-rw-   0        0        0     7198 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/energytoolbox/wakeblaster_simulation.py
--rw-rw-rw-   0        0        0     1514 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/energytoolbox/wind_frequency_matrix.py
--rw-rw-rw-   0        0        0     1954 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/energytoolbox/yield_calculator.py
--rw-rw-rw-   0        0        0      525 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/energytoolbox/__init__.py
--rw-rw-rw-   0        0        0      734 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/PKG-INFO
--rw-rw-rw-   0        0        0       84 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.4.4/README.md
--rw-rw-rw-   0        0        0       64 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/setup.cfg
--rw-rw-rw-   0        0        0     3204 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.4.4/setup.py
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/
--rw-rw-rw-   0        0        0     2629 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/example.py
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/
--rw-rw-rw-   0        0        0  1170512 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/flow-plane.h5
--rw-rw-rw-   0        0        0     6158 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/Lillgrund.json
--rw-rw-rw-   0        0        0      444 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/simulator-config.json
--rw-rw-rw-   0        0        0     2608 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/SWT-2.3-93m.wtg
--rw-rw-rw-   0        0        0       39 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblasterexamples/__init__.py
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/emd/
--rw-rw-rw-   0        0        0    13442 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/emd/converters.py
--rw-rw-rw-   0        0        0     4516 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/emd/submit.py
--rw-rw-rw-   0        0        0     9681 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/emd/wakeRequest.py
--rw-rw-rw-   0        0        0     3434 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/emd/wakeResult.py
--rw-rw-rw-   0        0        0       52 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/emd/__init__.py
--rw-rw-rw-   0        0        0     8314 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/flow_plane_plots.py
--rw-rw-rw-   0        0        0    23761 2021-03-04 15:03:56.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/sdk.py
--rw-rw-rw-   0        0        0      535 2021-03-04 14:16:55.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/__init__.py
--rw-rw-rw-   0        0        0       23 2021-03-18 17:57:00.000000 wakeblaster-sdk-2.4.4/wakeblastersdk/__version__.py
-drwxrwxrwx   0        0        0        0 2021-03-18 17:57:02.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/
--rw-rw-rw-   0        0        0        1 2021-03-18 17:57:01.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       85 2021-03-18 17:57:01.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      734 2021-03-18 17:57:01.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       43 2021-03-18 17:57:01.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0     1043 2021-03-18 17:57:01.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       49 2021-03-18 17:57:01.000000 wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:26.000000 wakeblaster-sdk-2.6.4/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/
+-rw-rw-rw-   0        0        0     5546 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/flow_case_maker.py
+-rw-rw-rw-   0        0        0     3806 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/tab_file_parser.py
+-rw-rw-rw-   0        0        0      561 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/energytoolbox/util.py
+-rw-rw-rw-   0        0        0     6717 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_dependencies.py
+-rw-rw-rw-   0        0        0     7198 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_simulation.py
+-rw-rw-rw-   0        0        0     1514 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/wind_frequency_matrix.py
+-rw-rw-rw-   0        0        0     1954 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/yield_calculator.py
+-rw-rw-rw-   0        0        0      525 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/energytoolbox/__init__.py
+-rw-rw-rw-   0        0        0      734 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0       84 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/README.md
+-rw-rw-rw-   0        0        0       64 2023-06-20 12:23:26.000000 wakeblaster-sdk-2.6.4/setup.cfg
+-rw-rw-rw-   0        0        0     3204 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/
+-rw-rw-rw-   0        0        0     2629 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/example.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/
+-rw-rw-rw-   0        0        0  1170512 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/flow-plane.h5
+-rw-rw-rw-   0        0        0     6158 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/Lillgrund.json
+-rw-rw-rw-   0        0        0      444 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/simulator-config.json
+-rw-rw-rw-   0        0        0     2608 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/SWT-2.3-93m.wtg
+-rw-rw-rw-   0        0        0       39 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblasterexamples/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/
+-rw-rw-rw-   0        0        0    13810 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/converters.py
+-rw-rw-rw-   0        0        0     4854 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/submit.py
+-rw-rw-rw-   0        0        0    11435 2023-03-20 14:39:30.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeRequest.py
+-rw-rw-rw-   0        0        0     3434 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeResult.py
+-rw-rw-rw-   0        0        0       52 2020-07-23 13:24:25.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/emd/__init__.py
+-rw-rw-rw-   0        0        0     8314 2021-01-06 14:57:00.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/flow_plane_plots.py
+-rw-rw-rw-   0        0        0    25630 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/sdk.py
+-rw-rw-rw-   0        0        0      584 2023-06-20 12:22:50.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-20 12:23:24.000000 wakeblaster-sdk-2.6.4/wakeblastersdk/__version__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      734 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1043 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       49 2023-06-20 12:23:25.000000 wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/top_level.txt
```

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/flow_case_maker.py` & `wakeblaster-sdk-2.6.4/energytoolbox/flow_case_maker.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/tab_file_parser.py` & `wakeblaster-sdk-2.6.4/energytoolbox/tab_file_parser.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/util.py` & `wakeblaster-sdk-2.6.4/energytoolbox/util.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/wakeblaster_dependencies.py` & `wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_dependencies.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,41 +5,49 @@
 class WindFarm:
     """
     Holder for information relating to a WakeBlaster wind farm (a.k.a asset)
     
     :param farm_description: wind farm description - see WakeBlaster docs
     :param wind_resource_grid: Contents of a WASP style .wrg or .rsf file
     :param farm_turbulence: wind farm default turbulence - see WakeBlaster docs
+    :param associated_WS: associateded wind speed, speedups between different points - see WakeBlaster docs
+    :param regional_roughness: regional roughness length - see WakeBlaster docs
     """
-    def __init__(self, farm_description, wind_resource_grid=None, farm_turbulence=None, associated_WS=None):
+    def __init__(self, farm_description, wind_resource_grid=None, farm_turbulence=None, associated_WS=None, regional_roughness=None):
         self._description = farm_description
         self._resource_grid = wind_resource_grid
         self._turbulence = farm_turbulence
         self._associated_WS = associated_WS
-
+        self._regional_roughness = regional_roughness
+        
     @classmethod
-    def from_file(cls, farm_file_path_json, wind_resource_grid_file_path=None, farm_turbulence_file_json=None):
+    def from_file(cls, farm_file_path_json, wind_resource_grid_file_path=None, farm_turbulence_file_json=None, regional_roughness_file_json=None):
         """
         Create WakeBlaster wind farm from file paths
 
         :param farm_file_path_json: JSON file describing the wind farm - see WakeBlaster docs
         :param wind_resource_grid_file_path: Path to WASP style .wrg or .rsf file
         :param farm_turbulence_file_json: JSON file describing wind farm turbulence - see WakeBlaster docs
+        :param regional_roughness_file_json: JSON file describing regional roughness - see WakeBlaster docs
         """
         with open(farm_file_path_json, 'r') as fp:
             farm_description = json.load(fp)
         wind_resource_grid = None
         if wind_resource_grid_file_path:
             with open(wind_resource_grid_file_path, 'r') as fp:
                 wind_resource_grid = fp.read()
         farm_turbulence = None
         if farm_turbulence_file_json:
             with open(farm_turbulence_file_json, 'r') as fp:
                 farm_turbulence = json.load(fp)
-        return cls(farm_description, wind_resource_grid, farm_turbulence)
+        regional_roughness = None
+        if regional_roughness_file_json:
+            with open(regional_roughness_file_json, 'r') as fp:
+                regional_roughness = json.load(fp)
+        return cls(farm_description=farm_description, wind_resource_grid=wind_resource_grid, farm_turbulence=farm_turbulence, regional_roughness=regional_roughness)
 
     def get_reference_id(self):
         def has(key):
             return key in self._description and len(self._description[key]) > 0
 
         if has('met_mast_instances'):
             return self._description['met_mast_instances'][0]['id']
@@ -60,14 +68,18 @@
     def turbulence(self):
         return self._turbulence
 
     @property
     def associated_WS(self):
         return self._associated_WS
 
+    @property
+    def regional_roughness(self):
+        return self._regional_roughness
+
 
 class WakeBlasterDependencies:
     """
     Portal for dependencies of a WakeBlaster simulation: Loads designs and farms into the WakeBlaster repository.
 
     :param api_key: You unique WakeBlaster API key
     :param api_url: URL of WakeBlaster API
@@ -113,15 +125,15 @@
         :param reference_id: Identifier of the turbine in the farm that should be used as the reference location for wind speeds. If 'None', it will use any location in the wind farm (which is irrelevant if there are no terrain effects)
         :param upload: If True (default), the wind farm will be uploaded to the WakeBlaster app. Setting upload=False can save time if the farm and its designs have previously been uplaoded
         :param associated_WS: Speed-ups between the reference point and the turbines
         """
         self._farm_id = farm_id
         self._reference_id = wind_farm.get_reference_id() if reference_id is None else reference_id
         if upload:
-            wb.upload_asset(farm_id, wind_farm.description, wind_farm.resource_grid, wind_farm.turbulence, associated_wind_speeds=wind_farm.associated_WS)
+            wb.upload_asset(farm_id, wind_farm.description, wind_farm.resource_grid, wind_farm.turbulence, associated_wind_speeds=wind_farm.associated_WS, regional_roughness=wind_farm.regional_roughness)
 
     @property
     def simulation_config(self):
         return self._simulation_config
 
     @property
     def farm_id(self):
```

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/wakeblaster_simulation.py` & `wakeblaster-sdk-2.6.4/energytoolbox/wakeblaster_simulation.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/wind_frequency_matrix.py` & `wakeblaster-sdk-2.6.4/energytoolbox/wind_frequency_matrix.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/yield_calculator.py` & `wakeblaster-sdk-2.6.4/energytoolbox/yield_calculator.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/energytoolbox/__init__.py` & `wakeblaster-sdk-2.6.4/energytoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/PKG-INFO` & `wakeblaster-sdk-2.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wakeblaster-sdk
-Version: 2.4.4
+Version: 2.6.4
 Summary: The WakeBlaster SDK
 Home-page: http://www.wakeblaster.net
 Author: ProPlanEn Ltd.
 Author-email: wakeblaster@proplanen.net
 License: UNKNOWN
 Description: # WakeBlaster SDK
```

### Comparing `wakeblaster-sdk-2.4.4/setup.py` & `wakeblaster-sdk-2.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblasterexamples/example.py` & `wakeblaster-sdk-2.6.4/wakeblasterexamples/example.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/flow-plane.h5` & `wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/flow-plane.h5`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/Lillgrund.json` & `wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/Lillgrund.json`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblasterexamples/examples/SWT-2.3-93m.wtg` & `wakeblaster-sdk-2.6.4/wakeblasterexamples/examples/SWT-2.3-93m.wtg`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/emd/converters.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/converters.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,28 +4,34 @@
 from contextlib import contextmanager
 import shutil
 import zipfile
 from os import path
 import logging
 import hashlib
 import bisect
+import numpy as np
+import pandas as pd
 
 LOGGER = logging.getLogger(__name__)
 
+REFERENCE_ID = 'reference'
+REF_DESIGN_ID = 'reference'
+
 def to_wtg(turbine_type):
     root = et.Element('WindTurbineGenerator', RotorDiameter=str(turbine_type.RotorDiameter), FormatVersion='1.01', Description='WindReq-WTG')
     et.SubElement(root, 'Comments').text = 'Generated by WakeBlaster SDK from WindPRO WakeReq format'
+    et.SubElement(root, 'DefaultOperatingMode').text = str(turbine_type.defaultMode)
     et.SubElement(et.SubElement(root, 'SuggestedHeights'), 'Height').text = str(turbine_type.HubHeight)
     for name, mode in turbine_type.Modes.items():
         perf_table = et.SubElement(
             root,
             'PerformanceTable',
             AirDensity=str(mode.airDensity),
             StationaryThrustCoEfficient=str(mode.stationaryThrustCoefficient),
-            OperatingMode=str(name)
+            OperatingMode=mode.id
         )
         et.SubElement(
             perf_table,
             'StartStopStrategy',
             LowSpeedCutIn=str(turbine_type.CutIn), LowSpeedCutOut=str(turbine_type.CutIn),
             HighSpeedCutIn=str(turbine_type.CutOut), HighSpeedCutOut=str(turbine_type.CutOut)
         )
@@ -36,32 +42,35 @@
     return et.tostring(root).decode('utf8')
 
 def to_design_descriptions(wake_req_file):
     for design_id, turbine_type in wake_req_file.TurbineTypes.items():
         yield design_id, to_wtg(turbine_type)
 
 def to_reference_design(wake_req_file):
-    return 'reference', {'height': wake_req_file.Reference.height}
+    return REF_DESIGN_ID, {'height': wake_req_file.Reference.height}
+
+def to_qualified_id(farm_id, design_id):
+    return '{}_{}'.format(farm_id, design_id)
 
-def to_turbine_description(turbine):
+def to_turbine_description(farm_id, turbine):
     return {
         'id': turbine.id,
-        'design_id': turbine.Type.id,
+        'design_id': to_qualified_id(farm_id, turbine.Type.id),
         'easting': turbine.x,
         'northing': turbine.y,
         'elevation': turbine.z
     }
 
-def to_wind_farm_description(turbines, reference):
-    return {'turbine_instances': [to_turbine_description(t) for t in turbines],
-            'met_mast_instances': [{'id': 'reference',
+def to_wind_farm_description(farm_id, turbines, reference):
+    return {'turbine_instances': [to_turbine_description(farm_id, t) for t in turbines],
+            'met_mast_instances': [{'id': REFERENCE_ID,
                                     'easting': reference.x,
                                     'northing': reference.y,
                                     'elevation': reference.z,
-                                    'design_id': 'reference'}]}
+                                    'design_id': REF_DESIGN_ID}]}
 
 def to_json(etree):
     result = {}
     for child in etree:
         if child.text and child.text.strip():
             result[child.tag] = child.text.strip()
         else:
@@ -72,14 +81,16 @@
     for client_configuration in client_configurations:
         if client_configuration.name.lower() == 'wakeblaster':
             config_tree = et.fromstring(client_configuration.contents)
             return to_json(config_tree)
     return {}
 
 def to_wind_farm_turbulence(farm):
+    if farm.turbulencesData is None:
+        return None
     wind_speeds, wind_directions = set(), set()
     value_lines = []
     for line in farm.turbulencesData.split('\r\n')[1:]:
         values = [float(v) for v in line.strip().split(' ') if v]
         if len(values) != 3:
             continue
         value_lines.append(values)
@@ -94,105 +105,116 @@
         turbulence_intensities[wind_speeds.index(values[0])][wind_directions.index(values[1])] = values[2]
     return {
         'turbulence_intensity': turbulence_intensities,
         'wind_directions': wind_directions,
         'wind_speeds': wind_speeds
     }
 
-def get_signal_id(parameter_type):
-    signal_map = {
-        'windSpeed': 'WindSpeed_avg',
-        'windDirection': 'WindDirection_avg',
-        # '': 'ActPower_avg',
-        # '': 'AirDensity_avg',
-        # '': 'AirTemperature_avg',
-        # '': 'AirPressure_avg',
-        # '': 'NacDirection_avg',
-        # '': 'OperatingState',
-        'mode': 'OperatingMode',
-    }
-    return signal_map[parameter_type]
 
-def to_instance_measurements(wake_req_file):
-    turbine_parameters = {
-        (t.id, p.type): p.data
-        for t in wake_req_file.Turbines
-        for p in t.Parameters
-        if p.data
+_ReferenceSignalIdLookup = {
+    'windSpeed': 'WindSpeed_avg',
+    'turbulenceStdDev': 'WindSpeed_std',
+    'windSpeedStd': 'WindSpeed_std',
+    'windDirection': 'WindDirection_avg',
+    'airDensity': 'AirDensity_avg',
+    'stability': 'MoninObukhovLength'
+}
+
+
+def turbine_signal_id_lookup(use_wind_speeds):
+    lookup = {
+        'operationMode': 'OperatingMode',
+        'operationState': 'OperatingState'
     }
-    counts = set(len(ps) for ps in turbine_parameters.values())
-    if len(counts) != 1:
-        raise RuntimeError('Different numbers of parameters for different values')
-    count = counts.pop()
-    measurements = []
-    for i in range(count):
-        flow_case_id = 'flow_case_{}'.format(i)
-        for (instance_id, parameter_type), parameters in turbine_parameters.items():
-            next_measurement = {
-                'flow_case_id': flow_case_id,
-                'instance_id': instance_id,
-                'signal_id': get_signal_id(parameter_type),
-                'value': parameters[i]
-            }
-            measurements.append(next_measurement)
-    return measurements
+    if use_wind_speeds:
+        lookup['windSpeed'] = 'WindSpeed_avg'
+    return lookup
+
 
-def to_reference_measurements(wake_req_file, flow_case_count=None):
+def get_timestamp_param(parameters):
+    for param in parameters:
+        if param.type == 'dateTime':
+            return param
+    return None
+
+
+def to_measurements(flow_cases, use_instance_wind_speed_measurements):
     measurements = []
-    flow_case_count = flow_case_count or len(wake_req_file.Reference.Parameters[0].data)
-    for i in range(flow_case_count):
-        for parameter in wake_req_file.Reference.Parameters:
-            measurements.append({
-                'flow_case_id': 'flow_case_{}'.format(i),
-                'instance_id': 'reference',
-                'signal_id': get_signal_id(parameter.type),
-                'value': parameter.data[i]
-            })
+    if (REFERENCE_ID, 'dateTime') in flow_cases.columns:
+        flow_cases = flow_cases.set_index((REFERENCE_ID, 'dateTime'))
+        time_series = True
+    else:
+        time_series = False
+    turbine_signal_ids = turbine_signal_id_lookup(use_instance_wind_speed_measurements)
+    for idx, series in flow_cases.iterrows():
+        if time_series:
+            measurement_template = {'timestamp': idx}
+        else:
+            measurement_template = {'flow_case_id': 'flow_case_{}'.format(idx)}
+        for (instance, param), value in series.items():
+            if instance == REFERENCE_ID:
+                #EMD provides additional signals in some cases, which we can be ignored.
+                if param in _ReferenceSignalIdLookup:
+                    measurements.append({
+                        **measurement_template,
+                        'instance_id': REFERENCE_ID,
+                        'signal_id': _ReferenceSignalIdLookup[param],
+                        'value': value
+                    })
+            else:
+                if param in turbine_signal_ids:  # turbine parameters not in signal ID lookup ignored
+                    measurements.append({
+                        **measurement_template,
+                        'instance_id': instance,
+                        'signal_id': turbine_signal_ids[param],
+                        'value': value
+                    })
     return measurements
 
-def to_associated_wind_speeds(wake_req_file, associated_wind_speed_reference=None):
+
+def to_flow_case_dataframe(wake_req_file):
+    data = pd.DataFrame()
+    for param in wake_req_file.Reference.Parameters:
+        data[(REFERENCE_ID, param.type)] = param.data
+    for turbine in wake_req_file.Turbines:
+        for param in turbine.Parameters:
+            data[(turbine.id, param.type)] = param.data
+    data.columns = pd.MultiIndex.from_tuples(data.columns, names=['Instance', 'Parameter'])
+    return data.transform(pd.to_numeric, errors='ignore')
+
+
+def to_associated_wind_speeds(flow_cases, wake_req_file):
     reference_parameters = {p.type: p.data for p in wake_req_file.Reference.Parameters}
     if 'windSpeed' not in reference_parameters:
         raise ValueError('windSpeed not found in reference data')
     if 'windDirection' not in reference_parameters:
         raise ValueError('windDirection not found in reference data')
-    reference_wind_speeds = sorted(float(ws) for ws in set(reference_parameters['windSpeed']))
-    reference_wind_directions = sorted(float(wd) for wd in set(reference_parameters['windDirection']))
-    wind_speed_count = len(reference_wind_speeds)
-    wind_direction_count = len(reference_wind_directions)
+    wind_speed_data = flow_cases.xs('windSpeed', level='Parameter', axis='columns')
+    ws_ratio_data = pd.DataFrame(index=flow_cases.index)
+    ref_ws = flow_cases[(REFERENCE_ID, 'windSpeed')]
+    ref_wd = flow_cases[(REFERENCE_ID, 'windDirection')]
+    for turbine in wake_req_file.Turbines:
+        ws_ratio_data[turbine.id] = flow_cases[(turbine.id, 'windSpeed')] / ref_ws
+    if wake_req_file.Configuration.is_time_varying:
+        speed_ups = ws_ratio_data.groupby(by=pd.cut(ref_wd, np.linspace(0.0, 360.0, 361, endpoint=True))).median()
+        speed_ups = speed_ups.interpolate().bfill().ffill()
+        interval_idx = pd.IntervalIndex(speed_ups.index)
+        wd_axis = 0.5 * (interval_idx.left + interval_idx.right)
+    else:
+        speed_ups = ws_ratio_data.groupby(by=ref_wd).median()
+        wd_axis = speed_ups.index.values
     wind_speeds = {
-        'reference_id': 'reference',
-        'reference_wind_directions': list(reference_wind_directions),
+        'reference_id': REFERENCE_ID,
+        'reference_wind_directions': wd_axis.tolist(),
         'instances': []
     }
-    if associated_wind_speed_reference is None:
-        wind_speeds['reference_wind_speeds'] = list(reference_wind_speeds)
-    else:
-        associated_wind_speed_index = bisect.bisect_left(reference_wind_speeds,
-                                                         associated_wind_speed_reference,
-                                                         hi=len(reference_wind_speeds)-1)
-
     for turbine in wake_req_file.Turbines:
-        turbine_parameters = {p.type: p.data for p in turbine.Parameters}
-        if 'windSpeed' not in turbine_parameters:
-            raise ValueError('windSpeed not found in turbine data for instance ' + turbine.id)
-        instance_wind_speeds = [[float('nan')] * wind_direction_count for _ in range(wind_speed_count)]
-        for ref_speed, ref_dir, turb_speed in zip(reference_parameters['windSpeed'],
-                                                  reference_parameters['windDirection'],
-                                                  turbine_parameters['windSpeed']):
-            instance_wind_speeds[reference_wind_speeds.index(float(ref_speed))][reference_wind_directions.index(float(ref_dir))] = float(turb_speed)
-
-        if associated_wind_speed_reference is not None:
-            ref_speed = reference_wind_speeds[associated_wind_speed_index]
-            # in this case, wind speed list must be  to 1 because there are no reference wind speeds
-            instance_wind_speeds = [ws / ref_speed for ws in instance_wind_speeds[associated_wind_speed_index]]
-
         wind_speeds['instances'].append({
             'instance_id': str(turbine.id),
-            'instance_wind_speeds': instance_wind_speeds
+            'instance_wind_speeds': speed_ups[turbine.id].values.tolist()
         })
     return wind_speeds
 
 def _md5(fname):
     hash_md5 = hashlib.md5()
     with open(fname, "rb") as f:
         for chunk in iter(lambda: f.read(4096), b""):
@@ -231,15 +253,18 @@
     'turbulenceIntensity': 'turbulence_intensity',
     'wakeSpeedFactor': 'wake_speed_factor',
     'airDensity': 'air_density'
 }
 
 def flow_case_order(result):
     flow_case_id = result['flow_case_id']
-    return int(flow_case_id.replace('flow_case_', ''))
+    if flow_case_id.startswith('flow_case_'):
+        return int(flow_case_id.replace('flow_case_', ''))
+    else:
+        return flow_case_id  # should be ISO-8601 timestamp which naturally sorts
 
 def write_results_csv(results, path):
     header_written = False
     delimiter = ' '
     header = []
     instance_ids = []
     with open(path, 'w') as fp:
```

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/emd/submit.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/submit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from os import path, makedirs
+from os import makedirs
 import sys
 import json
 import random
 import string
 from itertools import groupby
 
 from .wakeRequest import LoadWakeReqFile
@@ -42,39 +42,45 @@
     :type calculation_configuration: dict
 
     :returns: The ID of the simulation
     :rtype: str
     """
     sdk = _DryRun() if dry_run else _sdk
     wake_req = LoadWakeReqFile(file)
+    farm_id = 'test_farm_' + ''.join(random.choice(string.ascii_lowercase+string.digits) for _ in range(5))
     for design_id, wtg_file in to_design_descriptions(wake_req):
-        sdk.upload_turbine_design(design_id, wtg_file)
+        sdk.upload_turbine_design(to_qualified_id(farm_id, design_id), wtg_file)
     sdk.upload_met_mast_design(*to_reference_design(wake_req))
-    farm_id = 'test_farm_' + ''.join(random.choice(string.ascii_lowercase+string.digits) for _ in range(5))
     wind_farm_turbulence = to_wind_farm_turbulence(wake_req.Farm)
-    wind_speeds = to_associated_wind_speeds(wake_req, associated_wind_speed_reference)
+    flow_cases = to_flow_case_dataframe(wake_req)
+    sim_config = calculation_configuration or to_simulation_config(wake_req.CalculationConfigurations)
+    use_instance_wind_speed_measurements =\
+        sim_config.get('measurements', {}).get('wind_conditions_inference') == 'InstanceBased'
+    if use_instance_wind_speed_measurements:
+        assoc_wind_speeds = None
+    else:
+        assoc_wind_speeds = to_associated_wind_speeds(flow_cases, wake_req)
     sdk.upload_asset(farm_id,
-                     to_wind_farm_description(wake_req.Turbines, wake_req.Reference),
-                     associated_wind_speeds=wind_speeds,
+                     to_wind_farm_description(farm_id, wake_req.Turbines, wake_req.Reference),
+                     associated_wind_speeds=assoc_wind_speeds,
                      wind_farm_turbulence=wind_farm_turbulence)
-    keyfunc = lambda m: m['flow_case_id']
-    measurements = sorted(to_reference_measurements(wake_req, flow_case_count), key=keyfunc)
+    keyfunc = lambda m: m.get('flow_case_id') or m['timestamp']
+    measurements = sorted(to_measurements(flow_cases, use_instance_wind_speed_measurements), key=keyfunc)
     measurement_set_ids = []
     pending_measurements = []
     for key, group in groupby(measurements, keyfunc):
         next_measurements = list(group)
         if len(pending_measurements) + len(next_measurements) > max_measurements_per_set:
             measurement_set_ids.append(sdk.upload_measurement_set(farm_id, pending_measurements)['id'])
             pending_measurements = next_measurements
         else:
             pending_measurements += next_measurements
     if pending_measurements:
         measurement_set_ids.append(sdk.upload_measurement_set(farm_id, pending_measurements)['id'])
-    result = sdk.run_simulation(calculation_configuration or to_simulation_config(wake_req.CalculationConfigurations),
-                                measurement_set_ids)
+    result = sdk.run_simulation(sim_config, measurement_set_ids)
     simulation_id = result['id']
     if not path.isdir(simulation_dir):
         makedirs(simulation_dir)
     with open(path.join(simulation_dir, simulation_id + '.json'), 'w') as fp:
         json.dump(get_job_info(wake_req.JobInfo, simulation_id, result['version'], file), fp)
     return simulation_id
```

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/emd/wakeRequest.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,291 +1,325 @@
 # -*- coding: utf-8 -*-
 
 import zipfile
 from xml.dom.minidom import parseString
 
+
 def ReadAttribute(node, key, default=None):
-  if key in node.attributes.keys(): return node.attributes[key].value
-  return default
+    if key in node.attributes.keys():
+        return node.attributes[key].value
+    return default
+
 
 class JobInfo:
-  def __init__(self, node):
-    self.jobId = None
-    self.clientInformationName = None
-    self.clientInformationVersion = None
-    self.clientInformationUserName = None
-    self.coorSysType = None
-    self.coorSys = None
-    self.Parse(node)
-    
-  def Parse(self, node):
-    jobIdNode = node.getElementsByTagName('JobId')[0]
-    self.jobId = jobIdNode.firstChild.nodeValue
-    clientInformationNode = node.getElementsByTagName('ClientInformation')[0]
-    self.clientInformationName = ReadAttribute(clientInformationNode, 'name')
-    self.clientInformationVersion = ReadAttribute(clientInformationNode, 'version')
-    self.clientInformationUserName = ReadAttribute(clientInformationNode, 'userName')
-    coorSysNode = node.getElementsByTagName('CoorSys')[0]
-    self.coorSysType = ReadAttribute(coorSysNode, 'type')
-    self.coorSys = coorSysNode.firstChild.nodeValue
+    def __init__(self, node):
+        self.jobId = None
+        self.clientInformationName = None
+        self.clientInformationVersion = None
+        self.clientInformationUserName = None
+        self.coorSysType = None
+        self.coorSys = None
+        self.Parse(node)
+
+    def Parse(self, node):
+        jobIdNode = node.getElementsByTagName('JobId')[0]
+        self.jobId = jobIdNode.firstChild.nodeValue
+        clientInformationNode = node.getElementsByTagName('ClientInformation')[0]
+        self.clientInformationName = ReadAttribute(clientInformationNode, 'name')
+        self.clientInformationVersion = ReadAttribute(clientInformationNode, 'version')
+        self.clientInformationUserName = ReadAttribute(clientInformationNode, 'userName')
+        coorSysNode = node.getElementsByTagName('CoorSys')[0]
+        self.coorSysType = ReadAttribute(coorSysNode, 'type')
+        self.coorSys = coorSysNode.firstChild.nodeValue
+
 
 class Farm:
-  def __init__(self, request, node):
-    # Public 
-    self.rsfData = None
-    self.turbulencesData = None
-  
-    # Private
-    self.request = request
-    self.scenarioFile = None
-    self.rsfFile = None
-    self.turbulencesFile = None
-    self.Parse(node)
-    
-  def Parse(self, node):
-    try:
-      resourceNode = node.getElementsByTagName('Resource')[0]
-      self.rsfFile = ReadAttribute(resourceNode, 'file')
-    except:
-      self.rsfFile = None
-    scenariosNode = node.getElementsByTagName('Scenarios')[0]
-    self.scenarioFile = ReadAttribute(scenariosNode, 'file')
-    turbulencesNode = node.getElementsByTagName('Turbulences')[0]
-    self.turbulencesFile = ReadAttribute(turbulencesNode, 'file')
-  
-  def ProcessFile(self, filename, fileContent):
-    if filename == self.rsfFile:
-      self.rsfData = fileContent
-    if filename == self.turbulencesFile:
-      self.turbulencesData = fileContent
+    def __init__(self, request, node):
+        # Public
+        self.rsfData = None
+        self.turbulencesData = None
+
+        # Private
+        self.request = request
+        self.scenarioFile = None
+        self.rsfFile = None
+        self.turbulencesFile = None
+        self.Parse(node)
+
+    def Parse(self, node):
+        try:
+            resourceNode = node.getElementsByTagName('Resource')[0]
+            self.rsfFile = ReadAttribute(resourceNode, 'file')
+        except:
+            self.rsfFile = None
+        scenariosNode = node.getElementsByTagName('Scenarios')[0]
+        self.scenarioFile = ReadAttribute(scenariosNode, 'file')
+        turbulence_nodes = node.getElementsByTagName('Turbulences')
+        if turbulence_nodes:
+            turbulencesNode = turbulence_nodes[0]
+            self.turbulencesFile = ReadAttribute(turbulencesNode, 'file')
+        else:
+            self.turbulencesFile = None
+
+    def ProcessFile(self, filename, fileContent):
+        if filename == self.rsfFile:
+            self.rsfData = fileContent
+        if filename == self.turbulencesFile:
+            self.turbulencesData = fileContent
+
 
 class Mode:
-  def __init__(self, turbineType, node):
-    # Public
-    self.id = None
-    self.ctCurve = None
-    self.airDensity = None
-    self.stationaryThrustCoefficient = None
-    
-    # Private
-    self.turbineType = turbineType
-    self.ctFile = None
-    self.Parse(node)
-    
-  def Parse(self, node):
-    self.id = ReadAttribute(node, 'id')
-    self.airDensity = float(ReadAttribute(node, 'airDensity', '1.225'))
-    self.stationaryThrustCoefficient = float(ReadAttribute(node, 'stationaryThrustCoefficient', '0.05'))
-    self.ctFile = ReadAttribute(node, 'ctFile')
-    self.ctCurve = []
-    
-  def ProcessFile(self, filename, fileContent):
-    if filename == self.ctFile:
-      lines = fileContent.split('\n')
-      headerLine = True
-      for line in lines:
-        line = line.strip()
-        if headerLine:
-          headerLine = False
-        else:
-          elements = line.split(' ')
-          if len(elements) == 2:
-            self.ctCurve.append([float(x) for x in elements])
+    def __init__(self, turbineType, node):
+        # Public
+        self.id = None
+        self.ctCurve = None
+        self.airDensity = None
+        self.stationaryThrustCoefficient = None
+
+        # Private
+        self.turbineType = turbineType
+        self.ctFile = None
+        self.Parse(node)
+
+    def Parse(self, node):
+        self.id = ReadAttribute(node, 'id')
+        self.airDensity = float(ReadAttribute(node, 'airDensity', '1.225'))
+        self.stationaryThrustCoefficient = float(ReadAttribute(node, 'stationaryThrustCoefficient', '0.05'))
+        self.ctFile = ReadAttribute(node, 'ctFile')
+        self.ctCurve = []
+
+    def ProcessFile(self, filename, fileContent):
+        if filename == self.ctFile:
+            lines = fileContent.split('\n')
+            headerLine = True
+            for line in lines:
+                line = line.strip()
+                if headerLine:
+                    headerLine = False
+                else:
+                    elements = line.split(' ')
+                    if len(elements) == 2:
+                        self.ctCurve.append([float(x) for x in elements])
+
 
 class TurbineType:
-  def __init__(self, request, node):
-    # Public
-    self.id = None
-    self.HubHeight = None
-    self.RotorDiameter = None
-    self.CutIn = None
-    self.CutOut = None
-    self.Modes = {}
-    
-    # Private
-    self.defaultMode = None
-    self.request = request
-    self.Parse(node)
-    
-  def GetCTCurve(self, modeId=None):
-    if modeId is None:
-      modeId = self.defaultMode
-    return self.Modes[modeId].ctCurve    
-    
-  def Parse(self, node):
-    self.id = ReadAttribute(node, 'id')
-    hubHeightNode = node.getElementsByTagName('HubHeight')[0]
-    self.HubHeight = float(hubHeightNode.firstChild.nodeValue)
-    rotorDiameterNode = node.getElementsByTagName('RotorDiameter')[0]
-    self.RotorDiameter = float(rotorDiameterNode.firstChild.nodeValue)
-    cutInNode = node.getElementsByTagName('CutIn')[0]
-    self.CutIn = float(cutInNode.firstChild.nodeValue)
-    cutOutNode = node.getElementsByTagName('CutOut')[0]
-    self.CutOut = float(cutOutNode.firstChild.nodeValue)
-    modesNode = node.getElementsByTagName('Modes')[0]
-    self.defaultMode = ReadAttribute(modesNode, 'defaultMode')
-    for modeNode in modesNode.getElementsByTagName('Mode'):
-      mode = Mode(self, modeNode)
-      self.Modes[mode.id] = mode
-
-  def ProcessFile(self, filename, fileContent):
-    for modeId, mode in self.Modes.items():
-      mode.ProcessFile(filename, fileContent)
+    def __init__(self, request, node):
+        # Public
+        self.id = None
+        self.HubHeight = None
+        self.RotorDiameter = None
+        self.CutIn = None
+        self.CutOut = None
+        self.Modes = {}
+
+        # Private
+        self.defaultMode = None
+        self.request = request
+        self.Parse(node)
+
+    def GetCTCurve(self, modeId=None):
+        if modeId is None:
+            modeId = self.defaultMode
+        return self.Modes[modeId].ctCurve
+
+    def Parse(self, node):
+        self.id = ReadAttribute(node, 'id')
+        hubHeightNode = node.getElementsByTagName('HubHeight')[0]
+        self.HubHeight = float(hubHeightNode.firstChild.nodeValue)
+        rotorDiameterNode = node.getElementsByTagName('RotorDiameter')[0]
+        self.RotorDiameter = float(rotorDiameterNode.firstChild.nodeValue)
+        cutInNode = node.getElementsByTagName('CutIn')[0]
+        self.CutIn = float(cutInNode.firstChild.nodeValue)
+        cutOutNode = node.getElementsByTagName('CutOut')[0]
+        self.CutOut = float(cutOutNode.firstChild.nodeValue)
+        modesNode = node.getElementsByTagName('Modes')[0]
+        self.defaultMode = ReadAttribute(modesNode, 'defaultMode')
+        for modeNode in modesNode.getElementsByTagName('Mode'):
+            mode = Mode(self, modeNode)
+            self.Modes[mode.id] = mode
+
+    def ProcessFile(self, filename, fileContent):
+        for modeId, mode in self.Modes.items():
+            mode.ProcessFile(filename, fileContent)
+
 
 class Parameter:
-  def __init__(self, request, node):
-    # Public
-    self.type = None
-    self.data = []
-    
-    # Private
-    self.col = None
-    self.index = None
-    self.Parse(node)
-    
-  def Parse(self, node):
-    self.col = ReadAttribute(node, 'col')
-    self.type = ReadAttribute(node, 'type')
-
-  def ProcessHeader(self, headerElements):
-    self.index = headerElements.index(self.col)
-    
-  def ProcessLine(self, lineElements):
-    if self.index < len(lineElements):
-      self.data.append(lineElements[self.index])
+    def __init__(self, request, node):
+        # Public
+        self.type = None
+        self.data = []
+
+        # Private
+        self.col = None
+        self.index = None
+        self.Parse(node)
+
+    def Parse(self, node):
+        self.col = ReadAttribute(node, 'col')
+        self.type = ReadAttribute(node, 'type')
+
+    def ProcessHeader(self, headerElements):
+        self.index = headerElements.index(self.col)
+
+    def ProcessLine(self, lineElements):
+        if self.index < len(lineElements):
+            self.data.append(lineElements[self.index])
+
 
 class Instance:
-  def __init__(self, request, node):
-    self.id = None
-    self.Parameters = []
-    self.x = None
-    self.y = None
-    self.z = None
-    
-    # Private
-    self.request = request
-    self.scenarioFile = request.Farm.scenarioFile
-    self.Parse(node)
-
-  def Parse(self, node):
-    self.id = ReadAttribute(node, 'id')
-    self.x = float(ReadAttribute(node, 'x'))
-    self.y = float(ReadAttribute(node, 'y'))
-    self.z = float(ReadAttribute(node, 'z'))
-    for parameterNode in node.getElementsByTagName('Parameter'):
-      self.Parameters.append(Parameter(self, parameterNode))
-      
-  def ProcessFile(self, filename, fileContent):
-    if filename == self.scenarioFile:
-      lines = fileContent.split('\n')
-      headerLine = True
-      for line in lines:
-        line = line.strip()
-        if line == '':
-          continue
-        elements = line.split(' ')
-        if headerLine:
-          for parameter in self.Parameters:
-            parameter.ProcessHeader(elements)
-          headerLine = False
-        else:
-          for parameter in self.Parameters:
-            parameter.ProcessLine(elements)
+    def __init__(self, request, node):
+        self.id = None
+        self.Parameters = []
+        self.x = None
+        self.y = None
+        self.z = None
+
+        # Private
+        self.request = request
+        self.scenarioFile = request.Farm.scenarioFile
+        self.Parse(node)
+
+    def Parse(self, node):
+        self.id = ReadAttribute(node, 'id')
+        self.x = float(ReadAttribute(node, 'x'))
+        self.y = float(ReadAttribute(node, 'y'))
+        self.z = float(ReadAttribute(node, 'z'))
+        for parameterNode in node.getElementsByTagName('Parameter'):
+            self.Parameters.append(Parameter(self, parameterNode))
+
+    def ProcessFile(self, filename, fileContent):
+        if filename == self.scenarioFile:
+            lines = fileContent.split('\n')
+            headerLine = True
+            for line in lines:
+                line = line.strip()
+                if line == '':
+                    continue
+                elements = line.split(' ')
+                if headerLine:
+                    for parameter in self.Parameters:
+                        parameter.ProcessHeader(elements)
+                    headerLine = False
+                else:
+                    for parameter in self.Parameters:
+                        parameter.ProcessLine(elements)
 
 
 class Turbine(Instance):
-  def __init__(self, request, node):
-    self.Type = None
-    super().__init__(request, node)
-    
-  def GetCTCurve(self, modeId=None):
-    return self.Type.GetCTCurve(modeId)
-    
-  def Parse(self, node):
-    super().Parse(node)
-    
-    typeId = ReadAttribute(node, 'type')
-    self.Type = self.request.TurbineTypes[typeId]
+    def __init__(self, request, node):
+        self.Type = None
+        super().__init__(request, node)
+
+    def GetCTCurve(self, modeId=None):
+        return self.Type.GetCTCurve(modeId)
+
+    def Parse(self, node):
+        super().Parse(node)
+
+        typeId = ReadAttribute(node, 'type')
+        self.Type = self.request.TurbineTypes[typeId]
+
 
 class Reference(Instance):
-  def __init__(self, request, node):
-    self.height = None
-    super().__init__(request, node)
-
-  def Parse(self, node):
-    super().Parse(node)
-    self.height = float(ReadAttribute(node, 'height'))
+    def __init__(self, request, node):
+        self.height = None
+        super().__init__(request, node)
+
+    def Parse(self, node):
+        super().Parse(node)
+        self.height = float(ReadAttribute(node, 'height'))
+
 
 class CalculationConfiguration:
-  def __init__(self, name, filename):
-    self.name = name
-    self.contents = None
-    self.filename = filename
-  
-  def ProcessFile(self, filename, fileContents):
-    if filename == self.filename:
-      self.contents = fileContents
+    def __init__(self, name, filename):
+        self.name = name
+        self.contents = None
+        self.filename = filename
+
+    def ProcessFile(self, filename, fileContents):
+        if filename == self.filename:
+            self.contents = fileContents
+
+
+class Configuration:
+    def __init__(self):
+        self._settings = {}
+
+    def Parse(self, node):
+        for setting_node in node.getElementsByTagName('Setting'):
+            self._settings[ReadAttribute(setting_node, 'name')] = ReadAttribute(setting_node, 'value')
+
+    @property
+    def is_time_varying(self):
+        return self._settings.get('ScenariosMode') == 'TimeVarying'
+
 
 class WakeReqFile():
-  def __init__(self):
-      self.path = ''
-      self.xmlDom = None
-      self.JobInfo = None
-      self.Farm = None
-      self.CalculationConfigurations = []
-      self.TurbineTypes = {}
-      self.Turbines = []
-      self.Reference = None
-              
-  def Load(self,path):
-    self.path = path
-    with zipfile.ZipFile(self.path, "r") as z:
-      xmlData = z.read('WakeRequest.xml')
-      self.xmlDom = parseString(xmlData)
-      self.Parse(self.xmlDom)
-      for name in z.namelist():
-        fileContent = z.read(name).decode('utf8')
-        self.Reference.ProcessFile(name, fileContent)
-        for turbine in self.Turbines:
-          turbine.ProcessFile(name, fileContent)
-        for turbineId, turbineType in self.TurbineTypes.items():
-          turbineType.ProcessFile(name, fileContent)
-        self.Farm.ProcessFile(name, fileContent)
-        for calculation_configuration in self.CalculationConfigurations:
-          calculation_configuration.ProcessFile(name, fileContent)
-
-  def Parse(self, zipFile):
-    mainNode = self.xmlDom.getElementsByTagName('WakeRequest')[0]
-    
-    self.JobInfo = JobInfo(mainNode.getElementsByTagName('JobInfo')[0])
-    self.Farm = Farm(self, mainNode.getElementsByTagName('Farm')[0])
-
-    referenceNode = mainNode.getElementsByTagName('Reference')[0]
-    self.Reference = Reference(self, referenceNode)
-
-    turbineTypesNode = mainNode.getElementsByTagName('TurbineTypes')[0]
-    for turbineTypeNode in turbineTypesNode.getElementsByTagName('TurbineType'):
-      turbineType = TurbineType(self, turbineTypeNode)
-      self.TurbineTypes[turbineType.id] = turbineType
-
-    turbinesNode = mainNode.getElementsByTagName('Turbines')[0]
-    for turbineNode in turbinesNode.getElementsByTagName('Turbine'):
-      self.Turbines.append(Turbine(self, turbineNode))
-    
-    calculationConfigurationsNode = mainNode.getElementsByTagName('CalculationConfigurations')[0]
-    for calculationConfigurationNode in calculationConfigurationsNode.getElementsByTagName('CalculationConfiguration'):
-      self.CalculationConfigurations.append(
-        CalculationConfiguration(
-            ReadAttribute(calculationConfigurationNode, 'model'),
-            calculationConfigurationNode.firstChild.nodeValue
-          )
-        )
-    
+    def __init__(self):
+        self.path = ''
+        self.xmlDom = None
+        self.JobInfo = None
+        self.Farm = None
+        self.CalculationConfigurations = []
+        self.Configuration = {}
+        self.TurbineTypes = {}
+        self.Turbines = []
+        self.Reference = None
+
+    def Load(self,path):
+        self.path = path
+        with zipfile.ZipFile(self.path, "r") as z:
+            xmlData = z.read('WakeRequest.xml')
+            self.xmlDom = parseString(xmlData)
+            self.Parse(self.xmlDom)
+            for name in z.namelist():
+                fileContent = z.read(name).decode('utf8')
+                self.Reference.ProcessFile(name, fileContent)
+                for turbine in self.Turbines:
+                    turbine.ProcessFile(name, fileContent)
+                for turbineId, turbineType in self.TurbineTypes.items():
+                    turbineType.ProcessFile(name, fileContent)
+                self.Farm.ProcessFile(name, fileContent)
+                for calculation_configuration in self.CalculationConfigurations:
+                    calculation_configuration.ProcessFile(name, fileContent)
+
+    def Parse(self, zipFile):
+        mainNode = self.xmlDom.getElementsByTagName('WakeRequest')[0]
+
+        self.JobInfo = JobInfo(mainNode.getElementsByTagName('JobInfo')[0])
+        self.Farm = Farm(self, mainNode.getElementsByTagName('Farm')[0])
+
+        referenceNode = mainNode.getElementsByTagName('Reference')[0]
+        self.Reference = Reference(self, referenceNode)
+
+        turbineTypesNode = mainNode.getElementsByTagName('TurbineTypes')[0]
+        for turbineTypeNode in turbineTypesNode.getElementsByTagName('TurbineType'):
+            turbineType = TurbineType(self, turbineTypeNode)
+            self.TurbineTypes[turbineType.id] = turbineType
+
+        turbinesNode = mainNode.getElementsByTagName('Turbines')[0]
+        for turbineNode in turbinesNode.getElementsByTagName('Turbine'):
+            self.Turbines.append(Turbine(self, turbineNode))
+
+        calculationConfigurationsNode = mainNode.getElementsByTagName('CalculationConfigurations')[0]
+        for calculationConfigurationNode in calculationConfigurationsNode.getElementsByTagName('CalculationConfiguration'):
+            self.CalculationConfigurations.append(
+                CalculationConfiguration(
+                    ReadAttribute(calculationConfigurationNode, 'model'),
+                    calculationConfigurationNode.firstChild.nodeValue
+                )
+            )
+
+        self.Configuration = Configuration()
+        config_nodes = mainNode.getElementsByTagName('Configuration')
+        if len(config_nodes) > 0:
+            self.Configuration.Parse(mainNode.getElementsByTagName('Configuration')[0])
+
 
 def LoadWakeReqFile(path):
-  retVal = WakeReqFile()
-  retVal.Load(path)        
-  return retVal        
+    retVal = WakeReqFile()
+    retVal.Load(path)
+    return retVal
 
 if __name__ == '__main__':
     request = LoadWakeReqFile('..\\xsd\\examples\\request.wakeReq')
```

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/emd/wakeResult.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/emd/wakeResult.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/flow_plane_plots.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/flow_plane_plots.py`

 * *Files identical despite different names*

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/sdk.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/sdk.py`

 * *Files 3% similar despite different names*

```diff
@@ -134,34 +134,37 @@
     logger.debug('Getting design %s', design_id)
     endpoint = _api_base_url + '/designs/' + design_id + '/design'
     response = do_request(requests.get, endpoint, tries, headers=_standard_headers())
     _validate_response(response, 200, 'get design', design_id)
     return response.json() if json else response.text
 
 
-def upload_asset(asset_id, wind_farm_def, wind_resource_grid_file=None, wind_farm_turbulence=None, associated_wind_speeds=None, tries=5):
+def upload_asset(asset_id, wind_farm_def, wind_resource_grid_file=None, wind_farm_turbulence=None, associated_wind_speeds=None, regional_roughness=None, tries=5):
     """
     Upload a wind farm definition, overwriting it if a matching asset ID already existed.
 
     :param asset_id: ID of the asset (wind farm).
     :param wind_farm_def: Wind farm definition in a dict object according to wind farm definition format.
     :param wind_resource_grid_file: (optional) The contents of a WASP format .wrg or .rsf file as a string.
     :param wind_farm_turbulence: (optional) Information for the default wind farm turbulence. See docs
     :param associated_wind_speeds: (optional) Information about the wind speeds associated to each instance. Determines relative wind speeds across the farm. See docs
+    :param regional_roughness: (optional) Regional roughness length.
     :param tries: Number of times the HTTP request should be tried in case of timeout or 'too many requests'
     """
     logger.debug('Uploading asset %s', asset_id)
     endpoint = _api_base_url + '/assets/' + asset_id
     body = {'wind_farm_description': wind_farm_def}
     if wind_resource_grid_file:
         body['wind_resource_grid_file'] = wind_resource_grid_file
     if wind_farm_turbulence:
         body['wind_farm_turbulence'] = wind_farm_turbulence
     if associated_wind_speeds:
         body['associated_wind_speeds'] = associated_wind_speeds
+    if regional_roughness:
+        body['regional_roughness'] = regional_roughness
     response = do_request(
         requests.put,
         endpoint,
         tries,
         data=gzip.compress(to_json(body).encode('utf8')),
         headers={**_standard_headers(), 'Content-Type': 'application/json', 'Content-Encoding': 'gzip'}
     )
@@ -253,23 +256,42 @@
     """
     logger.debug('Retrieving information for simulation %s', simulation_id)
     endpoint = _api_base_url + '/simulations/' + simulation_id
     response = do_request(requests.get, endpoint, tries, headers=_standard_headers())
     _validate_response(response, 200, 'get simulation {}'.format(simulation_id))
     return response.json()
 
+def get_simulations(submitted_from=None, submitted_to=None, tries=5):
+    """
+    Get information about simulations, that have been or are running on this environment.
+
+    :param submitted_from: If provided, this is the start timestamp of the period.
+    :param submitted_to: If provided, this is the end timestamp of the period.
+    :param tries: Number of times the HTTP request should be tried in case of timeout or 'too many requests'
+    """
+    logger.debug('Retrieving information for simulations')
+    params = "?"
+    if submitted_from:
+        params += "submitted_from=" + submitted_from
+    if submitted_to:
+        params += "&submitted_to=" + submitted_to
+    endpoint = _api_base_url + '/simulations' + params
+    response = do_request(requests.get, endpoint, tries, headers=_standard_headers())
+    _validate_response(response, 200, 'get simulations')
+    return response.json()
+
 
 def get_results(simulation_id, tries=5, format='json', property=None, batch_limit=1000):
     """
     Get results of a simulation. Usually it is advisable to not call this until the result_count has been checked by calling get_simulation_info.
 
     :param simulation_id: Identifier of the simulation (as returned by run_simulation).
     :param tries: Number of times the HTTP request should be tried in case of timeout or 'too many requests'
     :param format: Format of the results. One of [json|csv]. If csv, the property can be specified. csv format contains instances (columns) against flow cases/timestamps (rows).
-    :param property: If format is csv, the property to retrieve. One of [power|unwaked_power|rotor_wind_speed|wake_speed_factor|air_density|turbulence_intensity]. Defaults to 'power'.
+    :param property: If format is csv, the property to retrieve. One of [power|unwaked_power|rotor_wind_speed|hub_wind_speed|wake_speed_factor|blockage_speed_factor|air_density|turbulence_intensity]. Defaults to 'power'.
     """
     if format not in ['json', 'csv']:
         raise ValueError('Unsupported format: ' + format)
     logger.debug('Retrieving results for simulation %s', simulation_id)
     results_endpoint = 'results' if format == 'json' else 'results-csv'
     endpoint = _api_base_url + '/' + results_endpoint + '?simulation_id=' + simulation_id + ('' if property is None else '&property=' + property)
     headers = {**_standard_headers(), 'Accept-Encoding': 'gzip'}
@@ -470,14 +492,31 @@
         written = _download_part(written)
         if written == -1:
             break
         attempts += 1
     else:
         raise WakeBlasterError('Could not download flow plane for simulation {}'.format(simulation_id))
 
+def download_surfer_grid(simulation_id, height, target_path):
+    """
+    Get a surfer grid
+    :param: simulation_id
+    :param: height
+    :param: target_path
+    :return: string, containing a surfer grid file
+    :rtype: str
+    """
+    response = do_request(requests.get, _api_base_url + '/flow-plane/' + simulation_id + "?format=surfer&height=" + str(height), headers={**_standard_headers(), 'Accept-Encoding': 'gzip'})
+    _validate_response(response, 200, 'surfer grid for flow plane log')
+    try:
+        with open(target_path, "w") as fp:
+            fp.write(response.text)
+    except OSError as ex:
+        raise WakeBlasterError('Could not write downloaded surfer grid to {}: {}'.format(target_path, ex))
+
 def get_version():
     """
     Get WakeBlaster version
     :return: string of the WakeBlaster version
     :rtype: str
     """
     response = requests.get(_api_base_url, headers={**_standard_headers(), 'Accept-Encoding': 'gzip'})
```

### Comparing `wakeblaster-sdk-2.4.4/wakeblastersdk/__init__.py` & `wakeblaster-sdk-2.6.4/wakeblastersdk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from .sdk import (
     get_asset,
     get_design,
     get_error_messages,
     get_results,
     get_simulation_info,
+    get_simulations,
     get_version,
     get_wind_farm_description,
     retrieve_results,
     run_simulation,
     set_api_url_and_key,
     upload_asset,
     upload_measurement_set,
     upload_met_mast_design,
     upload_turbine_design,
     WakeBlasterError,
     csv_to_dict,
     download_flow_plane,
+    download_surfer_grid,
     remaining_flow_cases
 )
 
 from .flow_plane_plots import plot_flow_plane_xy, plot_flow_plane_xz, plot_flow_plane_yz
```

### Comparing `wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/PKG-INFO` & `wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: wakeblaster-sdk
-Version: 2.4.4
+Version: 2.6.4
 Summary: The WakeBlaster SDK
 Home-page: http://www.wakeblaster.net
 Author: ProPlanEn Ltd.
 Author-email: wakeblaster@proplanen.net
 License: UNKNOWN
 Description: # WakeBlaster SDK
```

### Comparing `wakeblaster-sdk-2.4.4/wakeblaster_sdk.egg-info/SOURCES.txt` & `wakeblaster-sdk-2.6.4/wakeblaster_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

