# Comparing `tmp/py-miraie-ac-0.1.4.tar.gz` & `tmp/py-miraie-ac-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-miraie-ac-0.1.4.tar", last modified: Tue Jun 13 07:43:23 2023, max compression
+gzip compressed data, was "py-miraie-ac-0.1.6.tar", last modified: Tue Jun 20 06:40:06 2023, max compression
```

## Comparing `py-miraie-ac-0.1.4.tar` & `py-miraie-ac-0.1.6.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.857454 py-miraie-ac-0.1.4/
--rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     1273 2023-06-13 07:43:23.857454 py-miraie-ac-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.4/README.md
--rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      801 2023-06-13 07:43:23.858450 py-miraie-ac-0.1.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.835462 py-miraie-ac-0.1.4/src/
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.852458 py-miraie-ac-0.1.4/src/py_miraie_ac/
--rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/__init__.py
--rw-rw-rw-   0        0        0     6716 2023-06-13 07:30:45.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/api.py
--rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/constants.py
--rw-rw-rw-   0        0        0     4928 2023-06-11 14:23:54.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/device.py
--rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/deviceStatus.py
--rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/enums.py
--rw-rw-rw-   0        0        0      121 2023-06-05 03:55:32.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/exceptions.py
--rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/home.py
--rw-rw-rw-   0        0        0     1585 2023-06-13 07:04:26.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/test.py
--rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/user.py
--rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.4/src/py_miraie_ac/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-13 07:43:23.856449 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/
--rw-rw-rw-   0        0        0     1273 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-13 07:43:23.000000 py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 06:40:06.905960 py-miraie-ac-0.1.6/
+-rw-rw-rw-   0        0        0    35821 2023-06-09 07:50:41.000000 py-miraie-ac-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     1273 2023-06-20 06:40:06.905960 py-miraie-ac-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      666 2023-06-13 02:52:22.000000 py-miraie-ac-0.1.6/README.md
+-rw-rw-rw-   0        0        0      104 2023-06-09 16:09:32.000000 py-miraie-ac-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0      801 2023-06-20 06:40:06.906959 py-miraie-ac-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-20 06:40:06.736074 py-miraie-ac-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-06-20 06:40:06.899961 py-miraie-ac-0.1.6/src/py_miraie_ac/
+-rw-rw-rw-   0        0        0      403 2023-06-09 13:16:33.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/__init__.py
+-rw-rw-rw-   0        0        0     6893 2023-06-20 06:38:31.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/api.py
+-rw-rw-rw-   0        0        0     6891 2023-06-20 05:43:54.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/broker.py
+-rw-rw-rw-   0        0        0      421 2023-06-05 03:33:43.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/constants.py
+-rw-rw-rw-   0        0        0     4906 2023-06-20 05:44:23.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/device.py
+-rw-rw-rw-   0        0        0      995 2023-06-10 12:09:13.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/deviceStatus.py
+-rw-rw-rw-   0        0        0      917 2023-06-05 03:55:22.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/enums.py
+-rw-rw-rw-   0        0        0      378 2023-06-20 05:51:20.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/exceptions.py
+-rw-rw-rw-   0        0        0      483 2023-06-09 13:29:18.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/home.py
+-rw-rw-rw-   0        0        0        0 2023-06-20 06:38:21.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/test.py
+-rw-rw-rw-   0        0        0      460 2023-06-05 03:57:35.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/user.py
+-rw-rw-rw-   0        0        0      236 2023-06-09 13:29:27.000000 py-miraie-ac-0.1.6/src/py_miraie_ac/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-20 06:40:06.904957 py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/
+-rw-rw-rw-   0        0        0     1273 2023-06-20 06:40:06.000000 py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      569 2023-06-20 06:40:06.000000 py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 06:40:06.000000 py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-06-20 06:40:06.000000 py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 06:40:06.000000 py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/top_level.txt
```

### Comparing `py-miraie-ac-0.1.4/LICENSE` & `py-miraie-ac-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/PKG-INFO` & `py-miraie-ac-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.4
+Version: 0.1.6
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.4/README.md` & `py-miraie-ac-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/setup.cfg` & `py-miraie-ac-0.1.6/setup.cfg`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 792d 6d69 7261 6965 2d61 630d   = py-miraie-ac.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e34  .version = 0.1.4
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e31 2e36  .version = 0.1.6
 00000030: 0d0a 6175 7468 6f72 203d 204d 696c 6f20  ..author = Milo 
 00000040: 5468 6f6d 6173 0d0a 6175 7468 6f72 5f65  Thomas..author_e
 00000050: 6d61 696c 203d 2032 3037 3139 3530 312b  mail = 20719501+
 00000060: 6d69 6c6f 7468 6f6d 6173 4075 7365 7273  milothomas@users
 00000070: 2e6e 6f72 6570 6c79 2e67 6974 6875 622e  .noreply.github.
 00000080: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000090: 203d 2041 2070 6163 6b61 6765 2074 6f20   = A package to
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/api.py` & `py-miraie-ac-0.1.6/src/py_miraie_ac/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,120 +1,121 @@
 """The MirAIe API module"""
 
 import math
 import random
 import asyncio
 from typing import Callable
-
 import aiohttp
 from py_miraie_ac.broker import MirAIeBroker
 from py_miraie_ac.device import Device
 from py_miraie_ac.constants import DEVICE_DETAILS_URL, HOMES_URL,HTTP_CLIENT_ID,LOGIN_URL,STATUS_URL
 from py_miraie_ac.deviceStatus import DeviceStatus
 from py_miraie_ac.enums import (
     AuthType,
     DisplayState,
     FanMode,
     HVACMode,
     PowerMode,
     PresetMode,
     SwingMode,
 )
-from py_miraie_ac.exceptions import AuthException
+from py_miraie_ac.exceptions import AuthException, ConnectionException, MobileNotRegisteredException
 from py_miraie_ac.home import Home
 from py_miraie_ac.user import User
 from py_miraie_ac.utils import to_float
 
 class MirAIeAPI:
     """The MirAIe API class"""
-    __auth_type: str
-    __login_id: str
-    __password: str
-    __http_session: aiohttp.ClientSession
-    __user: User
-    __home: Home
-    __topics: list[str] = []
-    __broker: MirAIeBroker
+    _auth_type: str
+    _login_id: str
+    _password: str
+    _http_session: aiohttp.ClientSession
+    _user: User
+    _home: Home
+    _topics: list[str] = []
+    _broker: MirAIeBroker
 
     @property
     def devices(self) -> list[Device]:
         """Returns a list of available devices."""
-        return list(self.__home.devices.values())
+        return list(self._home.devices.values())
 
     def __init__(self, auth_type: AuthType, login_id: str, password: str):
-        self.__auth_type = str(auth_type.value)
-        self.__login_id = login_id
-        self.__password = password
-        self.__http_session = aiohttp.ClientSession()
-        self.__broker = MirAIeBroker()
+        self._auth_type = str(auth_type.value)
+        self._login_id = login_id
+        self._password = password
+        self._http_session = aiohttp.ClientSession()
+        self._broker = MirAIeBroker()
 
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *excinfo):
-        await self.__http_session.close()
-        self.__broker.disconnect()
+        await self._http_session.close()
+        self._broker.disconnect()
 
     async def initialize(self):
         """Initializes the MirAIe API"""
 
-        self.__user = await self.__login()
-        self.__broker = MirAIeBroker()
-
-        self.__home = await self.__get_home_details()
-        self.__broker.set_topics(self.__topics)
-        self.__broker.init_broker(self.__home.home_id, self.__user.access_token, self.reconnect_broker)
-        self.__broker.connect()
+        self._user = await self._login()
+        self._home = await self._get_home_details()
+        self._broker.set_topics(self._topics)
+        self._broker.init_broker(self._home.home_id, self._user.access_token, self.reconnect_broker)
+        self._broker.connect()
 
     def reconnect_broker(self, reconnect_callback: Callable):
         """Authenticates with MirAIe and reconnects to MQTT server with the new credentials"""
-        loop = self.__http_session.loop
-        fut = asyncio.run_coroutine_threadsafe(self.__login(), loop)
+        loop = self._http_session.loop
+        fut = asyncio.run_coroutine_threadsafe(self._login(), loop)
 
-        self.__user = fut.result()
-        reconnect_callback(self.__home.home_id, self.__user.access_token)
+        self._user = fut.result()
+        reconnect_callback(self._home.home_id, self._user.access_token)
 
-    async def __login(self):
+    async def _login(self):
         data = {
             "clientId": HTTP_CLIENT_ID,
-            "password": self.__password,
-            "scope": self.__get_scope(),
+            "password": self._password,
+            "scope": self._get_scope(),
         }
 
-        data[self.__auth_type] = self.__login_id
-        response = await self.__http_session.post(LOGIN_URL, json=data)
+        data[self._auth_type] = self._login_id
+        response = await self._http_session.post(LOGIN_URL, json=data)
 
         if response.status == 200:
             json = await response.json()
             return User(
                 access_token=json["accessToken"],
                 refresh_token=json["refreshToken"],
                 user_id=json["userId"],
                 expires_in=json["expiresIn"],
             )
-
-        raise AuthException("Authentication failed")
-
-    async def __get_home_details(self):
-        response = await self.__http_session.get(
-            HOMES_URL, headers=self.__build_http_headers()
+        elif response.status == 401:
+            raise AuthException("Authentication failed")
+        elif response.status == 412:
+            raise MobileNotRegisteredException(await response.json())
+        else:
+            raise ConnectionException(await response.json())
+
+    async def _get_home_details(self):
+        response = await self._http_session.get(
+            HOMES_URL, headers=self._build_http_headers()
         )
         resp = await response.json()
-        return await self.__parse_home_details(resp[0])
+        return await self._parse_home_details(resp[0])
 
-    async def __parse_home_details(self, json_response):
+    async def _parse_home_details(self, json_response):
         devices: list[Device] = []
 
         for space in json_response["spaces"]:
             space_name = space["spaceName"]
             for device in space["devices"]:
                 device_id = device["deviceId"]
                 topic = str(device["topic"][0])
-                device_details = await self.__get_device_details(device_id)
-                device_status = await self.__get_device_status(device_id)
+                device_details = await self._get_device_details(device_id)
+                device_status = await self._get_device_status(device_id)
 
                 device = Device(
                     device_id=device_id,
                     name=str(device["deviceName"]).lower().replace(" ", "-"),
                     friendly_name=device["deviceName"],
                     control_topic=f"{topic}/control",
                     status_topic=f"{topic}/status",
@@ -124,41 +125,41 @@
                     category=device_details["category"],
                     brand=device_details["brand"],
                     firmware_version=device_details["firmwareVersion"],
                     serial_number=device_details["serialNumber"],
                     model_number=device_details["modelNumber"],
                     product_serial_number=device_details["productSerialNumber"],
                     status=device_status,
-                    broker=self.__broker,
+                    broker=self._broker,
                     area_name=space_name,
                 )
 
-                self.__topics.append(device.status_topic)
-                self.__topics.append(device.connection_status_topic)
+                self._topics.append(device.status_topic)
+                self._topics.append(device.connection_status_topic)
                 devices.append(device)
 
         return Home(home_id=json_response["homeId"], devices=devices)
 
-    async def __get_device_details(self, device_id: str):
+    async def _get_device_details(self, device_id: str):
         url = f"{DEVICE_DETAILS_URL}/{device_id}"
 
-        response = await self.__http_session.get(
+        response = await self._http_session.get(
             url,
-            headers=self.__build_http_headers(),
+            headers=self._build_http_headers(),
         )
 
         json = await response.json()
         return json[0]
 
-    async def __get_device_status(self, device_id: str):
+    async def _get_device_status(self, device_id: str):
         status: DeviceStatus
 
-        response = await self.__http_session.get(
+        response = await self._http_session.get(
             STATUS_URL.replace("{deviceId}", device_id),
-            headers=self.__build_http_headers(),
+            headers=self._build_http_headers(),
         )
 
         json = await response.json()
         status = DeviceStatus(
             is_online=json["onlineStatus"] == "true",
             temperature=to_float(json["actmp"]),
             room_temp=to_float(json["rmtmp"]),
@@ -173,16 +174,16 @@
             else PresetMode.NONE,
             vertical_swing_mode=SwingMode(json["acvs"]),
             horizontal_swing_mode=SwingMode(json["achs"]),
         )
 
         return status
 
-    def __build_http_headers(self):
+    def _build_http_headers(self):
         return {
-            "Authorization": f"Bearer {self.__user.access_token}"
+            "Authorization": f"Bearer {self._user.access_token}"
             ,"Content-Type": "application/json",
         }
 
-    def __get_scope(self):
+    def _get_scope(self):
         rnd = math.floor(random.random() * 1000000000)
         return f"an{str(rnd)}"
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/device.py` & `py-miraie-ac-0.1.6/src/py_miraie_ac/device.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from py_miraie_ac.deviceStatus import DeviceStatus
 from py_miraie_ac.enums import DisplayState, FanMode, HVACMode, PowerMode, PresetMode, SwingMode
 from py_miraie_ac.utils import to_float
 
 class Device:
     """The MirAIe device class"""
 
-    __broker: MirAIeBroker
-    __callbacks: list[Callable]
+    _broker: MirAIeBroker
+    _callbacks: list[Callable]
 
     def __init__(
         self,
         device_id: str,
         name: str,
         friendly_name: str,
         control_topic: str,
@@ -45,32 +45,32 @@
         self.firmware_version = firmware_version
         self.serial_number = serial_number
         self.model_number = model_number
         self.product_serial_number = product_serial_number
         self.status = status
         self.area_name = area_name
 
-        self.__broker = broker
-        self.__callbacks = []
-        self.__broker.register_callback(self.status_topic, self.status_callback_handler)
-        self.__broker.register_callback(
+        self._broker = broker
+        self._callbacks = []
+        self._broker.register_callback(self.status_topic, self.status_callback_handler)
+        self._broker.register_callback(
             self.connection_status_topic, self.connection_callback_handler
         )
 
-    def __publish_state(self):
-        for callback in self.__callbacks:
+    def _publish_state(self):
+        for callback in self._callbacks:
             callback()
 
     def status_callback_handler(self, status: dict):
         """Handles MQTT messages received on the status topic"""
 
-        self.status = self.__parse_status_response(status)
-        self.__publish_state()
+        self.status = self._parse_status_response(status)
+        self._publish_state()
 
-    def __parse_status_response(self, json: dict) -> DeviceStatus:
+    def _parse_status_response(self, json: dict) -> DeviceStatus:
         is_online = self.status.is_online
         if "onlineStatus" in json:
             is_online = json["onlineStatus"] == "true"
 
         device_status = DeviceStatus(
             is_online=is_online,
             temperature=to_float(json["actmp"]),
@@ -91,48 +91,48 @@
         return device_status
 
     def connection_callback_handler(self, status: dict):
         """Handles MQTT messages received on the connection status topic"""
 
         if "onlineStatus" in status:
             self.status.is_online = status["onlineStatus"] == "true"
-            self.__publish_state()
+            self._publish_state()
 
     def set_temperature(self, temp: float):
         """Sets the temperature"""
-        self.__broker.set_temperature(self.control_topic, temp)
+        self._broker.set_temperature(self.control_topic, temp)
 
     def turn_on(self):
         """Turns on the devie"""
-        self.__broker.set_power(self.control_topic, PowerMode.ON)
+        self._broker.set_power(self.control_topic, PowerMode.ON)
 
     def turn_off(self):
         """Turns off the device"""
-        self.__broker.set_power(self.control_topic, PowerMode.OFF)
+        self._broker.set_power(self.control_topic, PowerMode.OFF)
 
     def set_hvac_mode(self, mode: HVACMode):
         """Sets the HVAC mode"""
-        self.__broker.set_hvac_mode(self.control_topic, mode)
+        self._broker.set_hvac_mode(self.control_topic, mode)
 
     def set_fan_mode(self, mode: FanMode):
         """Sets the fan mode"""
-        self.__broker.set_fan_mode(self.control_topic, mode)
+        self._broker.set_fan_mode(self.control_topic, mode)
 
     def set_preset_mode(self, mode: PresetMode):
         """Sets the preset mode"""
-        self.__broker.set_preset_mode(self.control_topic, mode)
+        self._broker.set_preset_mode(self.control_topic, mode)
 
     def set_vertical_swing_mode(self, mode: SwingMode):
         """Sets the swing mode"""
-        self.__broker.set_vertical_swing_mode(self.control_topic, mode)
+        self._broker.set_vertical_swing_mode(self.control_topic, mode)
 
     def set_horizontal_swing_mode(self, mode: SwingMode):
         """Sets the swing mode"""
-        self.__broker.set_horizontal_swing_mode(self.control_topic, mode)
+        self._broker.set_horizontal_swing_mode(self.control_topic, mode)
 
     def register_callback(self, callback: Callable[[], None]) -> None:
         """Registers a callback function"""
-        self.__callbacks.append(callback)
+        self._callbacks.append(callback)
 
     def remove_callback(self, callback: Callable[[], None]) -> None:
         """Removes a callback function"""
-        self.__callbacks.remove(callback)
+        self._callbacks.remove(callback)
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/deviceStatus.py` & `py-miraie-ac-0.1.6/src/py_miraie_ac/deviceStatus.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac/enums.py` & `py-miraie-ac-0.1.6/src/py_miraie_ac/enums.py`

 * *Files identical despite different names*

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/PKG-INFO` & `py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-miraie-ac
-Version: 0.1.4
+Version: 0.1.6
 Summary: A package to control and read MirAIe Aircons by Panasonic
 Home-page: https://github.com/milothomas/py-miraie-ac
 Author: Milo Thomas
 Author-email: 20719501+milothomas@users.noreply.github.com
 Project-URL: Bug Tracker, https://github.com/milothomas/py-miraie-ac/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `py-miraie-ac-0.1.4/src/py_miraie_ac.egg-info/SOURCES.txt` & `py-miraie-ac-0.1.6/src/py_miraie_ac.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/py_miraie_ac/__init__.py
 src/py_miraie_ac/api.py
+src/py_miraie_ac/broker.py
 src/py_miraie_ac/constants.py
 src/py_miraie_ac/device.py
 src/py_miraie_ac/deviceStatus.py
 src/py_miraie_ac/enums.py
 src/py_miraie_ac/exceptions.py
 src/py_miraie_ac/home.py
 src/py_miraie_ac/test.py
```

