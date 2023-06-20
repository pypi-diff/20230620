# Comparing `tmp/jaaql-monitor-1.2.71.tar.gz` & `tmp/jaaql-monitor-1.2.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-monitor-1.2.71.tar", last modified: Tue Jun 20 10:08:43 2023, max compression
+gzip compressed data, was "jaaql-monitor-1.2.72.tar", last modified: Tue Jun 20 10:10:37 2023, max compression
```

## Comparing `jaaql-monitor-1.2.71.tar` & `jaaql-monitor-1.2.72.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 10:08:43.164472 jaaql-monitor-1.2.71/
--rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.71/LICENSE.txt
--rw-rw-rw-   0        0        0     1454 2023-06-20 10:08:43.164472 jaaql-monitor-1.2.71/PKG-INFO
--rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.71/README.md
-drwxrwxrwx   0        0        0        0 2023-06-20 10:08:43.164472 jaaql-monitor-1.2.71/jaaql_monitor.egg-info/
--rw-rw-rw-   0        0        0     1454 2023-06-20 10:08:43.000000 jaaql-monitor-1.2.71/jaaql_monitor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      269 2023-06-20 10:08:43.000000 jaaql-monitor-1.2.71/jaaql_monitor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 10:08:43.000000 jaaql-monitor-1.2.71/jaaql_monitor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-20 10:08:43.000000 jaaql-monitor-1.2.71/jaaql_monitor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-20 10:08:43.000000 jaaql-monitor-1.2.71/jaaql_monitor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-20 10:08:43.164472 jaaql-monitor-1.2.71/monitor/
--rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.71/monitor/__init__.py
--rw-rw-rw-   0        0        0    31690 2023-06-20 10:08:32.000000 jaaql-monitor-1.2.71/monitor/main.py
--rw-rw-rw-   0        0        0      176 2023-06-20 10:08:34.000000 jaaql-monitor-1.2.71/monitor/version.py
--rw-rw-rw-   0        0        0       42 2023-06-20 10:08:43.169499 jaaql-monitor-1.2.71/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.71/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 10:10:37.806904 jaaql-monitor-1.2.72/
+-rw-rw-rw-   0        0        0    18124 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/LICENSE.txt
+-rw-rw-rw-   0        0        0     1454 2023-06-20 10:10:37.805905 jaaql-monitor-1.2.72/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 10:10:37.803906 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/
+-rw-rw-rw-   0        0        0     1454 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 10:10:37.000000 jaaql-monitor-1.2.72/jaaql_monitor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 10:10:37.804906 jaaql-monitor-1.2.72/monitor/
+-rw-rw-rw-   0        0        0        0 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/monitor/__init__.py
+-rw-rw-rw-   0        0        0    31684 2023-06-20 10:10:21.000000 jaaql-monitor-1.2.72/monitor/main.py
+-rw-rw-rw-   0        0        0      176 2023-06-20 10:10:28.000000 jaaql-monitor-1.2.72/monitor/version.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 10:10:37.807905 jaaql-monitor-1.2.72/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-06-13 23:48:02.000000 jaaql-monitor-1.2.72/setup.py
```

### Comparing `jaaql-monitor-1.2.71/LICENSE.txt` & `jaaql-monitor-1.2.72/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.71/PKG-INFO` & `jaaql-monitor-1.2.72/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.71
+Version: 1.2.72
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.71/README.md` & `jaaql-monitor-1.2.72/README.md`

 * *Files identical despite different names*

### Comparing `jaaql-monitor-1.2.71/jaaql_monitor.egg-info/PKG-INFO` & `jaaql-monitor-1.2.72/jaaql_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-monitor
-Version: 1.2.71
+Version: 1.2.72
 Summary: How to interact with jaaql
 Home-page: https://github.com/JAAQL/JAAQL-monitor
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `jaaql-monitor-1.2.71/monitor/main.py` & `jaaql-monitor-1.2.72/monitor/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 ARGS__encoded_config = ['--encoded-config']
 ARGS__config = ['-c', '--config']
 ARGS__folder_config = ['-f', '--folder-config']
 ARGS__input_file = ['-i', '--input-file']
 ARGS__parameter = ['-p', '--parameter']
 ARGS__single_query = ['-s', '--single-query']
 ARGS__environment = ['-e', '--environment-file']
-ARGS__prevent_unused_parameters = ['-p', '--prevent-unused-parameters']
+ARGS__allow_unused_parameters = ['-a', '--allow-unused-parameters']
 
 
 class JAAQLMonitorException(Exception):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
 
@@ -613,15 +613,15 @@
         state.file_name = file_name
 
     state.override_url = override_url
 
     state.is_verbose = len([arg for arg in args if arg in ['-v', '--verbose']]) != 0
     state.is_debugging = len([arg for arg in args if arg in ['-d', '--debugging']]) != 0
     state.single_query = len([arg for arg in args if arg in ARGS__single_query]) != 0
-    state.prevent_unused_parameters = len([arg for arg in args if arg in ARGS__prevent_unused_parameters]) == 0
+    state.prevent_unused_parameters = len([arg for arg in args if arg in ARGS__allow_unused_parameters]) == 0
 
     if state.is_verbose:
         print_version()
 
     for arg, arg_idx in zip(args, range(len(args))):
         if arg not in ARGS__parameter:
             continue
```

### Comparing `jaaql-monitor-1.2.71/setup.py` & `jaaql-monitor-1.2.72/setup.py`

 * *Files identical despite different names*

