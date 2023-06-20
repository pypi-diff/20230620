# Comparing `tmp/CommandAlarm-0.2.4.tar.gz` & `tmp/CommandAlarm-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CommandAlarm-0.2.4.tar", last modified: Sun Jun 11 21:07:37 2023, max compression
+gzip compressed data, was "CommandAlarm-0.2.5.tar", last modified: Tue Jun 20 20:44:36 2023, max compression
```

## Comparing `CommandAlarm-0.2.4.tar` & `CommandAlarm-0.2.5.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-11 21:07:37.733948 CommandAlarm-0.2.4/
--rw-r--r--   0 testuser  (1002) testuser  (1003)      296 2023-06-11 20:49:39.000000 CommandAlarm-0.2.4/CHANGELOG.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-11 21:07:37.733948 CommandAlarm-0.2.4/CommandAlarm.egg-info/
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2750 2023-06-11 21:07:37.000000 CommandAlarm-0.2.4/CommandAlarm.egg-info/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)      288 2023-06-11 21:07:37.000000 CommandAlarm-0.2.4/CommandAlarm.egg-info/SOURCES.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-11 21:07:37.000000 CommandAlarm-0.2.4/CommandAlarm.egg-info/dependency_links.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-11 21:07:37.000000 CommandAlarm-0.2.4/CommandAlarm.egg-info/entry_points.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-11 21:07:37.000000 CommandAlarm-0.2.4/CommandAlarm.egg-info/top_level.txt
--rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2023-06-09 19:46:38.000000 CommandAlarm-0.2.4/LICENSE
--rw-r--r--   0 testuser  (1002) testuser  (1003)       29 2023-06-09 19:46:38.000000 CommandAlarm-0.2.4/MANIFEST.in
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2750 2023-06-11 21:07:37.733948 CommandAlarm-0.2.4/PKG-INFO
--rw-r--r--   0 testuser  (1002) testuser  (1003)     2227 2023-06-11 19:30:33.000000 CommandAlarm-0.2.4/README.md
-drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-11 21:07:37.733948 CommandAlarm-0.2.4/commandalarm/
--rw-r--r--   0 testuser  (1002) testuser  (1003)       46 2023-06-11 18:35:05.000000 CommandAlarm-0.2.4/commandalarm/__init__.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)     7219 2023-06-09 22:16:23.000000 CommandAlarm-0.2.4/commandalarm/commandalarm.py
--rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-11 21:07:37.733948 CommandAlarm-0.2.4/setup.cfg
--rw-r--r--   0 testuser  (1002) testuser  (1003)      863 2023-06-11 18:34:49.000000 CommandAlarm-0.2.4/setup.py
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 20:44:36.729932 CommandAlarm-0.2.5/
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 20:44:36.709932 CommandAlarm-0.2.5/CommandAlarm.egg-info/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     3239 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      263 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/SOURCES.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)        1 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/dependency_links.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       64 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/entry_points.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       13 2023-06-20 20:44:36.000000 CommandAlarm-0.2.5/CommandAlarm.egg-info/top_level.txt
+-rw-r--r--   0 testuser  (1002) testuser  (1003)    35149 2023-06-15 23:25:58.000000 CommandAlarm-0.2.5/LICENSE
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     3239 2023-06-20 20:44:36.729932 CommandAlarm-0.2.5/PKG-INFO
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     2347 2023-06-20 07:40:35.000000 CommandAlarm-0.2.5/README.md
+drwxr-xr-x   0 testuser  (1002) testuser  (1003)        0 2023-06-20 20:44:36.721932 CommandAlarm-0.2.5/commandalarm/
+-rw-r--r--   0 testuser  (1002) testuser  (1003)      767 2023-06-20 19:16:56.000000 CommandAlarm-0.2.5/commandalarm/__init__.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     7352 2023-06-20 19:17:37.000000 CommandAlarm-0.2.5/commandalarm/commandalarm.py
+-rw-r--r--   0 testuser  (1002) testuser  (1003)       38 2023-06-20 20:44:36.729932 CommandAlarm-0.2.5/setup.cfg
+-rw-r--r--   0 testuser  (1002) testuser  (1003)     1308 2023-06-20 19:59:54.000000 CommandAlarm-0.2.5/setup.py
```

### Comparing `CommandAlarm-0.2.4/CommandAlarm.egg-info/PKG-INFO` & `CommandAlarm-0.2.5/CommandAlarm.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+License: GPLv3
+Project-URL: Bug Reports, https://github.com/alofgren/commandalarm/issues
+Project-URL: Source, https://github.com/alofgren/commandalarm
+Keywords: alarm,command,command-line,tool,timer,commandalarm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CommandAlarm
 
 CommandAlarm is a simple command line program that allows users to set an alarm with a custom command. 
