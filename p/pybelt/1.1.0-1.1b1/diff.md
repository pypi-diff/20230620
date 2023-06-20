# Comparing `tmp/pybelt-1.1.0.tar.gz` & `tmp/pybelt-1.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\pybelt-1.1.0.tar", last modified: Tue Jun 20 12:21:41 2023, max compression
+gzip compressed data, was "dist\pybelt-1.1b1.tar", last modified: Tue May 16 07:31:38 2023, max compression
```

## Comparing `pybelt-1.1.0.tar` & `pybelt-1.1b1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 12:21:41.000000 pybelt-1.1.0/
--rw-rw-rw-   0        0        0     2472 2023-06-20 12:21:41.000000 pybelt-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt/
--rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.1.0/pybelt/__init__.py
--rw-rw-rw-   0        0        0    37069 2023-05-16 07:04:42.000000 pybelt-1.1.0/pybelt/_communication_interface.py
--rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.1.0/pybelt/_gatt_profile.py
--rw-rw-rw-   0        0        0    62919 2023-06-20 12:09:19.000000 pybelt-1.1.0/pybelt/belt_controller.py
--rw-rw-rw-   0        0        0     3980 2023-05-15 13:07:23.000000 pybelt-1.1.0/pybelt/belt_scanner.py
-drwxrwxrwx   0        0        0        0 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt.egg-info/
--rw-rw-rw-   0        0        0     2472 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-20 12:21:41.000000 pybelt-1.1.0/pybelt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-20 12:21:41.000000 pybelt-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      759 2023-06-20 12:20:49.000000 pybelt-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:31:38.000000 pybelt-1.1b1/
+-rw-rw-rw-   0        0        0     2472 2023-05-16 07:31:38.000000 pybelt-1.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0     1636 2021-01-11 09:49:47.000000 pybelt-1.1b1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt/
+-rw-rw-rw-   0        0        0      112 2020-06-22 14:06:02.000000 pybelt-1.1b1/pybelt/__init__.py
+-rw-rw-rw-   0        0        0    37069 2023-05-16 07:04:42.000000 pybelt-1.1b1/pybelt/_communication_interface.py
+-rw-rw-rw-   0        0        0     8833 2023-01-05 13:18:44.000000 pybelt-1.1b1/pybelt/_gatt_profile.py
+-rw-rw-rw-   0        0        0    59380 2023-05-09 09:02:51.000000 pybelt-1.1b1/pybelt/belt_controller.py
+-rw-rw-rw-   0        0        0     3980 2023-05-15 13:07:23.000000 pybelt-1.1b1/pybelt/belt_scanner.py
+drwxrwxrwx   0        0        0        0 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/
+-rw-rw-rw-   0        0        0     2472 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-16 07:31:38.000000 pybelt-1.1b1/pybelt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 07:31:38.000000 pybelt-1.1b1/setup.cfg
+-rw-rw-rw-   0        0        0      759 2023-05-16 07:31:01.000000 pybelt-1.1b1/setup.py
```

### Comparing `pybelt-1.1.0/PKG-INFO` & `pybelt-1.1b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.1.0
+Version: 1.1b1
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 License: UNKNOWN
 Description: # pyBelt
```

### Comparing `pybelt-1.1.0/README.md` & `pybelt-1.1b1/README.md`

 * *Files identical despite different names*

### Comparing `pybelt-1.1.0/pybelt/_communication_interface.py` & `pybelt-1.1b1/pybelt/_communication_interface.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.1.0/pybelt/_gatt_profile.py` & `pybelt-1.1b1/pybelt/_gatt_profile.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.1.0/pybelt/belt_controller.py` & `pybelt-1.1b1/pybelt/belt_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -335,19 +335,14 @@
         """
         self._notifications_handlers.remove(handler)
 
     def set_orientation_notifications(self, enabled) -> bool:
         """
         Sets the state of orientation notifications.
 
