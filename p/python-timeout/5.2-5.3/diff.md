# Comparing `tmp/python-timeout-5.2.tar.gz` & `tmp/python-timeout-5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-timeout-5.2.tar", last modified: Tue Jun 13 00:03:11 2023, max compression
+gzip compressed data, was "python-timeout-5.3.tar", last modified: Tue Jun 20 19:56:02 2023, max compression
```

## Comparing `python-timeout-5.2.tar` & `python-timeout-5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.916420 python-timeout-5.2/
--rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.2/.gitignore
--rw-rw-rw-   0        0        0      973 2023-06-13 00:03:11.916420 python-timeout-5.2/PKG-INFO
--rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.913423 python-timeout-5.2/python_timeout.egg-info/
--rw-rw-rw-   0        0        0      973 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-13 00:03:11.000000 python-timeout-5.2/python_timeout.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-13 00:03:11.917420 python-timeout-5.2/setup.cfg
--rw-rw-rw-   0        0        0      413 2023-06-13 00:03:05.000000 python-timeout-5.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.914422 python-timeout-5.2/timeout/
--rw-rw-rw-   0        0        0     9145 2023-06-13 00:02:54.000000 python-timeout-5.2/timeout/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:03:11.915421 python-timeout-5.2/timeout/__pycache__/
--rw-rw-rw-   0        0        0     2743 2023-04-21 11:32:29.000000 python-timeout-5.2/timeout/__pycache__/__init__.cpython-39.pyc
+drwxrwxrwx   0        0        0        0 2023-06-20 19:56:02.607893 python-timeout-5.3/
+-rw-rw-rw-   0        0        0       35 2022-03-16 16:24:46.000000 python-timeout-5.3/.gitignore
+-rw-rw-rw-   0        0        0      973 2023-06-20 19:56:02.607893 python-timeout-5.3/PKG-INFO
+-rw-rw-rw-   0        0        0      757 2022-05-11 17:10:57.000000 python-timeout-5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 19:56:02.604895 python-timeout-5.3/python_timeout.egg-info/
+-rw-rw-rw-   0        0        0      973 2023-06-20 19:56:02.000000 python-timeout-5.3/python_timeout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-06-20 19:56:02.000000 python-timeout-5.3/python_timeout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 19:56:02.000000 python-timeout-5.3/python_timeout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-06-20 19:56:02.000000 python-timeout-5.3/python_timeout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 19:56:02.000000 python-timeout-5.3/python_timeout.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-20 19:56:02.608893 python-timeout-5.3/setup.cfg
+-rw-rw-rw-   0        0        0      413 2023-06-20 19:55:59.000000 python-timeout-5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:56:02.605895 python-timeout-5.3/timeout/
+-rw-rw-rw-   0        0        0     9408 2023-06-20 19:55:57.000000 python-timeout-5.3/timeout/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 19:56:02.606894 python-timeout-5.3/timeout/__pycache__/
+-rw-rw-rw-   0        0        0     2743 2023-04-21 11:32:29.000000 python-timeout-5.3/timeout/__pycache__/__init__.cpython-39.pyc
```

### Comparing `python-timeout-5.2/PKG-INFO` & `python-timeout-5.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 5.2
+Version: 5.3
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-5.2/README.md` & `python-timeout-5.3/README.md`

 * *Files identical despite different names*

### Comparing `python-timeout-5.2/python_timeout.egg-info/PKG-INFO` & `python-timeout-5.3/python_timeout.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-timeout
-Version: 5.2
+Version: 5.3
 Summary: Random timeout between minimum and maximum values
 Home-page: https://github.com/xjxckk/python-timeout/
 Description-Content-Type: text/markdown
 
 ### Timeout
 Random timeout between minimum and maximum values
```

### Comparing `python-timeout-5.2/timeout/__init__.py` & `python-timeout-5.3/timeout/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -143,17 +143,18 @@
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_minutes == 1:
                     print('Sleeping 1 minute until', til)
                 else:
                     print('Sleeping', timeout_in_minutes, 'minutes until', til)
 
-        sleep(timeout_in_seconds)
+        wait(timeout_in_seconds)
 
-class sleep_for:
+wait = sleep
+class sleep:
     '''Sleep amount of time in minutes, hours or days and prints when it will continue'''
     def __init__(self, seconds=None, minutes=None, hours=None, days=None, silent=False):
         if seconds:
             timeout_in_seconds = seconds
         if minutes:
             timeout_in_seconds = minutes * 60
         elif hours:
@@ -185,8 +186,13 @@
                 til = datetime.now() + timedelta(seconds=timeout_in_seconds)
                 til = til.strftime('%H:%M')
                 if timeout_in_minutes == 1:
                     print('Sleeping 1 minute until', til)
                 else:
                     print('Sleeping', timeout_in_minutes, 'minutes until', til)
 
-        sleep(timeout_in_seconds)
+        wait(timeout_in_seconds)
+
+class sleep_for:
+    '''Sleep amount of time in minutes, hours or days and prints when it will continue'''
+    def __init__(self, seconds=None, minutes=None, hours=None, days=None, silent=False):
+        sleep(seconds, minutes, hours, days, silent)
```

### Comparing `python-timeout-5.2/timeout/__pycache__/__init__.cpython-39.pyc` & `python-timeout-5.3/timeout/__pycache__/__init__.cpython-39.pyc`

 * *Files identical despite different names*

