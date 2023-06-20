# Comparing `tmp/urpautils-0.7.0.tar.gz` & `tmp/urpautils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\urpautils-0.7.0.tar", last modified: Thu Nov 10 09:17:41 2022, max compression
+gzip compressed data, was "dist\urpautils-0.7.1.tar", last modified: Tue Jun 20 12:48:46 2023, max compression
```

## Comparing `urpautils-0.7.0.tar` & `urpautils-0.7.1.tar`

### file list

```diff
@@ -1,21 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-11-10 09:17:41.819742 urpautils-0.7.0/
--rw-rw-rw-   0        0        0       26 2021-08-04 11:47:27.000000 urpautils-0.7.0/MANIFEST.in
--rw-rw-rw-   0        0        0    13029 2022-11-10 09:17:41.819242 urpautils-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0    10434 2022-11-10 09:06:13.000000 urpautils-0.7.0/README.md
--rw-rw-rw-   0        0        0       42 2022-11-10 09:17:41.820240 urpautils-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0     1092 2021-09-01 10:03:30.000000 urpautils-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-10 09:17:41.798822 urpautils-0.7.0/urpautils/
--rw-rw-rw-   0        0        0      322 2022-11-10 09:08:47.000000 urpautils-0.7.0/urpautils/__about__.py
--rw-rw-rw-   0        0        0      101 2021-08-03 13:14:30.000000 urpautils-0.7.0/urpautils/__init__.py
--rw-rw-rw-   0        0        0     6413 2021-10-21 11:46:40.000000 urpautils-0.7.0/urpautils/csv_utils.py
--rw-rw-rw-   0        0        0     9743 2021-09-30 13:30:34.000000 urpautils-0.7.0/urpautils/file_utils.py
--rw-rw-rw-   0        0        0        0 2021-08-04 11:43:23.000000 urpautils-0.7.0/urpautils/py.typed
--rw-rw-rw-   0        0        0    14603 2022-09-15 12:28:27.000000 urpautils-0.7.0/urpautils/robot.py
--rw-rw-rw-   0        0        0    14685 2022-11-10 09:06:13.000000 urpautils-0.7.0/urpautils/universal.py
-drwxrwxrwx   0        0        0        0 2022-11-10 09:17:41.816315 urpautils-0.7.0/urpautils.egg-info/
--rw-rw-rw-   0        0        0    13029 2022-11-10 09:17:41.000000 urpautils-0.7.0/urpautils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      379 2022-11-10 09:17:41.000000 urpautils-0.7.0/urpautils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-10 09:17:41.000000 urpautils-0.7.0/urpautils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-08-10 08:16:54.000000 urpautils-0.7.0/urpautils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       21 2022-11-10 09:17:41.000000 urpautils-0.7.0/urpautils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-11-10 09:17:41.000000 urpautils-0.7.0/urpautils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/.github/
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1377 2021-09-01 14:23:12.000000 urpautils-0.7.1/.github/workflows/test.yml
+-rw-rw-rw-   0        0        0     1307 2021-07-29 08:29:50.000000 urpautils-0.7.1/.gitignore
+-rw-rw-rw-   0        0        0     2831 2023-06-20 12:46:22.000000 urpautils-0.7.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1089 2021-07-29 08:29:50.000000 urpautils-0.7.1/LICENSE
+-rw-rw-rw-   0        0        0       26 2021-08-04 11:47:27.000000 urpautils-0.7.1/MANIFEST.in
+-rw-rw-rw-   0        0        0    13040 2023-06-20 12:48:46.000000 urpautils-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0    10437 2023-06-20 12:46:22.000000 urpautils-0.7.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/mock/
+-rw-rw-rw-   0        0        0      176 2021-09-01 14:28:37.000000 urpautils-0.7.1/mock/urpa.py
+-rw-rw-rw-   0        0        0       42 2023-06-20 12:48:46.000000 urpautils-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1092 2021-09-01 10:03:30.000000 urpautils-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/tests/
+-rw-rw-rw-   0        0        0        0 2021-08-04 10:09:43.000000 urpautils-0.7.1/tests/__init__.py
+-rw-rw-rw-   0        0        0       63 2021-08-05 09:55:36.000000 urpautils-0.7.1/tests/conftest.py
+-rw-rw-rw-   0        0        0       53 2021-08-05 09:55:36.000000 urpautils-0.7.1/tests/requirements.txt
+-rw-rw-rw-   0        0        0     2158 2021-10-21 11:47:44.000000 urpautils-0.7.1/tests/test_csv_utils.py
+-rw-rw-rw-   0        0        0     5561 2021-08-05 09:55:36.000000 urpautils-0.7.1/tests/test_file_utils.py
+-rw-rw-rw-   0        0        0     7452 2022-11-10 09:06:13.000000 urpautils-0.7.1/tests/test_universal.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/urpautils/
+-rw-rw-rw-   0        0        0      322 2023-06-20 12:46:22.000000 urpautils-0.7.1/urpautils/__about__.py
+-rw-rw-rw-   0        0        0      101 2021-08-03 13:14:30.000000 urpautils-0.7.1/urpautils/__init__.py
+-rw-rw-rw-   0        0        0     6413 2021-10-21 11:46:40.000000 urpautils-0.7.1/urpautils/csv_utils.py
+-rw-rw-rw-   0        0        0     9743 2021-09-30 13:30:34.000000 urpautils-0.7.1/urpautils/file_utils.py
+-rw-rw-rw-   0        0        0        0 2021-08-04 11:43:23.000000 urpautils-0.7.1/urpautils/py.typed
+-rw-rw-rw-   0        0        0    14603 2022-09-15 12:28:27.000000 urpautils-0.7.1/urpautils/robot.py
+-rw-rw-rw-   0        0        0    15412 2023-06-20 12:46:22.000000 urpautils-0.7.1/urpautils/universal.py
+drwxrwxrwx   0        0        0        0 2023-06-20 12:48:46.000000 urpautils-0.7.1/urpautils.egg-info/
+-rw-rw-rw-   0        0        0    13040 2023-06-20 12:48:45.000000 urpautils-0.7.1/urpautils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      583 2023-06-20 12:48:46.000000 urpautils-0.7.1/urpautils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 12:48:45.000000 urpautils-0.7.1/urpautils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2021-08-10 08:16:54.000000 urpautils-0.7.1/urpautils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       21 2023-06-20 12:48:45.000000 urpautils-0.7.1/urpautils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-20 12:48:45.000000 urpautils-0.7.1/urpautils.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `urpautils-0.7.0/PKG-INFO` & `urpautils-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urpautils
-Version: 0.7.0
+Version: 0.7.1
 Summary: Module containig universal functions used with UltimateRPA robots
 Home-page: https://github.com/ultimaterpa/urpautils
 Author: anerold
 Author-email: support@ultimaterpa.cz
 License: MIT
 Description: # urpautils
         ![workflow](https://github.com/ultimaterpa/urpautils/actions/workflows/test.yml/badge.svg)
@@ -141,15 +141,15 @@
         # Get timestamp
         timestamp = urpautils.timestamp()
         
         # Modify path to avoid win32api 260 character limit
         modified_path = urpautils.add_long_path_prefix("C:\\very\long\path")
         
         # Kill process tree
-        urpautils.killapp("image_name")
+        urpautils.kill_app("image_name")
         
         # Send an email
         # port is an optional argument. smtplib.SMTP_PORT (=25) is used if not provided
         # attachments is an optional argument
         # there is one more optional arg: debug_level (defaults to 0)
         urpautils.send_email_notification(
             "sender@stringdata.cz",
@@ -250,14 +250,15 @@
             "body",
             "smtp_server.cz"
         )
         def my_decorated_function():
             # before SomeError is raised the email is sent
             raise SomeError
         ```
