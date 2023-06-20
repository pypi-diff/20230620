# Comparing `tmp/dl_myo-1.0.0.tar.gz` & `tmp/dl_myo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dl_myo-1.0.0.tar", max compression
+gzip compressed data, was "dl_myo-1.0.1.tar", max compression
```

## Comparing `dl_myo-1.0.0.tar` & `dl_myo-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    35123 2023-06-19 21:19:24.631658 dl_myo-1.0.0/LICENSE
--rw-r--r--   0        0        0     3837 2023-06-19 21:19:24.631658 dl_myo-1.0.0/README.md
--rw-r--r--   0        0        0      749 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/__init__.py
--rw-r--r--   0        0        0    10771 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/client.py
--rw-r--r--   0        0        0     3293 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/commands.py
--rw-r--r--   0        0        0      503 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/constants.py
--rw-r--r--   0        0        0     4331 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/core.py
--rw-r--r--   0        0        0     5802 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/profile.py
--rw-r--r--   0        0        0     9161 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/types.py
--rw-r--r--   0        0        0       22 2023-06-19 21:19:24.631658 dl_myo-1.0.0/myo/version.py
--rw-r--r--   0        0        0     3271 2023-06-19 21:19:41.955942 dl_myo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 dl_myo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35123 2023-06-20 10:22:54.946067 dl_myo-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3837 2023-06-20 10:22:54.946067 dl_myo-1.0.1/README.md
+-rw-r--r--   0        0        0      749 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/__init__.py
+-rw-r--r--   0        0        0    10855 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/client.py
+-rw-r--r--   0        0        0     3293 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/commands.py
+-rw-r--r--   0        0        0      503 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/constants.py
+-rw-r--r--   0        0        0     4331 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/core.py
+-rw-r--r--   0        0        0     5802 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/profile.py
+-rw-r--r--   0        0        0     9161 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/types.py
+-rw-r--r--   0        0        0       22 2023-06-20 10:22:54.946067 dl_myo-1.0.1/myo/version.py
+-rw-r--r--   0        0        0     3271 2023-06-20 10:23:15.326388 dl_myo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4462 1970-01-01 00:00:00.000000 dl_myo-1.0.1/PKG-INFO
```

### Comparing `dl_myo-1.0.0/LICENSE` & `dl_myo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/README.md` & `dl_myo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/myo/__init__.py` & `dl_myo-1.0.1/myo/__init__.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/myo/client.py` & `dl_myo-1.0.1/myo/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,26 +94,26 @@
             logger.error("connection is already closed")
 
         # disconnect from the device
         await self._client.disconnect()
         self._client = None
         logger.info(f"disconnected from {self.device.name}")
 
-    def emg_data_aggregate(self, handle, emg_data: EMGData):
+    async def emg_data_aggregate(self, handle, emg_data: EMGData):
         """
         <> aggregate the raw EMG data channels
         """
         if handle in [
             Handle.EMG0_DATA,
             Handle.EMG1_DATA,
             Handle.EMG2_DATA,
             Handle.EMG3_DATA,
         ]:
-            self.on_emg_data(emg_data.sample1)
-            self.on_emg_data(emg_data.sample2)
+            await self.on_emg_data(emg_data.sample1)
+            await self.on_emg_data(emg_data.sample2)
 
     async def get_services(self, indent=1) -> str:
         """
         <> fetch available services as dict
         """
         sd = {}
         for service in self._client.services:  # BleakGATTServiceCollection
@@ -142,44 +142,44 @@
         """
         LED Command
         args:
             - color: myo.constants.RGB_*
         """
         await self.m.led(self._client, color, color)
 
-    def on_classifier_event(self, ce: ClassifierEvent):
+    async def on_classifier_event(self, ce: ClassifierEvent):
         raise NotImplementedError()
 
-    def on_emg_data(self, emg):  # data: list of 8 8-bit unsigned short
+    async def on_emg_data(self, emg):  # data: list of 8 8-bit unsigned short
         raise NotImplementedError()
 
-    def on_fv_data(self, fvd: FVData):
+    async def on_fv_data(self, fvd: FVData):
         raise NotImplementedError()
 
-    def on_imu_data(self, imu: IMUData):
+    async def on_imu_data(self, imu: IMUData):
         raise NotImplementedError()
 
-    def on_motion_event(self, me: MotionEvent):
+    async def on_motion_event(self, me: MotionEvent):
         raise NotImplementedError()
 
-    def notify_callback(self, sender: BleakGATTCharacteristic, data: bytearray):
+    async def notify_callback(self, sender: BleakGATTCharacteristic, data: bytearray):
         """
         <> invoke the on_* callbacks
         """
         handle = Handle(sender.handle)
         if handle == Handle.CLASSIFIER_EVENT:
-            self.on_classifier_event(ClassifierEvent(data))
+            await self.on_classifier_event(ClassifierEvent(data))
         elif handle == Handle.FV_DATA:
-            self.on_fv_data(FVData(data))
+            await self.on_fv_data(FVData(data))
         elif handle == Handle.IMU_DATA:
-            self.on_imu_data(IMUData(data))
+            await self.on_imu_data(IMUData(data))
         elif handle == Handle.MOTION_EVENT:
-            self.on_motion_event(MotionEvent(data))
+            await self.on_motion_event(MotionEvent(data))
         else:  # on EMG[0-3]_DATA handle
-            self.emg_data_aggregate(handle, EMGData(data))
+            await self.emg_data_aggregate(handle, EMGData(data))
 
     async def set_mode(self, emg_mode, imu_mode, classifier_mode):
         """
         Set Mode Command
             - configures EMG, IMU, and Classifier modes
         """
         await self.m.set_mode(self._client, emg_mode, imu_mode, classifier_mode)
```

### Comparing `dl_myo-1.0.0/myo/commands.py` & `dl_myo-1.0.1/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/myo/core.py` & `dl_myo-1.0.1/myo/core.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/myo/profile.py` & `dl_myo-1.0.1/myo/profile.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/myo/types.py` & `dl_myo-1.0.1/myo/types.py`

 * *Files identical despite different names*

### Comparing `dl_myo-1.0.0/pyproject.toml` & `dl_myo-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
   "no cov",
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
 ]
 
 [tool.poetry]
 name = "dl-myo"
-version = "1.0.0"
+version = "1.0.1"
 description = "Yet another MyoConnect alternative without dongles"
 authors = ["Iori Mizutani <iomz@sazanka.io>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "myo"}]
 
 [tool.poetry.dependencies]
```

### Comparing `dl_myo-1.0.0/PKG-INFO` & `dl_myo-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Yet another MyoConnect alternative without dongles
 License: GPLv3
 Author: Iori Mizutani
 Author-email: iomz@sazanka.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

