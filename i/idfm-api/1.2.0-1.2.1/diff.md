# Comparing `tmp/idfm_api-1.2.0.tar.gz` & `tmp/idfm_api-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idfm_api-1.2.0.tar", last modified: Tue Jun 20 17:19:08 2023, max compression
+gzip compressed data, was "idfm_api-1.2.1.tar", last modified: Tue Jun 20 17:46:38 2023, max compression
```

## Comparing `idfm_api-1.2.0.tar` & `idfm_api-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:19:08.637329 idfm_api-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 17:17:52.000000 idfm_api-1.2.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 17:19:08.637329 idfm_api-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-20 17:17:52.000000 idfm_api-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:19:08.625329 idfm_api-1.2.0/idfm_api/
--rw-r--r--   0 runner    (1001) docker     (123)     8033 2023-06-20 17:17:52.000000 idfm_api-1.2.0/idfm_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-20 17:17:52.000000 idfm_api-1.2.0/idfm_api/attribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    70382 2023-06-20 17:18:54.000000 idfm_api-1.2.0/idfm_api/lines.json
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-20 17:17:52.000000 idfm_api-1.2.0/idfm_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123) 11821534 2023-06-20 17:18:55.000000 idfm_api-1.2.0/idfm_api/stops.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:19:08.637329 idfm_api-1.2.0/idfm_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 17:19:08.000000 idfm_api-1.2.0/idfm_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:19:08.637329 idfm_api-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-20 17:17:52.000000 idfm_api-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:46:38.188803 idfm_api-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 17:45:26.000000 idfm_api-1.2.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 17:46:38.188803 idfm_api-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-06-20 17:45:26.000000 idfm_api-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:46:38.176803 idfm_api-1.2.1/idfm_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8233 2023-06-20 17:45:26.000000 idfm_api-1.2.1/idfm_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-20 17:45:26.000000 idfm_api-1.2.1/idfm_api/attribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70382 2023-06-20 17:46:23.000000 idfm_api-1.2.1/idfm_api/lines.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-06-20 17:45:26.000000 idfm_api-1.2.1/idfm_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123) 11821534 2023-06-20 17:46:24.000000 idfm_api-1.2.1/idfm_api/stops.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 17:46:38.188803 idfm_api-1.2.1/idfm_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-20 17:46:38.000000 idfm_api-1.2.1/idfm_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-20 17:46:38.000000 idfm_api-1.2.1/idfm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 17:46:38.000000 idfm_api-1.2.1/idfm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 17:46:38.000000 idfm_api-1.2.1/idfm_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-20 17:46:38.000000 idfm_api-1.2.1/idfm_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 17:46:38.188803 idfm_api-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-06-20 17:45:27.000000 idfm_api-1.2.1/setup.py
```

### Comparing `idfm_api-1.2.0/LICENCE` & `idfm_api-1.2.1/LICENCE`

 * *Files identical despite different names*

### Comparing `idfm_api-1.2.0/PKG-INFO` & `idfm_api-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idfm_api
-Version: 1.2.0
+Version: 1.2.1
 Summary: API for Ile de france mobilite
 Home-page: https://github.com/droso-hass/idfm-api
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://idfm-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/droso-hass/idfm-api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `idfm_api-1.2.0/idfm_api/__init__.py` & `idfm_api-1.2.1/idfm_api/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             line_id: A string indicating id of a line (if not specified, all schedules for this stop/direction will be returned regardless of the line)
         Returns:
             A list of TrafficData objects
         """
 
         # for backward compatibility where only the stoppoint id is specified
         if stop_id[0:4] != "STIF":
-            stop_id = f"STIF:StopPoint:Q:{stop_id}:"
+            stop_id = f"STIF:StopPoint:Q:{stop_id.split(':')[-1]}:"
         
         line = f"&LineRef=STIF:Line::{line_id}:" if line_id is not None else ""
         request = f"https://prim.iledefrance-mobilites.fr/marketplace/stop-monitoring?MonitoringRef={stop_id}"
         try:
             response = await self.__request(request+line)
         except UnknownIdentifierException:
             # if the MonitoringRef/LineRef couple does not exists, fallback to use only the MonitoringRef
@@ -120,34 +120,35 @@
     async def get_destinations(self, stop_id: str, direction_name: Optional[str] = None, line_id: Optional[str] = None) -> List[str]:
         """
         Returns the available destinations for a specified line
 
         Args:
             stop_id: A string indicating the id of the depart stop area
             direction_name: The direction of a train
-            line_id: A string indicating id of a line (if not specified, all schedules for this stop/direction will be returned regardless of the line)
+            line_id: A string indicating id of a line (if not specified, all destinations for this stop will be returned regardless of the line)
         Returns:
             A list of string representing the stations names
         """
         ret = set()
         for i in await self.get_traffic(stop_id, direction_name=direction_name, line_id=line_id):
             ret.add(i.destination_name)
         return list(ret)
 
-    async def get_directions(self, stop_id: str) -> List[str]:
+    async def get_directions(self, stop_id: str, line_id: Optional[str] = None) -> List[str]:
         """
         Returns the available directions for a specified line
 
         Args:
             stop_id: A string indicating the id of the depart stop area
+            line_id: A string indicating id of a line (if not specified, all directions for this stop will be returned regardless of the line)
         Returns:
             A list of string representing the stations names
         """
         ret = set()
-        for i in await self.get_traffic(stop_id):
+        for i in await self.get_traffic(stop_id, line_id=line_id):
             ret.add(i.direction)
         return list(ret)
 
     async def get_infos(self, line_id: str) -> List[InfoData]:
         """
         Returns the traffic informations (usually the current/planned perturbations) for the specified line
```

### Comparing `idfm_api-1.2.0/idfm_api/attribution.py` & `idfm_api-1.2.1/idfm_api/attribution.py`

 * *Files identical despite different names*

### Comparing `idfm_api-1.2.0/idfm_api/lines.json` & `idfm_api-1.2.1/idfm_api/lines.json`

 * *Files identical despite different names*

### Comparing `idfm_api-1.2.0/idfm_api/models.py` & `idfm_api-1.2.1/idfm_api/models.py`

 * *Files identical despite different names*

### Comparing `idfm_api-1.2.0/idfm_api/stops.json` & `idfm_api-1.2.1/idfm_api/stops.json`

 * *Files identical despite different names*

### Comparing `idfm_api-1.2.0/idfm_api.egg-info/PKG-INFO` & `idfm_api-1.2.1/idfm_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idfm-api
-Version: 1.2.0
+Version: 1.2.1
 Summary: API for Ile de france mobilite
 Home-page: https://github.com/droso-hass/idfm-api
 Author: drosocode
 License: MIT
 Project-URL: Documentation, https://idfm-api.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/droso-hass/idfm-api
 Classifier: Programming Language :: Python :: 3
```

### Comparing `idfm_api-1.2.0/setup.py` & `idfm_api-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 setup(
     name='idfm_api',
     packages=find_packages(include=['idfm_api']),
     package_data={
         'idfm_api': ['lines.json', 'stops.json'],
     },
-    version='1.2.0',
+    version='1.2.1',
     author='drosocode',
     license='MIT',
     description='API for Ile de france mobilite',
     url="https://github.com/droso-hass/idfm-api",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
```

