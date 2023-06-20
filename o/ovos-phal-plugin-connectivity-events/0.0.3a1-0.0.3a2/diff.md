# Comparing `tmp/ovos-phal-plugin-connectivity-events-0.0.3a1.tar.gz` & `tmp/ovos-phal-plugin-connectivity-events-0.0.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a1.tar", last modified: Sat Jun 10 01:53:50 2023, max compression
+gzip compressed data, was "ovos-phal-plugin-connectivity-events-0.0.3a2.tar", last modified: Tue Jun 20 15:54:44 2023, max compression
```

## Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1.tar` & `ovos-phal-plugin-connectivity-events-0.0.3a2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.711756 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-06-10 01:53:42.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-10 01:53:45.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 01:53:50.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-10 01:53:42.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 01:53:50.715756 ovos-phal-plugin-connectivity-events-0.0.3a1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-10 01:53:42.000000 ovos-phal-plugin-connectivity-events-0.0.3a1/test/test_connectivity_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-06-20 15:54:35.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-20 15:54:39.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:54:44.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2729 2023-06-20 15:54:35.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:54:44.542964 ovos-phal-plugin-connectivity-events-0.0.3a2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-06-20 15:54:35.000000 ovos-phal-plugin-connectivity-events-0.0.3a2/test/test_connectivity_events.py
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # ovos-PHAL-plugin - Connectivity Events
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events/__init__.py` & `ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,17 @@
     """The host is connected to a network, and appears to be able to reach the
     full Internet."""
 
 
 class ConnectivityEvents(PHALPlugin):
 
     def __init__(self, bus=None, config=None):
-        super().__init__(bus=bus, name="ovos-PHAL-plugin-connectivity-events", config=config)
-        self.sleep_time = 60
+        super().__init__(bus=bus, name="ovos-PHAL-plugin-connectivity-events",
+                         config=config)
+        self.sleep_time = self.config.get("check_interval") or 60
         self.stopping = Event()
         self.state = ConnectivityState.UNKNOWN
         self.bus.on("ovos.PHAL.internet_check", self.handle_check)
 
     def run(self):
         if self.config.get("disable_scheduled_checks"):
             LOG.info("Scheduled Checks are disabled")
@@ -63,15 +64,15 @@
         emits `mycroft.internet.disconnected` if internet is newly disconnected
         emits `enclosure.notify.no_internet` if new state has
             some networking but no internet
         :param new_state: Current connection state
         :param message: Message associated with request to check internet state
         """
         message = message or Message("connectivity_check")
-        LOG.info(f"Network state changed to: {new_state.value}")
+        LOG.info(f"Network state changed to: {new_state.name}")
         if new_state == ConnectivityState.FULL:  # Gained internet
             if self.state <= ConnectivityState.NONE:  # Gained network
                 self.bus.emit(message.reply("mycroft.network.connected"))
             self.bus.emit(message.reply("mycroft.internet.connected"))
         elif new_state > ConnectivityState.NONE:  # Gained non-internet network
             if self.state <= ConnectivityState.NONE:  # Gained network
                 self.bus.emit(message.reply("mycroft.network.connected"))
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO` & `ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-phal-plugin-connectivity-events
-Version: 0.0.3a1
+Version: 0.0.3a2
 Summary: A PHAL plugin for mycroft/ovos/neon
 Home-page: https://github.com/OpenVoiceOS/ovos-PHAL-plugin-connectivity-events
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: # ovos-PHAL-plugin - Connectivity Events
```

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt` & `ovos-phal-plugin-connectivity-events-0.0.3a2/ovos_phal_plugin_connectivity_events.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1/setup.py` & `ovos-phal-plugin-connectivity-events-0.0.3a2/setup.py`

 * *Files identical despite different names*

### Comparing `ovos-phal-plugin-connectivity-events-0.0.3a1/test/test_connectivity_events.py` & `ovos-phal-plugin-connectivity-events-0.0.3a2/test/test_connectivity_events.py`

 * *Files identical despite different names*

