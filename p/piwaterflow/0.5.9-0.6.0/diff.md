# Comparing `tmp/piwaterflow-0.5.9.tar.gz` & `tmp/piwaterflow-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piwaterflow-0.5.9.tar", last modified: Thu Jun  1 12:02:41 2023, max compression
+gzip compressed data, was "piwaterflow-0.6.0.tar", last modified: Tue Jun 20 07:22:40 2023, max compression
```

## Comparing `piwaterflow-0.5.9.tar` & `piwaterflow-0.6.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.671330 piwaterflow-0.5.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/piwaterflow/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/config_waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/piwaterflow/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)    23595 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/piwaterflow/waterflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/piwaterflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 12:02:41.000000 piwaterflow-0.5.9/piwaterflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:02:41.671330 piwaterflow-0.5.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:41.667330 piwaterflow-0.5.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_000_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_001_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_002_reverse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_003_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 12:02:30.000000 piwaterflow-0.5.9/tests/test_004_events.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/piwaterflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/config_waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/piwaterflow/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24177 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/piwaterflow/waterflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/piwaterflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-20 07:22:40.000000 piwaterflow-0.6.0/piwaterflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:40.689402 piwaterflow-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_000_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_001_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_002_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_003_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-20 07:22:30.000000 piwaterflow-0.6.0/tests/test_004_events.py
```

### Comparing `piwaterflow-0.5.9/PKG-INFO` & `piwaterflow-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.9
+Version: 0.6.0
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.9/README.md` & `piwaterflow-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/piwaterflow/config-template.yml` & `piwaterflow-0.6.0/piwaterflow/config-template.yml`

 * *Files 16% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 external_ac_signal_pin: 10
 programs:
   - name: first
     enabled: true
     start_time: '09:51'
     valves:
         - name: main
-          time: 14
+          time: 14 # In minutes
         - name: grass
-          time: 2
+          time: 2 # In minutes
   - name: second
     enabled: true
     start_time: '19:04'
     valves:
         - name: main
-          time: 0
+          time: 0 # In minutes
         - name: grass
-          time: 2
+          time: 2 # In minutes
 valves:
   main:
     pin: 33
   grass:
     pin: 35
-max_valve_time: 10
+max_valve_time: 10 # In minutes
 humidity_threshold: 90
 metrics: false
-max_loop_time: 20
+max_loop_time: 20 # In minutes
 influxdbconn:
   host: xxxxxxx
   bucket: xxxxxxx
   user: xxxxxxx
   password: xxxxxxx
```

### Comparing `piwaterflow-0.5.9/piwaterflow/config_waterflow.py` & `piwaterflow-0.6.0/piwaterflow/config_waterflow.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/piwaterflow/tests/test_000.py` & `piwaterflow-0.6.0/piwaterflow/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/piwaterflow/waterflow.py` & `piwaterflow-0.6.0/piwaterflow/waterflow.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,23 +4,22 @@
 """
 import os
 import time
 import shutil
 from datetime import datetime, timedelta
 from pathlib import Path
 import json
-import traceback
+import logging
 
 try:
     from RPi import GPIO
 except (ModuleNotFoundError, ImportError, RuntimeError):
     from fake_rpigpio.RPi import GPIO
 
 from influxdb_wrapper import influxdb_factory
-from log_mgr import Logger
 from .config_waterflow import WaterflowConfig
 
 class Waterflow():
     """ Waterflow class that manages a loop system to activate/deactivate watering valves.
         This should run in a raspberry pi or similar, with watering valves connected through relays.
         At this moment it can support up to 2 valves, and 2 different programs alnog the day.
         Those programs/valves can be switched on/off in a forced way apart from the programs.
@@ -43,30 +42,29 @@
         if dry_run:
             self.homevar = os.path.join(self.homevar, 'dryrun')
             if os.path.exists(self.homevar): # Only one instance of waterflow can run at a time, so this is safe
                 shutil.rmtree(self.homevar)
             if not os.path.exists(self.homevar):
                 os.makedirs(self.homevar)
 