@@ -30,50 +39,55 @@
 git clone https://github.com/alofgren/commandalarm.git
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
-```bash
+```
 usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
   command               the command to run
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
-  -s, --shell           run command with shell
+  -s, --shell           run command in a shell
   -n, --no-check        don't check the command return code
   -t TIMEOUT, --timeout TIMEOUT
                         timeout in seconds for the command to complete
 ```
 
 ## Examples
 
-To set an alarm for 2:00 PM on Tuesday, and play a sound when the alarm goes off:
+To set an alarm for 2:00 PM and play a sound when the alarm goes off:
 ```bash
-commandalarm -d 2 14:00:00 aplay alarm_sound.wav
+commandalarm 14:00:00 aplay alarm_sound.wav
 ```
 
-To set an alarm for 10:00 PM to run a command with shell and repeat indefinitely: 
+To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
 ```bash
-commandalarm 22:00:00 -r -s 'echo "Hello, world!"'
+commandalarm 09:15:00 --day 3 --timeout 30 python3 script.py
 ```
 
-To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
+To run a command in a shell, use the -s or --shell option:
+```bash
+commandalarm 16:00:00 --shell 'ENV_VAR="I am running in a shell"; echo $ENV_VAR'
+```
+
+To disable further option processing, use two hyphens ("--") before the command:
 ```bash
-commandalarm 09:15:00 -d 3 -t 30 python3 script.py
+commandalarm 16:00:00 -- ls -l
 ```
 
 ## Contributing
 
 If you would like to contribute to CommandAlarm, please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/alofgren/commandalarm).
 
 ## Donate
```

### Comparing `CommandAlarm-0.2.4/LICENSE` & `CommandAlarm-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `CommandAlarm-0.2.4/PKG-INFO` & `CommandAlarm-0.2.5/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 Metadata-Version: 2.1
 Name: CommandAlarm
-Version: 0.2.4
+Version: 0.2.5
 Summary: A simple command line program that allows users to set an alarm with a custom command.
 Home-page: https://github.com/alofgren/commandalarm
 Author: alofgren
 Author-email: drelofren@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+License: GPLv3
+Project-URL: Bug Reports, https://github.com/alofgren/commandalarm/issues
+Project-URL: Source, https://github.com/alofgren/commandalarm
+Keywords: alarm,command,command-line,tool,timer,commandalarm
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CommandAlarm
 
 CommandAlarm is a simple command line program that allows users to set an alarm with a custom command. 
@@ -30,50 +39,55 @@
 git clone https://github.com/alofgren/commandalarm.git
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
-```bash
+```
 usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
   command               the command to run
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
-  -s, --shell           run command with shell
+  -s, --shell           run command in a shell
   -n, --no-check        don't check the command return code
   -t TIMEOUT, --timeout TIMEOUT
                         timeout in seconds for the command to complete
 ```
 
 ## Examples
 
-To set an alarm for 2:00 PM on Tuesday, and play a sound when the alarm goes off:
+To set an alarm for 2:00 PM and play a sound when the alarm goes off:
 ```bash