+        
 Keywords: Robotic Process Automation,RPA,UltimateRPA,utilities
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

### Comparing `urpautils-0.7.0/README.md` & `urpautils-0.7.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -133,15 +133,15 @@
 # Get timestamp
 timestamp = urpautils.timestamp()
 
 # Modify path to avoid win32api 260 character limit
 modified_path = urpautils.add_long_path_prefix("C:\\very\long\path")
 
 # Kill process tree
-urpautils.killapp("image_name")
+urpautils.kill_app("image_name")
 
 # Send an email
 # port is an optional argument. smtplib.SMTP_PORT (=25) is used if not provided
 # attachments is an optional argument
 # there is one more optional arg: debug_level (defaults to 0)
 urpautils.send_email_notification(
     "sender@stringdata.cz",
@@ -241,8 +241,8 @@
     "subject",
     "body",
     "smtp_server.cz"
 )
 def my_decorated_function():
     # before SomeError is raised the email is sent
     raise SomeError
-```
+```
```

### Comparing `urpautils-0.7.0/setup.py` & `urpautils-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `urpautils-0.7.0/urpautils/csv_utils.py` & `urpautils-0.7.1/urpautils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `urpautils-0.7.0/urpautils/file_utils.py` & `urpautils-0.7.1/urpautils/file_utils.py`

 * *Files identical despite different names*

### Comparing `urpautils-0.7.0/urpautils/robot.py` & `urpautils-0.7.1/urpautils/robot.py`

 * *Files identical despite different names*

### Comparing `urpautils-0.7.0/urpautils/universal.py` & `urpautils-0.7.1/urpautils/universal.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,44 +110,62 @@
     sender = smtplib.SMTP(smtp_server, smtp_port)
     sender.set_debuglevel(debug_level)
     sender.sendmail(email_sender, recipients + recipients_copy, mail.as_string())
     sender.quit()
     logger.info("E-mail sent")
 
 