-        IMPORTANT: It is important to note that orientation updates from the belt were not designed for updating a
-        system in real-time, just for monitoring and showing on a map the orientation of the belt. In case you need a
-        vibration signal on the belt that is dependent on the orientation, you can use the `vibrate_at_magnetic_bearing`
-        or `send_pulse_command` (with orientation_type=MAGNETIC_BEARING) to get a vibration relative to magnetic North.
-
         :param enabled: 'True' to enable orientation notifications, 'False' to disable.
         :return: 'True' if the request has been sent successfully.
         """
         if self._connection_state == BeltConnectionState.DISCONNECTED:
             return False
         return self._communication_interface.set_gatt_notifications(self._gatt_profile.orientation_data_char, enabled)
 
@@ -430,64 +425,14 @@
                     (0x01 if save else 0x00),
                     (0x01 if pairing_required else 0x00)]),
                 self._gatt_profile.param_notification_char)
         if write_result == 2:
             raise TimeoutError("Timeout period reached when setting pairing requirement.")
         return write_result == 0
 
-    def set_orientation_notification_period(self, period, start_notification) -> bool:
-        """
-        Sets the period for orientation notifications.
-
-        Changing the period of orientation notifications is only available from firmware version 52. The minimum
-        notification period supported by the belt is 20ms (i.e. 50Hz).
-
-        IMPORTANT: It is important to note that orientation updates from the belt were not designed for updating a
-        system in real-time, just for monitoring and showing on a map the orientation of the belt. In case you need a
-        vibration signal on the belt that is dependent on the orientation, you can use the `vibrate_at_magnetic_bearing`
-        or `send_pulse_command` (with orientation_type=MAGNETIC_BEARING) to get a vibration relative to magnetic North.
-
-        The belt orientation may be inaccurate when used indoor because of magnetic interference. To get a better
-        orientation, it is recommended to calibrate the belt in the room where it is used (or outdoor if used outdoor).
-
-        It is not recommended to use short notification period over BLE connection. For short notification
-        periods, after disconnection, it may be required to wait a few seconds to reconnect the belt again. If the
-        reconnection failed, it may be necessary to restart the belt. In case the belt does not respond anymore, you can
-        make a “hard power-off” by pressing the power button of the belt more than 6 seconds and then pressing it again
-        to restart the belt.
-
-        :param period: The period in seconds. Minimum value is 20 milliseconds (50Hz).
-        :param start_notification: 'True' to start the orientation notification.
-        :return: 'True' on success, 'False' otherwise.
-        """
-        if self.get_connection_state() != BeltConnectionState.CONNECTED:
-            self.logger.warning("BeltController: No belt belt connected to set notification period.")
-            return False
-        if self.get_firmware_version() < 52:
-            self.logger.warning("BeltController: Belt firmware version not supported.")
-            return False
-        if period < 0.02:
-            self.logger.warning("BeltController: Notification period not supported.")
-            return False
-        period_ms = int(period * 1000.0)
-        self.set_orientation_notifications(False)
-        if self.write_gatt(self._gatt_profile.param_request_char,
-                           bytes([
-                               0x11,
-                               0x0F,
-                               0x00,
-                               period_ms & 0xFF,
-                               (period_ms >> 8) & 0xFF,
-                           ]),
-                           self._gatt_profile.param_notification_char,
-                           b'\x10\x0F') != 0:
-            self.logger.warning("BeltController: Failed to write notification period parameter.")
-            return False
-        return self.set_orientation_notifications(True)
-
     def vibrate_at_magnetic_bearing(
             self,
             bearing,
             switch_to_app_mode=True,
             channel_index=1,
             intensity=None,
             clear_other_channels=False) -> bool:
@@ -631,15 +576,15 @@
                 (0x00 if pattern_iterations is None else pattern_iterations),
                 pattern_period & 0xFF,
                 (pattern_period >> 8) & 0xFF,
                 pattern_start_time & 0xFF,
                 (pattern_start_time >> 8) & 0xFF,
                 (0x01 if exclusive_channel else 0x00),
                 (0x01 if clear_other_channels else 0x00)
-            ])) == 0
+                ])) == 0
 
     def send_pulse_command(
             self,
             channel_index,
             orientation_type,
             orientation,
             intensity,
```

### Comparing `pybelt-1.1.0/pybelt/belt_scanner.py` & `pybelt-1.1b1/pybelt/belt_scanner.py`

 * *Files identical despite different names*

### Comparing `pybelt-1.1.0/pybelt.egg-info/PKG-INFO` & `pybelt-1.1b1/pybelt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybelt
-Version: 1.1.0
+Version: 1.1b1
 Summary: An Python library to control the feelSpace naviBelt from your application
 Home-page: https://github.com/feelSpace/pybelt
 Author: feelSpace GmbH
 Author-email: dev@feelspace.de
 License: UNKNOWN
 Description: # pyBelt
```

### Comparing `pybelt-1.1.0/setup.py` & `pybelt-1.1b1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybelt",
-    version="1.1.0",
+    version="1.1b1",
     author="feelSpace GmbH",
     author_email="dev@feelspace.de",
     description="An Python library to control the feelSpace naviBelt from your application",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/feelSpace/pybelt",
     packages=setuptools.find_packages(),
```

