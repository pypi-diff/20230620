# Comparing `tmp/unifi_tracker-0.0.6.tar.gz` & `tmp/unifi_tracker-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unifi_tracker-0.0.6.tar", last modified: Thu Sep  8 01:09:32 2022, max compression
+gzip compressed data, was "unifi_tracker-0.0.7.tar", last modified: Mon Jun 19 23:20:29 2023, max compression
```

## Comparing `unifi_tracker-0.0.6.tar` & `unifi_tracker-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2022-09-08 01:09:32.882900 unifi_tracker-0.0.6/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     1071 2022-09-08 00:58:37.000000 unifi_tracker-0.0.6/LICENSE
--rw-r--r--   0 joelp     (1000) joelp     (1000)     5912 2022-09-08 01:09:32.882900 unifi_tracker-0.0.6/PKG-INFO
--rw-r--r--   0 joelp     (1000) joelp     (1000)     5343 2022-09-08 00:59:30.000000 unifi_tracker-0.0.6/README.md
--rw-r--r--   0 joelp     (1000) joelp     (1000)      103 2022-01-19 19:50:03.000000 unifi_tracker-0.0.6/pyproject.toml
--rw-r--r--   0 joelp     (1000) joelp     (1000)      694 2022-09-08 01:09:32.882900 unifi_tracker-0.0.6/setup.cfg
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2022-09-08 01:09:32.882900 unifi_tracker-0.0.6/src/
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2022-09-08 01:09:32.882900 unifi_tracker-0.0.6/src/unifi_tracker/
--rw-r--r--   0 joelp     (1000) joelp     (1000)      160 2022-09-08 00:59:30.000000 unifi_tracker-0.0.6/src/unifi_tracker/__init__.py
--rw-r--r--   0 joelp     (1000) joelp     (1000)     5764 2022-09-08 00:59:30.000000 unifi_tracker-0.0.6/src/unifi_tracker/unifi_tracker.py
-drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2022-09-08 01:09:32.882900 unifi_tracker-0.0.6/src/unifi_tracker.egg-info/
--rw-r--r--   0 joelp     (1000) joelp     (1000)     5912 2022-09-08 01:09:32.000000 unifi_tracker-0.0.6/src/unifi_tracker.egg-info/PKG-INFO
--rw-r--r--   0 joelp     (1000) joelp     (1000)      271 2022-09-08 01:09:32.000000 unifi_tracker-0.0.6/src/unifi_tracker.egg-info/SOURCES.txt
--rw-r--r--   0 joelp     (1000) joelp     (1000)        1 2022-09-08 01:09:32.000000 unifi_tracker-0.0.6/src/unifi_tracker.egg-info/dependency_links.txt
--rw-r--r--   0 joelp     (1000) joelp     (1000)       14 2022-09-08 01:09:32.000000 unifi_tracker-0.0.6/src/unifi_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     1071 2023-06-19 21:44:59.000000 unifi_tracker-0.0.7/LICENSE
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6140 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/PKG-INFO
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     5571 2023-06-19 21:37:12.000000 unifi_tracker-0.0.7/README.md
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      103 2022-01-19 19:50:03.000000 unifi_tracker-0.0.7/pyproject.toml
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      694 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/setup.cfg
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/src/
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/src/unifi_tracker/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      160 2023-06-19 21:45:24.000000 unifi_tracker-0.0.7/src/unifi_tracker/__init__.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6971 2023-06-19 23:08:20.000000 unifi_tracker-0.0.7/src/unifi_tracker/unifi_tracker.py
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     6140 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/PKG-INFO
+-rw-r--r--   0 joelp     (1000) joelp     (1000)      321 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/SOURCES.txt
+-rw-r--r--   0 joelp     (1000) joelp     (1000)        1 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/dependency_links.txt
+-rw-r--r--   0 joelp     (1000) joelp     (1000)       14 2023-06-19 23:20:29.000000 unifi_tracker-0.0.7/src/unifi_tracker.egg-info/top_level.txt
+drwxr-xr-x   0 joelp     (1000) joelp     (1000)        0 2023-06-19 23:20:29.227165 unifi_tracker-0.0.7/tests/
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2263 2022-02-09 21:14:36.000000 unifi_tracker-0.0.7/tests/test_diff.py
+-rw-r--r--   0 joelp     (1000) joelp     (1000)     2100 2023-06-19 21:19:32.000000 unifi_tracker-0.0.7/tests/test_property_setters.py
```

### Comparing `unifi_tracker-0.0.6/LICENSE` & `unifi_tracker-0.0.7/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Joel Pothering
+Copyright (c) 2023 Joel Pothering
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `unifi_tracker-0.0.6/PKG-INFO` & `unifi_tracker-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi_tracker
-Version: 0.0.6
+Version: 0.0.7
 Summary: Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 Home-page: https://github.com/idatum/unifi_tracker
 Author: Joel P.
 Author-email: joelp@live.com
 Project-URL: Bug Tracker, https://github.com/idatum/unifi_tracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,18 @@
 
 Summary
 -
 Works fine generally, basically like the existing HA unifi_direct, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.0.7
+- Added device_tracker.py option ```--processes``` to control the number of concurrent processes run during AP scanning, or to run them sequentially (i.e. ```--processes=0```).
+- Tested under Python11 and Debian12.
+-
 ### v0.0.6
 - Update README and docstrings corresponding to changes in HA 2022.9.
 ### v0.0.5
 - Added device_tracker.py options ```--homePayload``` (default is "home") and ```--awayPayload``` for MQTT message payload, corresponding to home and away presence. Starting with HA 2022.6, if you define your devices under HA's ```mqtt``` platform instead of ```device_tracker```, you should use ```--awayPayload=not_home```.
 ### v0.0.4
 - Missed updating module version in v0.0.3 release; now 0.0.4.
 ### v0.0.3
```

