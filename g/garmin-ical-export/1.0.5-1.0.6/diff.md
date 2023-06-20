# Comparing `tmp/garmin-ical-export-1.0.5.tar.gz` & `tmp/garmin-ical-export-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "garmin-ical-export-1.0.5.tar", last modified: Wed Nov 16 14:40:27 2022, max compression
+gzip compressed data, was "garmin-ical-export-1.0.6.tar", last modified: Tue Jun 20 13:08:19 2023, max compression
```

## Comparing `garmin-ical-export-1.0.5.tar` & `garmin-ical-export-1.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 14:40:27.720102 garmin-ical-export-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2576 2022-11-16 14:40:27.720102 garmin-ical-export-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 14:40:27.720102 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2576 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      500 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       65 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       33 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-16 14:40:27.000000 garmin-ical-export-1.0.5/garmin_ical_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 14:40:27.720102 garmin-ical-export-1.0.5/garminicalexport/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/garminicalexport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5895 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/garminicalexport/activities.py
--rw-r--r--   0 runner    (1001) docker     (122)     1755 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/garminicalexport/cmd.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/garminicalexport/data_types.py
--rw-r--r--   0 runner    (1001) docker     (122)     1464 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/garminicalexport/format_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2495 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/garminicalexport/garmin_api.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-16 14:40:27.720102 garmin-ical-export-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      816 2022-11-16 14:40:15.000000 garmin-ical-export-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:08:19.553082 garmin-ical-export-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-20 13:08:19.553082 garmin-ical-export-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:08:19.553082 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-20 13:08:19.000000 garmin-ical-export-1.0.6/garmin_ical_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:08:19.553082 garmin-ical-export-1.0.6/garminicalexport/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/garminicalexport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/garminicalexport/activities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/garminicalexport/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/garminicalexport/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/garminicalexport/format_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/garminicalexport/garmin_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:08:19.553082 garmin-ical-export-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-20 13:08:10.000000 garmin-ical-export-1.0.6/setup.py
```

### Comparing `garmin-ical-export-1.0.5/LICENSE` & `garmin-ical-export-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `garmin-ical-export-1.0.5/PKG-INFO` & `garmin-ical-export-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-ical-export
-Version: 1.0.5
+Version: 1.0.6
 Summary: Export Garmin Connect activities to iCalendar file
 Home-page: https://github.com/jirikuchta/garmin-ical-export
 Author: Jiri Kuchta
 Author-email: jiri.kuchta@email.cz
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `garmin-ical-export-1.0.5/README.md` & `garmin-ical-export-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `garmin-ical-export-1.0.5/garmin_ical_export.egg-info/PKG-INFO` & `garmin-ical-export-1.0.6/garmin_ical_export.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: garmin-ical-export
-Version: 1.0.5
+Version: 1.0.6
 Summary: Export Garmin Connect activities to iCalendar file
 Home-page: https://github.com/jirikuchta/garmin-ical-export
 Author: Jiri Kuchta
 Author-email: jiri.kuchta@email.cz
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `garmin-ical-export-1.0.5/garminicalexport/__init__.py` & `garmin-ical-export-1.0.6/garminicalexport/__init__.py`

 * *Files identical despite different names*

### Comparing `garmin-ical-export-1.0.5/garminicalexport/activities.py` & `garmin-ical-export-1.0.6/garminicalexport/activities.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,17 +77,16 @@
             self._data["startTimeLocal"], "%Y-%m-%d %H:%M:%S")
         if self._tzinfo:
             start_time = start_time.replace(tzinfo=self._tzinfo)
         return start_time
 
     @property
     def ical_dtend(self) -> datetime:
-        duration = 0
-        if self._data["duration"] is not None:
-            duration = round(self._data["duration"])
+        duration = self._data.get("elapsedDuration") \
+            or self._data.get("duration") or 0
         return self.ical_dtstart + timedelta(seconds=duration)
 
 
 class RunningActivity(Activity):
 
     @property
     def average_speed(self):
```

### Comparing `garmin-ical-export-1.0.5/garminicalexport/cmd.py` & `garmin-ical-export-1.0.6/garminicalexport/cmd.py`

 * *Files identical despite different names*

### Comparing `garmin-ical-export-1.0.5/garminicalexport/data_types.py` & `garmin-ical-export-1.0.6/garminicalexport/data_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     activityId: int
     activityName: Optional[str]
     activityType: ActivityTypeData
     averageSpeed: Optional[float]  # m/s
     description: Optional[str]
     distance: Optional[float]  # metres
     duration: Optional[float]  # seconds
+    elapsedDuration: Optional[float]  # seconds
     ownerId: int
     startTimeLocal: str
     timeZoneId: int
 
 
 class TimezoneData(TypedDict):
     unitId: int
```

### Comparing `garmin-ical-export-1.0.5/garminicalexport/format_utils.py` & `garmin-ical-export-1.0.6/garminicalexport/format_utils.py`

 * *Files identical despite different names*

### Comparing `garmin-ical-export-1.0.5/garminicalexport/garmin_api.py` & `garmin-ical-export-1.0.6/garminicalexport/garmin_api.py`

 * *Files identical despite different names*

### Comparing `garmin-ical-export-1.0.5/setup.py` & `garmin-ical-export-1.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 def readme():
     with open("README.md", encoding='utf-8') as f:
         return f.read()
 
 
 setup(
     name="garmin-ical-export",
-    version="1.0.5",
+    version="1.0.6",
     description="Export Garmin Connect activities to iCalendar file",
     long_description=readme(),
     long_description_content_type="text/markdown",
     author="Jiri Kuchta",
     author_email="jiri.kuchta@email.cz",
     url="https://github.com/jirikuchta/garmin-ical-export",
     packages=["garminicalexport"],
```

