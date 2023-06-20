# Comparing `tmp/esp-idf-monitor-1.1.0.tar.gz` & `tmp/esp-idf-monitor-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-cmnzt9cx/esp-idf-monitor-1.1.0.tar", last modified: Thu Jun 15 14:48:47 2023, max compression
+gzip compressed data, was "/home/runner/work/esp-idf-monitor/esp-idf-monitor/dist/.tmp-rhl95jpb/esp-idf-monitor-1.1.1.tar", last modified: Tue Jun 20 14:17:18 2023, max compression
```

## Comparing `esp-idf-monitor-1.1.0.tar` & `esp-idf-monitor-1.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/ansi_color_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/argument_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/chip_specific_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/coredump.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/gdbhelper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/line_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/output_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/pc_address_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/rom_elf_getter.py
--rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/stoppable_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/base/web_socket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/gdb_panic_server.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17723 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/esp_idf_monitor/idf_monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 14:48:47.000000 esp-idf-monitor-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-15 14:48:23.000000 esp-idf-monitor-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6115 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/ansi_color_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/argument_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/chip_specific_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/coredump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5718 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/gdbhelper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/line_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/output_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/pc_address_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/rom_elf_getter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12976 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4999 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/stoppable_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3403 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/base/web_socket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11375 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/gdb_panic_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17723 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/esp_idf_monitor/idf_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 14:17:18.000000 esp-idf-monitor-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-06-20 14:17:02.000000 esp-idf-monitor-1.1.1/setup.py
```

### Comparing `esp-idf-monitor-1.1.0/LICENSE` & `esp-idf-monitor-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/PKG-INFO` & `esp-idf-monitor-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.1.0
+Version: 1.1.1
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.1.0/README.md` & `esp-idf-monitor-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/ansi_color_converter.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/ansi_color_converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -58,33 +58,40 @@
             output.write(b'')  # type: ignore
         except Exception:
             self.decode_output = True
         else:
             self.decode_output = False
         self.handle = GetStdHandle(STD_ERROR_HANDLE if self.output == sys.stderr else STD_OUTPUT_HANDLE)
         self.matched = b''
+        self.decode_buffer = b''
         self.force_color = force_color  # always print ANSI for colors if true
 
     def _output_write(self, data):  # type: (Union[str, bytes]) -> None
         try:
             if self.decode_output:
+                data = self.decode_buffer + data  # type: ignore
                 self.output.write(data.decode())  # type: ignore
+                self.decode_buffer = b''
             else:
                 self.output.write(data)  # type: ignore
         except (IOError, OSError):
             # Windows 10 bug since the Fall Creators Update, sometimes writing to console randomly throws
             # an exception (however, the character is still written to the screen)
             # Ref https://github.com/espressif/esp-idf/issues/1163
             #
             # Also possible for Windows to throw an OSError error if the data is invalid for the console
             # (garbage bytes, etc)
             pass
         except UnicodeDecodeError:
-            # In case of double byte Unicode characters display '?'
-            self.output.write('?')  # type: ignore
+            self.decode_buffer += data  # type: ignore
+            if len(self.decode_buffer) > 4:
+                # Multi-byte character contain up to 4 bytes and if buffer have more then 4 bytes
+                # and still can not decode it we can just ignore some bytes
+                self.output.write(self.decode_buffer.decode(errors='replace'))  # type: ignore
+                self.decode_buffer = b''
 
     def write(self, data):  # type: ignore
         if isinstance(data, bytes):
             data = bytearray(data)
         else:
             data = bytearray(data, 'utf-8')
```

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/argument_parser.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/argument_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/chip_specific_config.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/chip_specific_config.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_parser.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_parser.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/console_reader.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/console_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/constants.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/constants.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/coredump.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/coredump.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/gdbhelper.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/gdbhelper.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/line_matcher.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/line_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/logger.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/logger.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/output_helpers.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/output_helpers.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/pc_address_matcher.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/pc_address_matcher.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/rom_elf_getter.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/rom_elf_getter.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_handler.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_handler.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/serial_reader.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/serial_reader.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/stoppable_thread.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/base/web_socket_client.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/base/web_socket_client.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/gdb_panic_server.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/gdb_panic_server.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor/idf_monitor.py` & `esp-idf-monitor-1.1.1/esp_idf_monitor/idf_monitor.py`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/PKG-INFO` & `esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-idf-monitor
-Version: 1.1.0
+Version: 1.1.1
 Summary: Serial monitor for esp-idf
 Home-page: https://github.com/espressif/esp-idf-monitor
 Author: Espressif Systems
 Author-email: 
 Keywords: espressif,embedded,monitor,serial
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `esp-idf-monitor-1.1.0/esp_idf_monitor.egg-info/SOURCES.txt` & `esp-idf-monitor-1.1.1/esp_idf_monitor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-idf-monitor-1.1.0/setup.py` & `esp-idf-monitor-1.1.1/setup.py`

 * *Files identical despite different names*