-def repeat(func) -> Callable:
-    """Function, which contains wrapper and is used as decorator for other functions/methods"""
+def repeat(action: str, repetition: int = 3) -> Callable:
+    """
+    Function that returns a decorator used to repeat commands in a function until no exception occurs,
+    or the maximum number of attempts is reached.
+
+    :param action: str, the name of the action for logging purposes
+    :param repetition: int, the number of repetitions (default is 3)
+    :return: Callable, the decorated function
+    """
 
-    @functools.wraps(func)
-    def wrapper(*args, action: str, repetition: int = 3, **kwargs) -> Callable:
-        """Repeat commands in a function until no Exception occurs, or run out of attempts
-
-        :param action:          str, the name of the action for logging purposes
-        :param repetition:      int, the number of repetitions, by default, is 3
-        :return Callable
+    def decorator(func: Callable) -> Callable:
         """
+        Decorator function that wraps the provided function with the repeat behavior.
 
-        error = None
-        logger.info(f"Executing action: '{action}'")
-        for pokus in range(1, repetition + 1):
-            try:
-                logger.info(f"'{pokus}'. attempt to execute: '{action}'")
-                return func(*args, **kwargs)
-            except Exception as err:
-                error = err
-                logger.exception(f"An Exception has occured: {err}")
-                continue
-            finally:
-                if not error:
-                    logger.info(f"Successfully executed: '{action}'")
+        :param func: Callable, the function to be decorated
+        :return: Callable, the decorated function
+        """
+
+        @functools.wraps(func)
+        def wrapper(*args, **kwargs) -> Callable:
+            """
+            Repeat commands in a function until no exception occurs, or the maximum number of attempts is reached.
+
+            :param args: positional arguments to be passed to the decorated function
+            :param kwargs: keyword arguments to be passed to the decorated function
+            :return: Callable, the decorated function's return value
+            """
+
+            error = None
+            logger.info(f"Executing action: '{action}'")
+            for pokus in range(1, repetition + 1):
+                try:
+                    logger.info(f"'{pokus}'. attempt to execute: '{action}'")
+                    return func(*args, **kwargs)
+                except Exception as err:
+                    error = err
+                    logger.exception(f"An Exception has occured: {err}")
+                    continue
+                finally:
+                    if not error:
+                        logger.info(f"Successfully executed: '{action}'")
+
+            logger.error(f"Unsuccessfully executed: '{action}'")
+            raise RuntimeError(f"Robot was unable to execute this action '{action}' due to this error '{error}'")
 
-        logger.error(f"Unsuccessfully executed: '{action}'")
-        raise RuntimeError(f"Robot was unable to execute this action '{action}' due to this error '{error}'")
+        return wrapper
 
-    return wrapper
+    return decorator
 
 
 def get_birth_date(number: str) -> datetime.date:
     """Returns birth date calculated from personal identification number
 
     :param number:   string in format xxxxxxxxxx
     :return:         datetime.date object (or raises ValueError)
```

### Comparing `urpautils-0.7.0/urpautils.egg-info/PKG-INFO` & `urpautils-0.7.1/urpautils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urpautils
-Version: 0.7.0
+Version: 0.7.1
 Summary: Module containig universal functions used with UltimateRPA robots
 Home-page: https://github.com/ultimaterpa/urpautils
 Author: anerold
 Author-email: support@ultimaterpa.cz
 License: MIT
 Description: # urpautils
         ![workflow](https://github.com/ultimaterpa/urpautils/actions/workflows/test.yml/badge.svg)
@@ -141,15 +141,15 @@
         # Get timestamp
         timestamp = urpautils.timestamp()
         
         # Modify path to avoid win32api 260 character limit
         modified_path = urpautils.add_long_path_prefix("C:\\very\long\path")
         
         # Kill process tree
-        urpautils.killapp("image_name")
+        urpautils.kill_app("image_name")
         
         # Send an email
         # port is an optional argument. smtplib.SMTP_PORT (=25) is used if not provided
         # attachments is an optional argument
         # there is one more optional arg: debug_level (defaults to 0)
         urpautils.send_email_notification(
             "sender@stringdata.cz",
@@ -250,14 +250,15 @@
             "body",
             "smtp_server.cz"
         )
         def my_decorated_function():
             # before SomeError is raised the email is sent
             raise SomeError
         ```
+        
 Keywords: Robotic Process Automation,RPA,UltimateRPA,utilities
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
```