-commandalarm -d 2 14:00:00 aplay alarm_sound.wav
+commandalarm 14:00:00 aplay alarm_sound.wav
 ```
 
-To set an alarm for 10:00 PM to run a command with shell and repeat indefinitely: 
+To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
 ```bash
-commandalarm 22:00:00 -r -s 'echo "Hello, world!"'
+commandalarm 09:15:00 --day 3 --timeout 30 python3 script.py
 ```
 
-To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
+To run a command in a shell, use the -s or --shell option:
+```bash
+commandalarm 16:00:00 --shell 'ENV_VAR="I am running in a shell"; echo $ENV_VAR'
+```
+
+To disable further option processing, use two hyphens ("--") before the command:
 ```bash
-commandalarm 09:15:00 -d 3 -t 30 python3 script.py
+commandalarm 16:00:00 -- ls -l
 ```
 
 ## Contributing
 
 If you would like to contribute to CommandAlarm, please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/alofgren/commandalarm).
 
 ## Donate
```

### Comparing `CommandAlarm-0.2.4/README.md` & `CommandAlarm-0.2.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,50 +16,55 @@
 git clone https://github.com/alofgren/commandalarm.git
 cd commandalarm
 pip install .
 ```
 
 ## Usage Output
 
-```bash
+```
 usage: commandalarm [-h] [-v] [-d {1,2,3,4,5,6,7}] [-r] [-s] [-n] [-t TIMEOUT] time command [command ...]
 
 Set an alarm with a custom command.
 
 positional arguments:
   time                  the time in the format HH:MM:SS
   command               the command to run
 
 optional arguments:
   -h, --help            show this help message and exit
   -v, --version         show program's version number and exit
   -d {1,2,3,4,5,6,7}, --day {1,2,3,4,5,6,7}
                         the day of the week as an integer from 1 to 7, where 1 represents Monday
   -r, --repeat          repeat indefinitely
-  -s, --shell           run command with shell
+  -s, --shell           run command in a shell
   -n, --no-check        don't check the command return code
   -t TIMEOUT, --timeout TIMEOUT
                         timeout in seconds for the command to complete
 ```
 
 ## Examples
 
-To set an alarm for 2:00 PM on Tuesday, and play a sound when the alarm goes off:
+To set an alarm for 2:00 PM and play a sound when the alarm goes off:
 ```bash
-commandalarm -d 2 14:00:00 aplay alarm_sound.wav
+commandalarm 14:00:00 aplay alarm_sound.wav
 ```
 
-To set an alarm for 10:00 PM to run a command with shell and repeat indefinitely: 
+To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
 ```bash
-commandalarm 22:00:00 -r -s 'echo "Hello, world!"'
+commandalarm 09:15:00 --day 3 --timeout 30 python3 script.py
 ```
 
