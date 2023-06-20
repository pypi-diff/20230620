# Comparing `tmp/ajenti-panel-2.2.5.tar.gz` & `tmp/ajenti-panel-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ajenti-panel-2.2.5.tar", last modified: Mon May  8 04:10:16 2023, max compression
+gzip compressed data, was "ajenti-panel-2.2.6.tar", last modified: Tue Jun 20 15:33:08 2023, max compression
```

## Comparing `ajenti-panel-2.2.5.tar` & `ajenti-panel-2.2.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.653646 ajenti-panel-2.2.5/
--rw-r--r--   0 eugene     (501) staff       (20)      190 2023-05-08 04:10:16.653733 ajenti-panel-2.2.5/PKG-INFO
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.649271 ajenti-panel-2.2.5/aj/
--rw-r--r--   0 eugene     (501) staff       (20)     4243 2023-05-08 04:08:59.000000 ajenti-panel-2.2.5/aj/__init__.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.649768 ajenti-panel-2.2.5/aj/api/
--rw-r--r--   0 eugene     (501) staff       (20)      188 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/api/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     3940 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/api/endpoint.py
--rw-r--r--   0 eugene     (501) staff       (20)     7176 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/api/http.py
--rw-r--r--   0 eugene     (501) staff       (20)     4994 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/api/mail.py
--rw-r--r--   0 eugene     (501) staff       (20)     8389 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/auth.py
--rw-r--r--   0 eugene     (501) staff       (20)     2161 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/compat.py
--rw-r--r--   0 eugene     (501) staff       (20)    12255 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/config.py
--rw-r--r--   0 eugene     (501) staff       (20)    10353 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/core.py
--rw-r--r--   0 eugene     (501) staff       (20)     1958 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/entry.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.650577 ajenti-panel-2.2.5/aj/gate/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/gate/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     6351 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/gate/gate.py
--rw-r--r--   0 eugene     (501) staff       (20)     9770 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/gate/middleware.py
--rw-r--r--   0 eugene     (501) staff       (20)     2134 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/gate/session.py
--rw-r--r--   0 eugene     (501) staff       (20)     3899 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/gate/stream.py
--rw-r--r--   0 eugene     (501) staff       (20)     7857 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/gate/worker.py
--rw-r--r--   0 eugene     (501) staff       (20)    13431 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/http.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/https_redirect.py
--rw-r--r--   0 eugene     (501) staff       (20)     4095 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/log.py
--rw-r--r--   0 eugene     (501) staff       (20)    10728 2023-02-13 11:54:42.000000 ajenti-panel-2.2.5/aj/plugins.py
--rw-r--r--   0 eugene     (501) staff       (20)     4533 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/routing.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.651201 ajenti-panel-2.2.5/aj/security/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/security/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     4395 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/security/pwreset.py
--rw-r--r--   0 eugene     (501) staff       (20)      786 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/aj/security/totp.py
--rw-r--r--   0 eugene     (501) staff       (20)      802 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/security/verifier.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.646004 ajenti-panel-2.2.5/aj/static/
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.651355 ajenti-panel-2.2.5/aj/static/emails/
--rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/static/emails/reset_email.html
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.651753 ajenti-panel-2.2.5/aj/static/images/
--rw-r--r--   0 eugene     (501) staff       (20)    19273 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/static/images/Logo.png
--rw-r--r--   0 eugene     (501) staff       (20)     3612 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/static/images/error.jpeg
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.652873 ajenti-panel-2.2.5/aj/util/
--rw-r--r--   0 eugene     (501) staff       (20)      340 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/util/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)      402 2020-05-02 13:26:29.000000 ajenti-panel-2.2.5/aj/util/broadcast_queue.py
--rw-r--r--   0 eugene     (501) staff       (20)      708 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/util/lazy.py
--rw-r--r--   0 eugene     (501) staff       (20)     1577 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/aj/util/misc.py
--rw-r--r--   0 eugene     (501) staff       (20)     1074 2020-05-02 13:26:29.000000 ajenti-panel-2.2.5/aj/util/pidfile.py
--rw-r--r--   0 eugene     (501) staff       (20)      527 2020-04-13 10:52:48.000000 ajenti-panel-2.2.5/aj/util/public.py
--rw-r--r--   0 eugene     (501) staff       (20)      373 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/util/strings.py
--rw-r--r--   0 eugene     (501) staff       (20)     2424 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/aj/wsgi.py
--rwxr-xr-x   0 eugene     (501) staff       (20)     1858 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/ajenti-client-ssl-gen
--rwxr-xr-x   0 eugene     (501) staff       (20)     4261 2023-01-06 10:26:21.000000 ajenti-panel-2.2.5/ajenti-panel
--rwxr-xr-x   0 eugene     (501) staff       (20)     1340 2022-06-28 14:12:43.000000 ajenti-panel-2.2.5/ajenti-ssl-gen
--rwxr-xr-x   0 eugene     (501) staff       (20)     1477 2022-02-17 09:04:54.000000 ajenti-panel-2.2.5/ajenti-upgrade
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:16.653525 ajenti-panel-2.2.5/ajenti_panel.egg-info/
--rw-r--r--   0 eugene     (501) staff       (20)      190 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)      913 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) staff       (20)       26 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/requires.txt
--rw-r--r--   0 eugene     (501) staff       (20)        3 2023-05-08 04:10:16.000000 ajenti-panel-2.2.5/ajenti_panel.egg-info/top_level.txt
--rw-r--r--   0 eugene     (501) staff       (20)       67 2023-05-08 04:10:16.653968 ajenti-panel-2.2.5/setup.cfg
--rwxr-xr-x   0 eugene     (501) staff       (20)     1924 2023-05-08 04:08:59.000000 ajenti-panel-2.2.5/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.214991 ajenti-panel-2.2.6/
+-rw-r--r--   0 eugene     (501) staff       (20)      190 2023-06-20 15:33:08.215064 ajenti-panel-2.2.6/PKG-INFO
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.210729 ajenti-panel-2.2.6/aj/
+-rw-r--r--   0 eugene     (501) staff       (20)     4243 2023-06-20 15:28:29.000000 ajenti-panel-2.2.6/aj/__init__.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.211246 ajenti-panel-2.2.6/aj/api/
+-rw-r--r--   0 eugene     (501) staff       (20)      188 2020-04-13 10:52:48.000000 ajenti-panel-2.2.6/aj/api/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3940 2023-02-13 11:54:42.000000 ajenti-panel-2.2.6/aj/api/endpoint.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7176 2023-02-13 11:54:42.000000 ajenti-panel-2.2.6/aj/api/http.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4994 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/api/mail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8389 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/auth.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2161 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/compat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12255 2023-02-13 11:54:42.000000 ajenti-panel-2.2.6/aj/config.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10353 2023-01-06 10:26:21.000000 ajenti-panel-2.2.6/aj/core.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1958 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/entry.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.211978 ajenti-panel-2.2.6/aj/gate/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.6/aj/gate/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     6351 2023-01-06 10:26:21.000000 ajenti-panel-2.2.6/aj/gate/gate.py
+-rw-r--r--   0 eugene     (501) staff       (20)     9700 2023-06-20 15:28:29.000000 ajenti-panel-2.2.6/aj/gate/middleware.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2172 2023-06-20 15:28:29.000000 ajenti-panel-2.2.6/aj/gate/session.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3899 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/gate/stream.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7857 2023-01-06 10:26:21.000000 ajenti-panel-2.2.6/aj/gate/worker.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13431 2023-02-13 11:54:42.000000 ajenti-panel-2.2.6/aj/http.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/https_redirect.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4095 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/log.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10728 2023-02-13 11:54:42.000000 ajenti-panel-2.2.6/aj/plugins.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4533 2023-01-06 10:26:21.000000 ajenti-panel-2.2.6/aj/routing.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.212615 ajenti-panel-2.2.6/aj/security/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 ajenti-panel-2.2.6/aj/security/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4395 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/security/pwreset.py
+-rw-r--r--   0 eugene     (501) staff       (20)      786 2023-01-06 10:26:21.000000 ajenti-panel-2.2.6/aj/security/totp.py
+-rw-r--r--   0 eugene     (501) staff       (20)      802 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/security/verifier.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.207735 ajenti-panel-2.2.6/aj/static/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.212750 ajenti-panel-2.2.6/aj/static/emails/
+-rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/static/emails/reset_email.html
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.213070 ajenti-panel-2.2.6/aj/static/images/
+-rw-r--r--   0 eugene     (501) staff       (20)    19273 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/static/images/Logo.png
+-rw-r--r--   0 eugene     (501) staff       (20)     3612 2020-04-13 10:52:48.000000 ajenti-panel-2.2.6/aj/static/images/error.jpeg
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.214010 ajenti-panel-2.2.6/aj/util/
+-rw-r--r--   0 eugene     (501) staff       (20)      340 2020-04-13 10:52:48.000000 ajenti-panel-2.2.6/aj/util/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)      402 2020-05-02 13:26:29.000000 ajenti-panel-2.2.6/aj/util/broadcast_queue.py
+-rw-r--r--   0 eugene     (501) staff       (20)      708 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/util/lazy.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1577 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/aj/util/misc.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1074 2020-05-02 13:26:29.000000 ajenti-panel-2.2.6/aj/util/pidfile.py
+-rw-r--r--   0 eugene     (501) staff       (20)      527 2020-04-13 10:52:48.000000 ajenti-panel-2.2.6/aj/util/public.py
+-rw-r--r--   0 eugene     (501) staff       (20)      373 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/util/strings.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2424 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/aj/wsgi.py
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1858 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/ajenti-client-ssl-gen
+-rwxr-xr-x   0 eugene     (501) staff       (20)     4261 2023-01-06 10:26:21.000000 ajenti-panel-2.2.6/ajenti-panel
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1340 2022-06-28 14:12:43.000000 ajenti-panel-2.2.6/ajenti-ssl-gen
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1477 2022-02-17 09:04:54.000000 ajenti-panel-2.2.6/ajenti-upgrade
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:08.214813 ajenti-panel-2.2.6/ajenti_panel.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)      190 2023-06-20 15:33:08.000000 ajenti-panel-2.2.6/ajenti_panel.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      913 2023-06-20 15:33:08.000000 ajenti-panel-2.2.6/ajenti_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-06-20 15:33:08.000000 ajenti-panel-2.2.6/ajenti_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       26 2023-06-20 15:33:08.000000 ajenti-panel-2.2.6/ajenti_panel.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        3 2023-06-20 15:33:08.000000 ajenti-panel-2.2.6/ajenti_panel.egg-info/top_level.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       67 2023-06-20 15:33:08.215385 ajenti-panel-2.2.6/setup.cfg
+-rwxr-xr-x   0 eugene     (501) staff       (20)     1924 2023-06-20 15:28:29.000000 ajenti-panel-2.2.6/setup.py
```

### Comparing `ajenti-panel-2.2.5/aj/__init__.py` & `ajenti-panel-2.2.6/aj/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 import os
 import platform as pyplatform
 import signal
 import subprocess
 