### Comparing `unifi_tracker-0.0.6/README.md` & `unifi_tracker-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,18 @@
 
 Summary
 -
 Works fine generally, basically like the existing HA unifi_direct, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.0.7
+- Added device_tracker.py option ```--processes``` to control the number of concurrent processes run during AP scanning, or to run them sequentially (i.e. ```--processes=0```).
+- Tested under Python11 and Debian12.
+-
 ### v0.0.6
 - Update README and docstrings corresponding to changes in HA 2022.9.
 ### v0.0.5
 - Added device_tracker.py options ```--homePayload``` (default is "home") and ```--awayPayload``` for MQTT message payload, corresponding to home and away presence. Starting with HA 2022.6, if you define your devices under HA's ```mqtt``` platform instead of ```device_tracker```, you should use ```--awayPayload=not_home```.
 ### v0.0.4
 - Missed updating module version in v0.0.3 release; now 0.0.4.
 ### v0.0.3
```

### Comparing `unifi_tracker-0.0.6/setup.cfg` & `unifi_tracker-0.0.7/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = unifi_tracker
-version = 0.0.6
+version = 0.0.7
 author = Joel P.
 author_email = joelp@live.com
 description = Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/idatum/unifi_tracker
 project_urls =
```

### Comparing `unifi_tracker-0.0.6/src/unifi_tracker/unifi_tracker.py` & `unifi_tracker-0.0.7/src/unifi_tracker/unifi_tracker.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import json
 import logging
 from paramiko import WarningPolicy
 from paramiko import SSHClient
 from multiprocessing import Pool
 
 _LOGGER = logging.getLogger("unifi_tracker")
@@ -25,14 +26,16 @@
         # Unifi command to remotely call via SSH.
         self.UNIFI_CMDLINE = 'mca-dump'
         # Properties to extract from returned JSON.
         self.UNIFI_SSID_TABLE = 'vap_table'
         self.UNIFI_CLIENT_TABLE = 'sta_table'
         # Some reasonable limit to number of hosts to scan in parallel.
         self.MAX_AP_HOST_SCANS = 32
+        # Scanning processes run in parallel; set to 0 to run serially.
+        self._processes = os.cpu_count()
 
     @property
     def UseHostKeys(self):
         '''Whether to ignore existing SSH client host key.'''
         return self._useHostKeys
 
     @UseHostKeys.setter
@@ -53,14 +56,23 @@
         '''WiFi client idle time threshold in seconds.'''
         return self._maxIdleTime
 
     @MaxIdleTime.setter
     def MaxIdleTime(self, value: int):
         self._maxIdleTime = value
 
+    @property
+    def Processes(self):
+        '''Scanning processes run in parallel; set to 0 for sequential processing.'''
+        return self._processes
+
+    @Processes.setter
+    def Processes(self, value: int):
+        self._processes = value
+
     def exec_ssh_cmdline(self, user: str, host: str, cmdline: str):
         '''Remotely execute command via SSH'''
         try:
             if self._useHostKeys:
                 _LOGGER.debug("Using system host keys file.")
                 self.ssh_client.load_system_host_keys()
             else:
@@ -89,41 +101,59 @@
                 _LOGGER.debug(jresult)
                 raise UnifiTrackerException(f"No client table {ap_host}")
             ap_clients += ssid.get(self.UNIFI_CLIENT_TABLE)
         return ap_clients
 
     def get_ap_mac_clients(self, ssh_username: str, ap_host: str):
         '''MAC to client JSON from a Unifi AP'''
+        _LOGGER.debug(f'Scanning {ap_host}.')
         return {client.get('mac').upper(): client for client in self.get_ap_clients(ssh_username=ssh_username, ap_host=ap_host)}
 