-        self.debuglogger = Logger(self.class_name(), 'waterflow', dry_run=dry_run)
-        self.userlogger = Logger(self.class_name(), 'loop', dry_run=dry_run)
+        self.logger = logging.getLogger()
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self.config = WaterflowConfig(package_name=self.class_name(),
                                       template_path=template_config_path,
                                       config_file_name="config.yml",
                                       dry_run=dry_run)
 
         self.events = self._read_events()
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
-        self.conn.openConn(self.config['influxdbconn'])
+        self.conn.open_conn(self.config['influxdbconn'])
 
     def __del__(self):
         if self.dry_run and os.path.exists(self.homevar):
             shutil.rmtree(self.homevar)
 
     @classmethod
     def class_name(cls):
@@ -236,30 +234,29 @@
             mod_time_since_epoc = os.path.getmtime(token_path)
             modification_time = datetime.fromtimestamp(mod_time_since_epoc).astimezone()
         else:
             modification_time = datetime.fromtimestamp(0) # Loop never run ok. Return oldest possible date
 
         return modification_time
 
-    def force(self, type_force: str, value: int):
+    def force(self, type_force: str, value: str):
         """ Set the force-flag, so that the loop will start the execution of a program or valve
             If a program is forced, it will execute with the times defined in the config
             If a valve is forced, it will start delivering water, until manually stopped
         Args:
             type_force (str): Can be "program" or "valve"
-            value (int): Index of the item to be forced
+            value (str): Name of the item to be forced
 
         Returns:
             bool: If forced correctly
         """
-        config = self.config.get_dict()
-        if (type_force == 'program' and 0 <= value < len(config['programs'])) or \
-           (type_force == 'valve' and 0 <= value < len(config['valves'])):
+        if (type_force == 'program' and self._get_program(value)) or \
+           (type_force == 'valve' and self._get_valve_data(value)):
             with open(self._get_homevar_path('force'), 'w', encoding="utf-8") as force_file:
-                force_file.write(f'{{"type":"{type_force}","value":{value}}}')
+                force_file.write(f'{{"type":"{type_force}","value":"{value}"}}')
                 return True
         else:
             return False
 
     def stop(self):
         """ Set the Stop-flag, so that the loop will stop the forced valve or program execution
         Returns:
@@ -310,16 +307,18 @@
         events_file_path = self._get_homevar_path('events')
         if os.path.exists(events_file_path):
             with open(events_file_path, 'r', encoding="utf-8") as events_file:
                 events = json.load(events_file)
         return events
 
     def _get_event_string(self, event: tuple):
-        if event[1] == 'ExecValve':
+        if event[1] == 'ExecProg':
             result = f'Executing program {event[2]}.'
+        elif event[1] == 'ExecValve':
+            result = f'Executing valve {event[2]}.'
         elif event[1] == 'InverterON':
             result = 'Inverter relay ON.'
         elif event[1] == 'InverterOFF':
             result = 'Inverter relay OFF.'
         elif event[1] == 'ValveON':
             result = f'Valve {event[2]} ON.'
         elif event[1] == 'ValveOFF':
@@ -337,14 +336,16 @@
             result = f'Forced program {event[2]} executing now.'
         elif event[1] == 'ForcedValve':
             result = f'Forced valve {event[2]} executing now.'
         elif event[1] == 'Stop':
             result = 'Activity stopped.'
         elif event[1] == 'Exception':
             result = f'Error looping: {event[2]}'
+        else:
+            result = f'Unknown event: {event[1]}, value {event[2]}'
 
         return f'{event[0]}:{result}'
 
     def get_log(self):
         """ Get the user log (not the debug log). This is the one the is shown in the wwwaterflow
         Returns:
             str: The whole user logs
@@ -358,17 +359,17 @@
         """ Sleep "time_sleep" time, but checks every 5 seconds if a stop has been requested
         Args:
             time_sleep (int): Number of seconds to sleep
         """
         time_count = 0
 
         # Clamp sleep time... as safety. Never let a valve stay ON more than this