-__version__ = '2.2.5'
+__version__ = '2.2.6'
 
 # Global state
 
 product = None
 """ Custom product name """
 
 config = None
```

### Comparing `ajenti-panel-2.2.5/aj/api/endpoint.py` & `ajenti-panel-2.2.6/aj/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/api/http.py` & `ajenti-panel-2.2.6/aj/api/http.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/api/mail.py` & `ajenti-panel-2.2.6/aj/api/mail.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/auth.py` & `ajenti-panel-2.2.6/aj/auth.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/compat.py` & `ajenti-panel-2.2.6/aj/compat.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/config.py` & `ajenti-panel-2.2.6/aj/config.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/core.py` & `ajenti-panel-2.2.6/aj/core.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/entry.py` & `ajenti-panel-2.2.6/aj/entry.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/gate/gate.py` & `ajenti-panel-2.2.6/aj/gate/gate.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/gate/middleware.py` & `ajenti-panel-2.2.6/aj/gate/middleware.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import pwd
 import random
 import base64
 import time
 import gevent
 from socketio import Namespace
-from cookies import Cookies
+from http.cookies import SimpleCookie
 from gevent.timeout import Timeout
 from jadi import service
 
 import aj
 from aj.gate.gate import WorkerGate
 from aj.gate.session import Session
 from aj.gate.worker import WorkerError
