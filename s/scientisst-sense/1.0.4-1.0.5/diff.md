# Comparing `tmp/scientisst-sense-1.0.4.tar.gz` & `tmp/scientisst-sense-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scientisst-sense-1.0.4.tar", last modified: Wed Aug 24 10:51:52 2022, max compression
+gzip compressed data, was "scientisst-sense-1.0.5.tar", last modified: Tue Jun 20 09:57:32 2023, max compression
```

## Comparing `scientisst-sense-1.0.4.tar` & `scientisst-sense-1.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:52.947187 scientisst-sense-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-08-24 10:51:52.947187 scientisst-sense-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:52.943187 scientisst-sense-1.0.4/scientisst/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      361 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:52.943187 scientisst-sense-1.0.4/scientisst/esp_adc/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/esp_adc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/esp_adc/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     4129 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/esp_adc/esp_adc.py
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/esp_adc/lut_adc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2116 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/frame.py
--rw-r--r--   0 runner    (1001) docker     (121)    21075 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/scientisst.py
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/scientisst/state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:52.947187 scientisst-sense-1.0.4/scientisst_sense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4132 2022-08-24 10:51:52.000000 scientisst-sense-1.0.4/scientisst_sense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      730 2022-08-24 10:51:52.000000 scientisst-sense-1.0.4/scientisst_sense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-24 10:51:52.000000 scientisst-sense-1.0.4/scientisst_sense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-08-24 10:51:52.000000 scientisst-sense-1.0.4/scientisst_sense.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-08-24 10:51:52.000000 scientisst-sense-1.0.4/scientisst_sense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-08-24 10:51:52.000000 scientisst-sense-1.0.4/scientisst_sense.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     3339 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:52.947187 scientisst-sense-1.0.4/sense_src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3708 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/arg_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     1145 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/custom_script.py
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/device_picker.py
--rw-r--r--   0 runner    (1001) docker     (121)     3553 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/file_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1176 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/stream_lsl.py
--rw-r--r--   0 runner    (1001) docker     (121)      748 2022-08-24 10:51:44.000000 scientisst-sense-1.0.4/sense_src/thread_builder.py
--rw-r--r--   0 runner    (1001) docker     (121)      909 2022-08-24 10:51:52.947187 scientisst-sense-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/scientisst/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/scientisst/esp_adc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/esp_adc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/esp_adc/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/esp_adc/esp_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/esp_adc/lut_adc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22230 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/scientisst.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/scientisst/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/scientisst_sense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4132 2023-06-20 09:57:32.000000 scientisst-sense-1.0.5/scientisst_sense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-20 09:57:32.000000 scientisst-sense-1.0.5/scientisst_sense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 09:57:32.000000 scientisst-sense-1.0.5/scientisst_sense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-20 09:57:32.000000 scientisst-sense-1.0.5/scientisst_sense.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-20 09:57:32.000000 scientisst-sense-1.0.5/scientisst_sense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 09:57:32.000000 scientisst-sense-1.0.5/scientisst_sense.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3339 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/sense_src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/arg_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/custom_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/device_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3553 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/file_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/stream_lsl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-20 09:57:22.000000 scientisst-sense-1.0.5/sense_src/thread_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-06-20 09:57:32.166280 scientisst-sense-1.0.5/setup.cfg
```

### Comparing `scientisst-sense-1.0.4/LICENSE` & `scientisst-sense-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/PKG-INFO` & `scientisst-sense-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientisst-sense
-Version: 1.0.4
+Version: 1.0.5
 Summary: The ScientISST SENSE Python API
 Home-page: https://github.com/scientisst/scientisst-sense-api-python
 Author: ScientISST
 Author-email: developer@scientisst.com
 Project-URL: Bug Tracker, https://github.com/scientisst/scientisst-sense-api-python/issues
 Project-URL: Documentation, https://scientisst.github.io/scientisst-sense-api-python
 Classifier: Programming Language :: Python :: 3
@@ -132,15 +132,15 @@
 ```
 
 ## Example
 
 Example usage to acquire AI1 at 10Hz sample rate (Linux):
 
 ```
-python3 sense.py -f 10 -c 1 08:3A:F2:49:AC:D2 -o output.csv
+python3 sense.py -f 10 -c 1 -o output.csv 08:3A:F2:49:AC:D2
 ```
 
 
 ## Plot
 
 Dependencies:
 - pandas
```

### Comparing `scientisst-sense-1.0.4/README.md` & `scientisst-sense-1.0.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 ```
 
 ## Example
 
 Example usage to acquire AI1 at 10Hz sample rate (Linux):
 
 ```
-python3 sense.py -f 10 -c 1 08:3A:F2:49:AC:D2 -o output.csv
+python3 sense.py -f 10 -c 1 -o output.csv 08:3A:F2:49:AC:D2
 ```
 
 
 ## Plot
 
 Dependencies:
 - pandas