+    def parallel_scan(self, ssh_username: str, ap_hosts: list[str]):
+        '''List of results of parallel calls to get_ap_mac_clients.'''
+        with Pool(processes=self._processes) as pool:
+            _LOGGER.debug(f'Running {self._processes} scans in parallel.')
+            return pool.starmap(self.get_ap_mac_clients, [(ssh_username, ap_host) for ap_host in ap_hosts])
+
+    def sequential_scan(self, ssh_username: str, ap_hosts: list[str]):
+        '''List of results of sequential calls to get_ap_mac_clients'''
+        all_ap_mac_clients = []
+        for ap_host in ap_hosts:
+            macs_res = self.get_ap_mac_clients(ssh_username, ap_host)
+            all_ap_mac_clients.append(macs_res)
+        return all_ap_mac_clients
+
     def scan_aps(self, ssh_username: str, ap_hosts: list[str], last_mac_clients: dict={}):
         '''Retrieve and merge clients from all APs; diff with last retrieved.
         Return tuple: dict of clients, list of client adds, list of client deletes.
         All AP retrievals need to succeed in order to process diff.
         '''
         _LOGGER.debug("scanning start")
         if len(ap_hosts) > self.MAX_AP_HOST_SCANS:
             raise UnifiTrackerException(f"Exceeded limit of {self.MAX_AP_HOST_SCANS} APs that can be scanned in parallel.")
         mac_clients = {}
         added = []
         deleted = []
-        with Pool() as pool:
-            for ap_mac_clients in pool.starmap(self.get_ap_mac_clients, [(ssh_username, ap_host) for ap_host in ap_hosts]):
-                if self._maxIdleTime is None:
-                    mac_clients.update(ap_mac_clients)
-                else:
-                    # Filter on clients below idle time threshold
-                    for mac, client in ap_mac_clients.items():
-                        idletime = client["idletime"] if 'idletime' in client else 0
-                        _LOGGER.debug(f'{mac} idletime={idletime}')
-                        if idletime > self._maxIdleTime:
-                            if mac in last_mac_clients:
-                                _LOGGER.info(f'{mac} exceeded idle time threshold; excluding.')
-                            continue
-                        mac_clients[mac] = client
+        if self._processes == 0:
+            all_ap_mac_clients = self.sequential_scan(ssh_username, ap_hosts)
+        else:
+            all_ap_mac_clients = self.parallel_scan(ssh_username, ap_hosts)
+        for ap_mac_clients in all_ap_mac_clients:
+            if self._maxIdleTime is None:
+                mac_clients.update(ap_mac_clients)
+            else:
+                # Filter on clients below idle time threshold
+                for mac, client in ap_mac_clients.items():
+                    idletime = client["idletime"] if 'idletime' in client else 0
+                    _LOGGER.debug(f'{mac} idletime={idletime}')
+                    if idletime > self._maxIdleTime:
+                        if mac in last_mac_clients:
+                            _LOGGER.info(f'{mac} exceeded idle time threshold; excluding.')
+                        continue
+                    mac_clients[mac] = client
         for mac, client in mac_clients.items():
             if mac not in last_mac_clients:
                 added.append(mac)
                 hostname = f"{client['hostname']} ({mac})" if 'hostname' in client else mac
                 _LOGGER.info(f"added {hostname}")
         for mac, client in last_mac_clients.items():
             if mac not in mac_clients:
```

### Comparing `unifi_tracker-0.0.6/src/unifi_tracker.egg-info/PKG-INFO` & `unifi_tracker-0.0.7/src/unifi_tracker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unifi-tracker
-Version: 0.0.6
+Version: 0.0.7
 Summary: Track the comings and goings of WiFi clients on multiple Unifi APs and generate a diff between scans.
 Home-page: https://github.com/idatum/unifi_tracker
 Author: Joel P.
 Author-email: joelp@live.com
 Project-URL: Bug Tracker, https://github.com/idatum/unifi_tracker/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -77,14 +77,18 @@
 
 Summary
 -
 Works fine generally, basically like the existing HA unifi_direct, and allows me to more freely innovate and be less dependent on another component for running HA for my home automation.
 
 History
 -
+### v0.0.7
+- Added device_tracker.py option ```--processes``` to control the number of concurrent processes run during AP scanning, or to run them sequentially (i.e. ```--processes=0```).
+- Tested under Python11 and Debian12.
+-
 ### v0.0.6
 - Update README and docstrings corresponding to changes in HA 2022.9.
 ### v0.0.5
 - Added device_tracker.py options ```--homePayload``` (default is "home") and ```--awayPayload``` for MQTT message payload, corresponding to home and away presence. Starting with HA 2022.6, if you define your devices under HA's ```mqtt``` platform instead of ```device_tracker```, you should use ```--awayPayload=not_home```.
 ### v0.0.4
 - Missed updating module version in v0.0.3 release; now 0.0.4.
 ### v0.0.3
```