-To set an alarm for 9:15 AM on Wednesday to run a Python script with a timeout of 30 seconds: 
+To run a command in a shell, use the -s or --shell option:
+```bash
+commandalarm 16:00:00 --shell 'ENV_VAR="I am running in a shell"; echo $ENV_VAR'
+```
+
+To disable further option processing, use two hyphens ("--") before the command:
 ```bash
-commandalarm 09:15:00 -d 3 -t 30 python3 script.py
+commandalarm 16:00:00 -- ls -l
 ```
 
 ## Contributing
 
 If you would like to contribute to CommandAlarm, please feel free to submit a pull request or open an issue on the [GitHub repository](https://github.com/alofgren/commandalarm).
 
 ## Donate
```

### Comparing `CommandAlarm-0.2.4/commandalarm/commandalarm.py` & `CommandAlarm-0.2.5/commandalarm/commandalarm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 # commandalarm.py
 # Copyright (C) 2023 alofgren <drelofren@outlook.com>
 #
 # This program is free software: you can redistribute it and/or modify it under
 # the terms of the GNU General Public License as published by the Free Software
 # Foundation, either version 3 of the License, or (at your option) any later
 # version.
@@ -12,20 +11,23 @@
 # ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
 # FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along with
 # this program. If not, see <http://www.gnu.org/licenses/>.
 """ Set an alarm with a custom command. """
 
+import argparse
+import datetime
+import errno
+import platform
 import signal
+import subprocess
 import sys
+import threading
 import time
-import datetime
-import argparse
-import subprocess
 from . import __version__
 
 ALARM_FIRED = False  # pylint: disable=W0603
 
 
 def alarm_handler(signum, frame):  # pylint: disable=W0613
     """
@@ -61,43 +63,25 @@
         days_ahead += 7
     date_obj += datetime.timedelta(days=days_ahead)
     alarm_datetime = datetime.datetime.combine(date_obj, time_obj)
     seconds_until_alarm = int(
         round((alarm_datetime - datetime.datetime.now()).total_seconds()))
     if seconds_until_alarm <= 0:
         seconds_until_alarm = 1
-    signal.signal(signal.SIGALRM, alarm_handler)
-    signal.alarm(seconds_until_alarm)
+    if platform.system() == 'Windows':
+        timer = threading.Timer(seconds_until_alarm,
+                                alarm_handler,
+                                args=(None, None))
+        timer.start()
+    else:
+        signal.signal(signal.SIGALRM, alarm_handler)
+        signal.alarm(seconds_until_alarm)
     print(f"Alarm set for {alarm_datetime}")
 
 
-def validate_weekday(value):
-    """
-    Validates whether the given value is a valid weekday integer between 1 and 7.
-
-    Parameters:
-    value (str): The value to be validated.
-
-    Returns:
-    int: The weekday integer if it is valid.
-
-    Raises:
-    argparse.ArgumentTypeError: If the value is not a valid integer or not a valid weekday.
-    """
-    try:
-        weekday = int(value)
-        if weekday < 1 or weekday > 7:
-            raise argparse.ArgumentTypeError(
-                "%s is not a valid weekday (must be between 1 and 7)" % value)
-        return weekday
-    except ValueError as value_err:
-        raise argparse.ArgumentTypeError("%s is not a valid integer" %
-                                         value) from value_err
-
-
 def valid_time_string(time_str):
     """
     Validates that the time string is in the correct format.
 
     Parameters:
     time_str (str): The time in the format HH:MM:SS.
 
@@ -112,19 +96,25 @@
         return time_str
     except ValueError as value_err:
         raise argparse.ArgumentTypeError(
             f"{time_str} is not a valid time in the format HH:MM:SS"
         ) from value_err
 
 
-def main():
+def parse_arguments():
     """
-    The main function that parses command-line arguments, sets the alarm and runs the command.
+    Parse command-line arguments using argparse.
+
+    Returns:
+    argparse.Namespace: A namespace containing the parsed arguments.
+
+    Raises:
+    ValueError: If the time argument is not a valid time string.
+    ValueError: If the day argument is not a valid integer between 1 and 7.
     """
-    global ALARM_FIRED  # pylint: disable=W0603
     parser = argparse.ArgumentParser(
         description="Set an alarm with a custom command.")
     parser.add_argument(
         "time",
         type=valid_time_string,
         help="the time in the format HH:MM:SS",
     )
@@ -137,15 +127,15 @@
     parser.add_argument("-v",
                         "--version",
                         action="version",
                         version="%(prog)s " + __version__)
     parser.add_argument(
         "-d",
         "--day",
-        type=validate_weekday,
+        type=int,
         default=datetime.date.today().isoweekday(),
         help=
         "the day of the week as an integer from 1 to 7, where 1 represents Monday",
         choices=range(1, 8),
     )
     parser.add_argument(
         "-r",
@@ -153,57 +143,72 @@
         action="store_true",
         help="repeat indefinitely",
     )
     parser.add_argument("-s",
                         "--shell",
                         action="store_true",
                         default=False,
-                        help="run command with shell")
+                        help="run command in a shell")
     parser.add_argument("-n",
                         "--no-check",
                         action="store_false",
                         default=True,
                         help="don't check the command return code",
                         dest="check")
     parser.add_argument("-t",
                         "--timeout",
                         default=None,
                         type=int,
                         help="timeout in seconds for the command to complete")
