# Comparing `tmp/hass-nabucasa-0.8.tar.gz` & `tmp/hass-nabucasa-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hass-nabucasa-0.8.tar", last modified: Tue Mar 19 13:14:00 2019, max compression
+gzip compressed data, was "dist/hass-nabucasa-0.9.tar", last modified: Thu Mar 21 15:12:51 2019, max compression
```

## Comparing `hass-nabucasa-0.8.tar` & `hass-nabucasa-0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-19 13:14:00.000000 hass-nabucasa-0.8/
--rw-r--r--   0 root         (0) root         (0)      909 2019-03-19 13:14:00.000000 hass-nabucasa-0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       39 2019-03-01 22:18:23.000000 hass-nabucasa-0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-19 13:14:00.000000 hass-nabucasa-0.8/hass_nabucasa/
--rw-r--r--   0 root         (0) root         (0)     6232 2019-03-11 09:43:41.000000 hass-nabucasa-0.8/hass_nabucasa/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13557 2019-03-15 12:30:59.000000 hass-nabucasa-0.8/hass_nabucasa/acme.py
--rw-r--r--   0 root         (0) root         (0)     6468 2019-03-11 09:43:41.000000 hass-nabucasa-0.8/hass_nabucasa/auth.py
--rw-r--r--   0 root         (0) root         (0)     2199 2019-03-15 12:30:59.000000 hass-nabucasa-0.8/hass_nabucasa/client.py
--rw-r--r--   0 root         (0) root         (0)     2260 2019-03-11 09:43:41.000000 hass-nabucasa-0.8/hass_nabucasa/cloud_api.py
--rw-r--r--   0 root         (0) root         (0)     2283 2019-03-12 11:06:17.000000 hass-nabucasa-0.8/hass_nabucasa/cloudhooks.py
--rw-r--r--   0 root         (0) root         (0)     1869 2019-03-15 13:15:14.000000 hass-nabucasa-0.8/hass_nabucasa/const.py
--rw-r--r--   0 root         (0) root         (0)    10736 2019-03-15 12:30:59.000000 hass-nabucasa-0.8/hass_nabucasa/iot.py
--rw-r--r--   0 root         (0) root         (0)    10378 2019-03-19 13:13:44.000000 hass-nabucasa-0.8/hass_nabucasa/remote.py
--rw-r--r--   0 root         (0) root         (0)     2468 2019-03-15 12:30:59.000000 hass-nabucasa-0.8/hass_nabucasa/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-19 13:14:00.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/
--rw-r--r--   0 root         (0) root         (0)      909 2019-03-19 13:13:59.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      488 2019-03-19 13:14:00.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-03-19 13:13:59.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-03-19 13:13:59.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       78 2019-03-19 13:13:59.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2019-03-19 13:13:59.000000 hass-nabucasa-0.8/hass_nabucasa.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      432 2019-03-19 13:14:00.000000 hass-nabucasa-0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1273 2019-03-19 13:13:44.000000 hass-nabucasa-0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/
+-rw-r--r--   0 root         (0) root         (0)      909 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       39 2019-03-01 22:18:23.000000 hass-nabucasa-0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa/
+-rw-r--r--   0 root         (0) root         (0)     6232 2019-03-11 09:43:41.000000 hass-nabucasa-0.9/hass_nabucasa/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13557 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/acme.py
+-rw-r--r--   0 root         (0) root         (0)     6468 2019-03-11 09:43:41.000000 hass-nabucasa-0.9/hass_nabucasa/auth.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/client.py
+-rw-r--r--   0 root         (0) root         (0)     2260 2019-03-11 09:43:41.000000 hass-nabucasa-0.9/hass_nabucasa/cloud_api.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2019-03-12 11:06:17.000000 hass-nabucasa-0.9/hass_nabucasa/cloudhooks.py
+-rw-r--r--   0 root         (0) root         (0)     1869 2019-03-15 13:15:14.000000 hass-nabucasa-0.9/hass_nabucasa/const.py
+-rw-r--r--   0 root         (0) root         (0)    10736 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/iot.py
+-rw-r--r--   0 root         (0) root         (0)    10439 2019-03-21 15:12:30.000000 hass-nabucasa-0.9/hass_nabucasa/remote.py
+-rw-r--r--   0 root         (0) root         (0)     2468 2019-03-15 12:30:59.000000 hass-nabucasa-0.9/hass_nabucasa/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      909 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      488 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       78 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/hass_nabucasa.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      432 2019-03-21 15:12:51.000000 hass-nabucasa-0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1273 2019-03-21 15:12:30.000000 hass-nabucasa-0.9/setup.py
```

### Comparing `hass-nabucasa-0.8/PKG-INFO` & `hass-nabucasa-0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: hass-nabucasa
-Version: 0.8
+Version: 0.9
 Summary: Home Assistant cloud integration by Nabu Casa, inc.
 Home-page: https://www.nabucasa.com/
 Author: Nabu Casa, Inc.
 Author-email: opensource@nabucasa.com
 License: GPL v3