```

### Comparing `scientisst-sense-1.0.4/scientisst/esp_adc/constants.py` & `scientisst-sense-1.0.5/scientisst/esp_adc/constants.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/scientisst/esp_adc/esp_adc.py` & `scientisst-sense-1.0.5/scientisst/esp_adc/esp_adc.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/scientisst/esp_adc/lut_adc.py` & `scientisst-sense-1.0.5/scientisst/esp_adc/lut_adc.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/scientisst/exceptions.py` & `scientisst-sense-1.0.5/scientisst/exceptions.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/scientisst/frame.py` & `scientisst-sense-1.0.5/scientisst/frame.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/scientisst/scientisst.py` & `scientisst-sense-1.0.5/scientisst/scientisst.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import sys
 
 
 # if sys.platform == "linux":
 import socket
+import select
 
 # else:
 import serial
 
 import time
 import re
 from math import log2
@@ -60,14 +61,22 @@
         ):
             raise InvalidParameterError()
 
         self.com_mode = com_mode
         self.address = address
         self.serial_speed = serial_speed
         self.__log = log
+        
+        self.__serial = None
+        self.__socket = None
+        self.__num_chs = 0
+        self.__api_mode = 1
+        self.__sample_rate = None
+        self.__chs = [None] * 8
+        self.__log = False
 
         # Setup socket in function of com_mode argument
         self.__setupSocket()
 
         # try to connect to board
         while True:
             try:
@@ -247,31 +256,31 @@
         start = 0
         for it in range(self.__num_frames):
             bf = result[start : start + self.__packet_size]
             mid_frame_flag = 0
 
             #  if CRC check failed, try to resynchronize with the next valid frame
             while not self.__checkCRC4(bf, self.__packet_size):
-                sys.stderr.write("Error checking CRC4")
+                sys.stderr.write("Error checking CRC4\n")
                 #  checking with one new byte at a time
                 result_tmp = list(self.__recv(1))
                 if len(result_tmp) != 1:
                     raise ContactingDeviceError()
 
                 result += result_tmp
                 start += 1
                 bf = result[start : start + self.__packet_size]
 
             f = Frame(self.__num_chs)
             frames.append(f)
             if self.__api_mode == API_MODE_SCIENTISST:
                 # Get seq number and IO states
-                f.seq = bf[-1] >> 4
+                f.seq = bf[-2] >> 4 | bf[-1] << 4
                 for i in range(4):
-                    f.digital[i] = 0 if (bf[-2] & (0x80 >> i)) == 0 else 1
+                    f.digital[i] = 0 if (bf[-3] & (0x80 >> i)) == 0 else 1
 
                 # Get channel values
                 byte_it = 0
                 for i in range(self.__num_chs):
                     index = self.__num_chs - 1 - i
                     curr_ch = self.__chs[index]
 
@@ -280,14 +289,17 @@
                         f.a[index] = (
                             int.from_bytes(
                                 bf[byte_it : byte_it + 4], byteorder="little"
                             )
                             & 0xFFFFFF
                         )
                         byte_it += 3