-    args = parser.parse_args()
+    return parser.parse_args()
+
+
+def main():
+    """
+    The main function that parses command-line arguments, sets the alarm and runs the command.
+    """
+    global ALARM_FIRED  # pylint: disable=W0603
+    args = parse_arguments()
     try:
         set_alarm(args.time, args.day)
         while True:
             while not ALARM_FIRED:
-                signal.pause()
-            print("Time is up!")
+                if platform.system() == 'Windows':
+                    time.sleep(1)
+                else:
+                    signal.pause()
             command_str = " ".join(args.command)
+            command = command_str if args.shell else args.command
+            print("Time is up!")
             print("Running command:", command_str)
             try:
-                command = command_str if args.shell else args.command
                 result = subprocess.run(command,
                                         capture_output=True,
                                         shell=args.shell,
                                         timeout=args.timeout,
                                         check=args.check,
                                         text=True)
-                print(result.stdout)
+                print(result.stdout.strip())
             except FileNotFoundError:
                 print("Command not found", file=sys.stderr)
+                sys.exit(errno.ENOENT)
             except subprocess.CalledProcessError as called_process_err:
                 print(
                     f"Command returned non-zero exit status {called_process_err.returncode}",
                     file=sys.stderr)
                 print(f"stderr: {called_process_err.stderr}", file=sys.stderr)
+                sys.exit(called_process_err.returncode)
             except PermissionError as permission_err:
                 print(f"Permission error: {permission_err}", file=sys.stderr)
+                sys.exit(errno.EACCES)
             except subprocess.TimeoutExpired as timeout_expired:
                 print(
                     f"Command timed out after {timeout_expired.timeout} seconds",
                     file=sys.stderr)
+                sys.exit(errno.ETIME)
             if args.repeat:
                 ALARM_FIRED = False
                 time.sleep(1)
                 set_alarm(args.time, args.day)
             else:
                 break
     except KeyboardInterrupt:
```

### Comparing `CommandAlarm-0.2.4/setup.py` & `CommandAlarm-0.2.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,38 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-setuptools.setup(
-    name="CommandAlarm",
-    version="0.2.4",
-    author="alofgren",
-    author_email="drelofren@outlook.com",
-    description="A simple command line program that allows users to set an alarm with a custom command.",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="https://github.com/alofgren/commandalarm",
-    packages=setuptools.find_packages(),
-    entry_points={
+setuptools.setup (
+    name = "CommandAlarm",
+    version = "0.2.5",
+    author = "alofgren",
+    author_email = "drelofren@outlook.com",
+    description = "A simple command line program that allows users to set an alarm with a custom command.",
+    license = "GPLv3",
+    keywords = ["alarm","command","command-line","tool","timer","commandalarm"],
+    url = "https://github.com/alofgren/commandalarm",
+    long_description = long_description,
+    long_description_content_type = "text/markdown",
+    packages = setuptools.find_packages(),
+    entry_points = {
         "console_scripts": [
-            "commandalarm=commandalarm.commandalarm:main"
+            "commandalarm = commandalarm.commandalarm:main"
         ]
     },
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    classifiers = [
+        "Development Status :: 3 - Alpha",
+        "Environment :: Console",
+        "Intended Audience :: End Users/Desktop",
+        "Natural Language :: English",
         "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Topic :: Utilities",
     ],
+    project_urls = {
+        "Bug Reports": "https://github.com/alofgren/commandalarm/issues",
+        "Source": "https://github.com/alofgren/commandalarm",
+    },
     python_requires = ">=3"
 )
```