-Download-URL: https://github.com/NabuCasa/hass-nabucasa/tarball/0.8
+Download-URL: https://github.com/NabuCasa/hass-nabucasa/tarball/0.9
 Description: UNKNOWN
 Keywords: homeassistant,cloud
 Platform: any
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `hass-nabucasa-0.8/hass_nabucasa/__init__.py` & `hass-nabucasa-0.9/hass_nabucasa/__init__.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/acme.py` & `hass-nabucasa-0.9/hass_nabucasa/acme.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/auth.py` & `hass-nabucasa-0.9/hass_nabucasa/auth.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/client.py` & `hass-nabucasa-0.9/hass_nabucasa/client.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/cloud_api.py` & `hass-nabucasa-0.9/hass_nabucasa/cloud_api.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/cloudhooks.py` & `hass-nabucasa-0.9/hass_nabucasa/cloudhooks.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/const.py` & `hass-nabucasa-0.9/hass_nabucasa/const.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/iot.py` & `hass-nabucasa-0.9/hass_nabucasa/iot.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa/remote.py` & `hass-nabucasa-0.9/hass_nabucasa/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,14 +291,15 @@
 
                 self.cloud.client.dispatcher_message(const.DISPATCH_REMOTE_DISCONNECT)
                 await asyncio.sleep(random.randint(1, 15))
                 await self.connect()
         except asyncio.CancelledError:
             pass
         finally:
+            _LOGGER.debug("Close remote UI reconnect guard")
             self._reconnect_task = None
 
     async def _certificate_handler(self) -> None:
         """Handle certification ACME Tasks."""
         try:
             while True:
                 await asyncio.sleep(utils.next_midnight())
```

### Comparing `hass-nabucasa-0.8/hass_nabucasa/utils.py` & `hass-nabucasa-0.9/hass_nabucasa/utils.py`

 * *Files identical despite different names*

### Comparing `hass-nabucasa-0.8/hass_nabucasa.egg-info/PKG-INFO` & `hass-nabucasa-0.9/hass_nabucasa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: hass-nabucasa
-Version: 0.8
+Version: 0.9
 Summary: Home Assistant cloud integration by Nabu Casa, inc.
 Home-page: https://www.nabucasa.com/
 Author: Nabu Casa, Inc.
 Author-email: opensource@nabucasa.com
 License: GPL v3
-Download-URL: https://github.com/NabuCasa/hass-nabucasa/tarball/0.8
+Download-URL: https://github.com/NabuCasa/hass-nabucasa/tarball/0.9
 Description: UNKNOWN
 Keywords: homeassistant,cloud
 Platform: any
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `hass-nabucasa-0.8/setup.py` & `hass-nabucasa-0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup
 
-VERSION = "0.8"
+VERSION = "0.9"
 
 setup(
     name="hass-nabucasa",
     version=VERSION,
     license="GPL v3",
     author="Nabu Casa, Inc.",
     author_email="opensource@nabucasa.com",
@@ -26,14 +26,14 @@
     ],
     keywords=["homeassistant", "cloud"],
     zip_safe=False,
     platforms="any",
     packages=["hass_nabucasa"],
     install_requires=[
         "warrant==0.6.1",
-        "snitun==0.15",
+        "snitun==0.17",
         "acme==0.32.0",
         "cryptography>=2.5",
         "attrs>=18.2.0",
         "pytz",
     ],
 )
```