-        if time_sleep > self.config['max_valve_time']:
-            time_sleep = self.config['max_valve_time']
-            self.debuglogger.info(f'Valve time clamped to {self.config["max_valve_time"]}')
+        if time_sleep > self.config['max_valve_time']*60:
+            time_sleep = self.config['max_valve_time']*60
+            self.logger.info('Valve time clamped to %s minutes.', self.config["max_valve_time"])
 
         while not self.stop_requested() and time_count < time_sleep:
             time_count = time_count + 5
             time.sleep(5)  # Every X seconds
 
     def _emit_action_metric(self, action, forced):
         if self.config['metrics'] and self.conn:
@@ -388,15 +389,17 @@
 
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
         self._add_event('InverterON', None)
         valve_pin = self.config['valves'][valve]['pin']
         GPIO.output(valve_pin, GPIO.HIGH)
         self._add_event('ValveON', valve)
 
-        self._sleep(self.config['max_valve_time']*60)
+        # If dry run, then we fast forward the sleep
+        if not self.dry_run:
+            self._sleep(self.config['max_valve_time']*60)
 
         GPIO.output(valve_pin, GPIO.LOW)
         self._add_event('ValveOFF', valve)
         # if inverter_enable: # If we dont have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.LOW)  # INVERTER always OFF after operations
         self._add_event('InverterOFF', None)
 
@@ -412,28 +415,40 @@
         #         return True
         #     else:
         #         return False
         # else:
         #    return False
         return False
 
+    def _get_program(self, program_name: str):
+        program = None
+        for program_it in self.config['programs']:
+            if program_it['name'] == program_name:
+                program = program_it
+                break
+        return program
+
+    def _get_valve_data(self, valve_name: str):
+        valve_data = None
+        for it_valve_name, it_valve_data in self.config['valves'].items():
+            if it_valve_name == valve_name:
+                valve_data = it_valve_data
+                break
+        return valve_data
+
     def _execute_program(self, program_name: str):
         """
         Works for regular programs, or forced ones (if program number is sent)
         """
         self._add_event('ExecProg', program_name)
         # inverter_enable =  not GPIO.input(self.config['external_ac_signal_pin'])
         # if inverter_enable: # If we don't have external 220V power input, then activate inverter
         GPIO.output(self.config['inverter_relay_pin'], GPIO.HIGH)
         self._add_event('InverterON', None)
-        program = None
-        for program_it in self.config['programs']:
-            if program_it['name'] == program_name:
-                program = program_it
-                break
+        program = self._get_program(program_name)
 
         for valve in program['valves']:
             if valve['time'] > 0 and not self.stop_requested():
                 valve_pin = self.config['valves'][valve['name']]['pin']
                 GPIO.output(valve_pin, GPIO.HIGH)
                 self._add_event('ValveON', valve['name'])
 
@@ -460,42 +475,44 @@
         if not self.events or self.events[-1][1] != 'LastProg' or self.events[-1][2] != last_event_date:
             self._add_event('LastProg', last_event_date)
 
     def _execute_forced(self, forced_info: dict):
         forced_type = forced_info.get("type")
         forced_value = forced_info.get("value")
         if forced_type == "program":
+            self.logger.info("Executing forced program: %s", forced_value)
             self._add_event('ForcedProg', forced_value)
             # ------------------------
             self._emit_action_metric(f'prog{forced_value}', True)
             self._execute_program(forced_value)
             self._write_last_program_time(self.curr_time)
         elif forced_type == "valve":
+            self.logger.info("Executing forced valve: %s", forced_value)
             self._add_event('ForcedValve', forced_value)
             # ------------------------
             self._emit_action_metric(f'valve{forced_value}', True)
             self._execute_valve(forced_value)
 
     def _check_and_execute_program(self):
         last_program_time = self._read_last_program_time(default=self.curr_time)
         new_next_program, new_program_name = self._recalc_next_program(last_program_time)
         if new_next_program:
             # ------------------------
             time_reached = self.curr_time >= new_next_program
-            time_threshold_exceeded = self.curr_time > (new_next_program + timedelta(minutes=self.config['max_loop_time']))
+            threshold_exceeded = self.curr_time > (new_next_program + timedelta(minutes=self.config['max_loop_time']))
             skip_program = self._skip_program()
             # If we have reached the time of the new_program_time, BUT not by more than 10 minutes...