@@ -125,18 +125,15 @@
         self.sessions[session_key] = session
         return session
 
     def obtain_session(self, env):
         cookie_str = env.get('HTTP_COOKIE', None)
         session = None
         if cookie_str:
-            cookie = Cookies.from_request(
-                cookie_str,
-                ignore_bad_cookies=True,
-            ).get('session', None)
+            cookie = SimpleCookie(cookie_str).get('session', None)
             if cookie and cookie.value:
                 if cookie.value in self.sessions:
                     # Session found
                     session = self.sessions[cookie.value]
                     if session.is_dead():
                         session = None
         return session
```

### Comparing `ajenti-panel-2.2.5/aj/gate/session.py` & `ajenti-panel-2.2.6/aj/gate/session.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import time
 import logging
-from cookies import Cookie
+from http.cookies import SimpleCookie
 
 from aj.gate.gate import WorkerGate
 
 
 class Session():
     """
     Holds the HTTP session data
@@ -60,21 +60,20 @@
         return not self.active or self.get_age() > self.session_max_time
 
     def set_cookie(self, http_context):
         """
         Adds headers to :class:`aj.http.HttpContext` that set
         the session cookie
         """
-        cookie = Cookie(
-            'session',
-            self.key,
-            path='/',
-            httponly=True
-        ).render_response()
-        http_context.add_header('Set-Cookie', cookie)
+
+        cookie = SimpleCookie()
+        cookie['session'] = self.key
+        cookie['session']['path'] = '/'
+        cookie['session']['httponly'] = True
+        http_context.add_header('Set-Cookie', cookie.output(header=''))
 
     def serialize(self):
         return {
             'key':self.key,
             'identity':self.identity,
             'timestamp':self.timestamp,
             'client_info':self.client_info
```

### Comparing `ajenti-panel-2.2.5/aj/gate/stream.py` & `ajenti-panel-2.2.6/aj/gate/stream.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/gate/worker.py` & `ajenti-panel-2.2.6/aj/gate/worker.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/http.py` & `ajenti-panel-2.2.6/aj/http.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/https_redirect.py` & `ajenti-panel-2.2.6/aj/https_redirect.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/log.py` & `ajenti-panel-2.2.6/aj/log.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/plugins.py` & `ajenti-panel-2.2.6/aj/plugins.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/routing.py` & `ajenti-panel-2.2.6/aj/routing.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/security/pwreset.py` & `ajenti-panel-2.2.6/aj/security/pwreset.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/security/totp.py` & `ajenti-panel-2.2.6/aj/security/totp.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/security/verifier.py` & `ajenti-panel-2.2.6/aj/security/verifier.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/static/emails/reset_email.html` & `ajenti-panel-2.2.6/aj/static/emails/reset_email.html`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/static/images/Logo.png` & `ajenti-panel-2.2.6/aj/static/images/Logo.png`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/static/images/error.jpeg` & `ajenti-panel-2.2.6/aj/static/images/error.jpeg`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/util/lazy.py` & `ajenti-panel-2.2.6/aj/util/lazy.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/util/misc.py` & `ajenti-panel-2.2.6/aj/util/misc.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/util/pidfile.py` & `ajenti-panel-2.2.6/aj/util/pidfile.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/util/public.py` & `ajenti-panel-2.2.6/aj/util/public.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/aj/wsgi.py` & `ajenti-panel-2.2.6/aj/wsgi.py`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/ajenti-client-ssl-gen` & `ajenti-panel-2.2.6/ajenti-client-ssl-gen`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/ajenti-panel` & `ajenti-panel-2.2.6/ajenti-panel`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/ajenti-ssl-gen` & `ajenti-panel-2.2.6/ajenti-ssl-gen`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/ajenti-upgrade` & `ajenti-panel-2.2.6/ajenti-upgrade`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/ajenti_panel.egg-info/SOURCES.txt` & `ajenti-panel-2.2.6/ajenti_panel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ajenti-panel-2.2.5/setup.py` & `ajenti-panel-2.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,18 +54,18 @@
     def run(self):
         _install.run(self)
         self.execute(_post_install, [self.install_scripts], msg='Running post install script')
 
 
 setup(
     name='ajenti-panel',
-    version='2.2.5',
+    version='2.2.6',
     python_requires='>=3',
     install_requires=[
-        'aj==2.2.5',
+        'aj==2.2.6',
         'pyyaml',
         'requests',
     ],
     description='Ajenti core based panel',
     author='Eugene Pankov',
     author_email='e@ajenti.org',
     url='https://ajenti.org/',
```