+                        if convert:
+                            f.mv[index] = ((f.a[index]) * (3.3*2) / (pow(2, 24) - 1))*1000
+                            f.mv[index] = round(f.mv[index], 3)
 
                     # If it's an AI channel
                     else:
                         if not mid_frame_flag:
                             f.a[index] = (
                                 int.from_bytes(
                                     bf[byte_it : byte_it + 2], byteorder="little"
@@ -483,14 +495,15 @@
                 ):
                     raise InvalidAddressError()
 
                 self.__socket = socket.socket(
                     socket.AF_BLUETOOTH, socket.SOCK_STREAM, socket.BTPROTO_RFCOMM
                 )
                 self.__socket.connect((self.address, 1))
+                self.__socket.settimeout(TIMEOUT_IN_SECONDS)
             else:
                 self.__serial = serial.Serial(
                     self.address, self.serial_speed, timeout=TIMEOUT_IN_SECONDS
                 )
         elif self.com_mode == COM_MODE_TCP_SERVER:
             if not self.address.isdigit():
                 raise InvalidAddressError()
@@ -519,16 +532,14 @@
 
             self.__socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.__socket.connect(("scientisst.local", port))
 
         else:
             raise InvalidParameterError
 
-        self.__socket.settimeout(TIMEOUT_IN_SECONDS)
-
     def __getPacketSize(self):
         packet_size = 0
 
         if self.__api_mode == API_MODE_SCIENTISST:
             num_intern_active_chs = 0
             num_extern_active_chs = 0
 
@@ -548,15 +559,15 @@
             if not (num_intern_active_chs % 2):  # If it's an even number
                 packet_size += (num_intern_active_chs * 12) / 8
             else:
                 packet_size += (
                     (num_intern_active_chs * 12) - 4
                 ) / 8  # -4 because 4 bits can go in the I/0 byte
             # for the I/Os and seq+crc bytes
-            packet_size += 2
+            packet_size += 3
 
         else:
             raise NotSupportedError()
 
         return int(packet_size)
 
     def __changeAPI(self, api):
@@ -572,24 +583,28 @@
         api |= 0b11
 
         self.__send(api)
 
     def __checkCRC4(self, data, length):
         CRC4tab = [0, 3, 6, 5, 12, 15, 10, 9, 11, 8, 13, 14, 7, 4, 1, 2]
         crc = 0
-        for i in range(length - 1):
+        for i in range(length - 2):
             b = data[i]
             crc = CRC4tab[crc] ^ (b >> 4)
             crc = CRC4tab[crc] ^ (b & 0x0F)
 
-        # CRC for last byte
+        # CRC for seq
+        crc = CRC4tab[crc] ^ (data[-2] >> 4)        #First 4 bits
+        #Last 8 bits of seq
         crc = CRC4tab[crc] ^ (data[-1] >> 4)
+        crc = CRC4tab[crc] ^ (data[-1] & 0x0F)
+
         crc = CRC4tab[crc]
 
-        return crc == (data[-1] & 0x0F)
+        return crc == (data[-2] & 0x0F)
 
     def __send(self, command, nrOfBytes=0):
         """
         Send data
         """
 
         if nrOfBytes <= 4:
@@ -624,20 +639,30 @@
         # else:
         # raise ContactingDeviceError()
 
     def __recv(self, nrOfBytes, waitall_flag=True):
         """
         Receive data
         """
-        result = None
+        result = b""
         if self.__socket:
-            if waitall_flag:
-                result = self.__socket.recv(nrOfBytes, socket.MSG_WAITALL)
-            else:
-                result = self.__socket.recv(nrOfBytes)
+            # We have to use a select here with a single socket because we can't apply a timeout in any other way
+            ready = select.select([self.__socket], [], [], 5)  # 10 seconds timeout
+            if ready[0]:
+                if waitall_flag:
+                    remaining = nrOfBytes
+                    while remaining > 0:
+                        ready = select.select([self.__socket], [], [], 10)
+                        if not ready[0]:
+                            raise ContactingDeviceError()
+                        temp = self.__socket.recv(remaining)
+                        result += temp
+                        remaining = nrOfBytes - len(result)
+                else:
+                    result = self.__socket.recv(nrOfBytes)
         elif self.__serial:
             result = self.__serial.read(nrOfBytes)
         else:
             raise InvalidParameterError()
         if self.__log:
             if nrOfBytes > 1:
                 sys.stdout.write(
```

### Comparing `scientisst-sense-1.0.4/scientisst_sense.egg-info/PKG-INFO` & `scientisst-sense-1.0.5/scientisst_sense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scientisst-sense
-Version: 1.0.4
+Version: 1.0.5
 Summary: The ScientISST SENSE Python API
 Home-page: https://github.com/scientisst/scientisst-sense-api-python
 Author: ScientISST
 Author-email: developer@scientisst.com
 Project-URL: Bug Tracker, https://github.com/scientisst/scientisst-sense-api-python/issues
 Project-URL: Documentation, https://scientisst.github.io/scientisst-sense-api-python
 Classifier: Programming Language :: Python :: 3
@@ -132,15 +132,15 @@
 ```
 
 ## Example
 
 Example usage to acquire AI1 at 10Hz sample rate (Linux):
 
 ```
-python3 sense.py -f 10 -c 1 08:3A:F2:49:AC:D2 -o output.csv
+python3 sense.py -f 10 -c 1 -o output.csv 08:3A:F2:49:AC:D2
 ```
 
 
 ## Plot
 
 Dependencies:
 - pandas
```

### Comparing `scientisst-sense-1.0.4/scientisst_sense.egg-info/SOURCES.txt` & `scientisst-sense-1.0.5/scientisst_sense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense.py` & `scientisst-sense-1.0.5/sense.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense_src/arg_parser.py` & `scientisst-sense-1.0.5/sense_src/arg_parser.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense_src/custom_script.py` & `scientisst-sense-1.0.5/sense_src/custom_script.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense_src/device_picker.py` & `scientisst-sense-1.0.5/sense_src/device_picker.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense_src/file_writer.py` & `scientisst-sense-1.0.5/sense_src/file_writer.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense_src/stream_lsl.py` & `scientisst-sense-1.0.5/sense_src/stream_lsl.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/sense_src/thread_builder.py` & `scientisst-sense-1.0.5/sense_src/thread_builder.py`

 * *Files identical despite different names*

### Comparing `scientisst-sense-1.0.4/setup.cfg` & `scientisst-sense-1.0.5/setup.cfg`

 * *Files identical despite different names*

