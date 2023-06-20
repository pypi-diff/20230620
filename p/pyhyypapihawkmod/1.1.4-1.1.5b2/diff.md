# Comparing `tmp/pyhyypapihawkmod-1.1.4.tar.gz` & `tmp/pyhyypapihawkmod-1.1.5b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.1.4.tar", last modified: Sun Jun 18 10:38:22 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.5b2.tar", last modified: Tue Jun 20 10:40:42 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.1.4.tar` & `pyhyypapihawkmod-1.1.5b2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.068194 pyhyypapihawkmod-1.1.4/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-06-18 10:38:22.066683 pyhyypapihawkmod-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2060 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.045209 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     7697 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-06-18 10:38:22.063686 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-18 10:38:21.000000 pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-18 10:38:22.068194 pyhyypapihawkmod-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-06-18 10:36:49.000000 pyhyypapihawkmod-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:40:42.034148 pyhyypapihawkmod-1.1.5b2/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/MANIFEST.in
+-rw-rw-rw-   0        0        0      519 2023-06-20 10:40:42.033639 pyhyypapihawkmod-1.1.5b2/PKG-INFO
+-rw-rw-rw-   0        0        0     2126 2023-06-20 10:39:09.000000 pyhyypapihawkmod-1.1.5b2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:40:42.021409 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-06-19 07:52:00.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     8139 2023-06-20 10:38:34.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27863 2023-06-20 10:21:52.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:40:42.031614 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      519 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 10:40:41.000000 pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:40:42.034148 pyhyypapihawkmod-1.1.5b2/setup.cfg
+-rw-rw-rw-   0        0        0      923 2023-06-20 10:38:42.000000 pyhyypapihawkmod-1.1.5b2/setup.py
```

### Comparing `pyhyypapihawkmod-1.1.4/LICENSE.md` & `pyhyypapihawkmod-1.1.5b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/PKG-INFO` & `pyhyypapihawkmod-1.1.5b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.4
+Version: 1.1.5b2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.4/README.md` & `pyhyypapihawkmod-1.1.5b2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
 - CLI usage. (GCF client is there, just needs some more automation.)
 - Capture panic api...for obvious reasons.
 - What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
 
 
 Changelog 
 
+1.1.5
+- Added functions to supply notifications for debugging
+
 1.1.4
 - Bugfix: When no "triggers" exist a blank key is now returned instead of nothing. This caused a KeyError in home assistant.
 
 1.1.3
 - Bugfix: Fixes a bug when calling notifications
 
 1.1.2
```

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/alarm_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,7 +201,23 @@
     def status(self) -> dict[Any, Any]:
         """Return the status of Hyyp connected alarms."""
 
         self._fetch_data()
         formatted_data: dict[Any, Any] = self._format_data()
 
         return formatted_data
+
+
+
+    def debug_notifications(self) -> dict[Any, Any]:
+        """Pull notifications for debug purposes."""
+        # The API returns data from site level.
+
+        self._fetch_data()
+        site_ids = {site["id"]: site for site in self._sync_info["sites"]}
+        
+        for site in site_ids:
+            self._fetch_notifications(site_id=site)
+            site_ids[site] = self._notifications
+
+
+        return site_ids
```

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,18 @@
         return _json_result
 
     def load_alarm_infos(self) -> dict[Any, Any]:
         """Get alarm infos formatted for hass infos."""
 
         return HyypAlarmInfos(self).status()
 
+    def get_debug_notifications(self) -> dict[Any, Any]:
+        """Get alarm infos formatted for hass infos."""
+        return HyypAlarmInfos(self).debug_notifications()
+
     def site_notifications(
         self, site_id: int, timestamp: int | None = None, json_key: int | None = None
     ) -> Any:
         """Get site notifications from API."""
 
         _params: dict[str, Any] = STD_PARAMS.copy()
         _params["siteId"] = site_id
```

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.1.4
+Version: 1.1.5b2
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.1.4/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.5b2/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.1.4/setup.py` & `pyhyypapihawkmod-1.1.5b2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.1.4",
+    version="1.1.5b2",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