-            if time_reached and not time_threshold_exceeded and not skip_program:
+            if time_reached and not threshold_exceeded and not skip_program:
                 self._emit_action_metric(f'prog_{new_program_name}', False)
                 self._execute_program(new_program_name)
                 program_executed = True
             else:
                 program_executed = False
 
-            if program_executed or skip_program or time_threshold_exceeded:
+            if program_executed or skip_program or threshold_exceeded:
                 self._write_last_program_time(self.curr_time)
 
     def loop(self, date_now: datetime = None):
         """ Loop executed every x minutes... in crontab for example.
         Args:
             date_now (datetime): Naive date to consider the execution of the loop. 
                                  Normally used only for debuggin/unittesting
@@ -505,23 +522,23 @@
                 if date_now:
                     self.curr_time = date_now.astimezone() # Make aware
                 else:
                     self.curr_time = datetime.now().astimezone()
                 forced_info = self.get_forced_info()
 
                 if not self.stop_requested():
-                    self.debuglogger.info('Looping...')
+                    self.logger.info('Looping...')
                     self._setup_gpio(self.config['valves'])
 
                     if forced_info:
                         self._execute_forced(forced_info)
                     else:
                         self._check_and_execute_program()
                 else:
-                    self.debuglogger.info('Loop skipped (Stop request).')
+                    self.logger.info('Loop skipped (Stop request).')
                     self._add_event('Stop', None)
                     self._emit_action_metric('Stop', True)
                     self.stop_remove()
 
                 if forced_info:
                     # Remove force token file
                     os.remove(os.path.join(self.homevar, 'force'))
@@ -530,15 +547,15 @@
                 self._log_next_program_time()
 
                 # Updates "modified" time AT THE END, so that we can keep track about waterflow looping SUCCESFULLY.
                 token_path = os.path.join(self.homevar, 'token')
                 Path(token_path).touch()
 
             except Exception as ex:
-                self.debuglogger.error(f'Exception looping: {str(ex)} | Stack: {traceback.format_exc()}')
+                self.logger.error('Exception looping: %s', str(ex), exc_info=True)
                 self._add_event('Exception', str(ex))
                 raise RuntimeError(ex) from ex
             finally:
                 GPIO.cleanup()
                 self.release_lock()
         else:
-            self.debuglogger.error('Loop executed while locked by previous execution.')
+            self.logger.error('Loop executed while locked by previous execution.')
```

### Comparing `piwaterflow-0.5.9/piwaterflow.egg-info/PKG-INFO` & `piwaterflow-0.6.0/piwaterflow.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piwaterflow
-Version: 0.5.9
+Version: 0.6.0
 Summary: Raspberry Pi Waterflow resilient system
 Home-page: https://github.com/Phornee/piwaterflow
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # PiWaterflow
         This is a resilient watering system, executed in a Raspberry Pi to control irrigation valves using relays.
```

### Comparing `piwaterflow-0.5.9/piwaterflow.egg-info/SOURCES.txt` & `piwaterflow-0.6.0/piwaterflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/setup.py` & `piwaterflow-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="piwaterflow",
-    version="0.5.9",
+    version="0.6.0",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Waterflow resilient system",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/piwaterflow",
     packages=setuptools.find_packages(),
@@ -20,15 +20,15 @@
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation",
     ],
     install_requires=[
-        'log_mgr>=0.0.2',
+        'log_mgr>=0.1.1',
         'config_yml>=0.3.1',
         'RPi.GPIO>=0.7.0',
         'fake-rpigpio>=0.1.1',
-        'influxdb_wrapper>=0.0.4'
+        'influxdb_wrapper>=0.0.5'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `piwaterflow-0.5.9/tests/test_001_forward.py` & `piwaterflow-0.6.0/tests/test_001_forward.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/tests/test_002_reverse.py` & `piwaterflow-0.6.0/tests/test_002_reverse.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/tests/test_003_lock.py` & `piwaterflow-0.6.0/tests/test_003_lock.py`

 * *Files identical despite different names*

### Comparing `piwaterflow-0.5.9/tests/test_004_events.py` & `piwaterflow-0.6.0/tests/test_004_events.py`

 * *Files identical despite different names*

