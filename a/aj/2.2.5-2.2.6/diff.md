# Comparing `tmp/aj-2.2.5.tar.gz` & `tmp/aj-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aj-2.2.5.tar", last modified: Mon May  8 04:10:12 2023, max compression
+gzip compressed data, was "aj-2.2.6.tar", last modified: Tue Jun 20 15:33:05 2023, max compression
```

## Comparing `aj-2.2.5.tar` & `aj-2.2.6.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.331717 aj-2.2.5/
--rw-r--r--   0 eugene     (501) staff       (20)       99 2020-04-13 10:52:48.000000 aj-2.2.5/MANIFEST.in
--rw-r--r--   0 eugene     (501) staff       (20)      176 2023-05-08 04:10:12.331792 aj-2.2.5/PKG-INFO
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.326759 aj-2.2.5/aj/
--rw-r--r--   0 eugene     (501) staff       (20)     4243 2023-05-08 04:08:59.000000 aj-2.2.5/aj/__init__.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.328042 aj-2.2.5/aj/api/
--rw-r--r--   0 eugene     (501) staff       (20)      188 2020-04-13 10:52:48.000000 aj-2.2.5/aj/api/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     3940 2023-02-13 11:54:42.000000 aj-2.2.5/aj/api/endpoint.py
--rw-r--r--   0 eugene     (501) staff       (20)     7176 2023-02-13 11:54:42.000000 aj-2.2.5/aj/api/http.py
--rw-r--r--   0 eugene     (501) staff       (20)     4994 2022-02-17 09:04:54.000000 aj-2.2.5/aj/api/mail.py
--rw-r--r--   0 eugene     (501) staff       (20)     8389 2022-06-28 14:12:43.000000 aj-2.2.5/aj/auth.py
--rw-r--r--   0 eugene     (501) staff       (20)     2161 2022-06-28 14:12:43.000000 aj-2.2.5/aj/compat.py
--rw-r--r--   0 eugene     (501) staff       (20)    12255 2023-02-13 11:54:42.000000 aj-2.2.5/aj/config.py
--rw-r--r--   0 eugene     (501) staff       (20)    10353 2023-01-06 10:26:21.000000 aj-2.2.5/aj/core.py
--rw-r--r--   0 eugene     (501) staff       (20)     1958 2022-02-17 09:04:54.000000 aj-2.2.5/aj/entry.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.329035 aj-2.2.5/aj/gate/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 aj-2.2.5/aj/gate/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     6351 2023-01-06 10:26:21.000000 aj-2.2.5/aj/gate/gate.py
--rw-r--r--   0 eugene     (501) staff       (20)     9770 2023-02-13 11:54:42.000000 aj-2.2.5/aj/gate/middleware.py
--rw-r--r--   0 eugene     (501) staff       (20)     2134 2023-02-13 11:54:42.000000 aj-2.2.5/aj/gate/session.py
--rw-r--r--   0 eugene     (501) staff       (20)     3899 2022-02-17 09:04:54.000000 aj-2.2.5/aj/gate/stream.py
--rw-r--r--   0 eugene     (501) staff       (20)     7857 2023-01-06 10:26:21.000000 aj-2.2.5/aj/gate/worker.py
--rw-r--r--   0 eugene     (501) staff       (20)    13431 2023-02-13 11:54:42.000000 aj-2.2.5/aj/http.py
--rw-r--r--   0 eugene     (501) staff       (20)      856 2022-06-28 14:12:43.000000 aj-2.2.5/aj/https_redirect.py
--rw-r--r--   0 eugene     (501) staff       (20)     4095 2022-06-28 14:12:43.000000 aj-2.2.5/aj/log.py
--rw-r--r--   0 eugene     (501) staff       (20)    10728 2023-02-13 11:54:42.000000 aj-2.2.5/aj/plugins.py
--rw-r--r--   0 eugene     (501) staff       (20)     4533 2023-01-06 10:26:21.000000 aj-2.2.5/aj/routing.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.329904 aj-2.2.5/aj/security/
--rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 aj-2.2.5/aj/security/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)     4395 2022-02-17 09:04:54.000000 aj-2.2.5/aj/security/pwreset.py
--rw-r--r--   0 eugene     (501) staff       (20)      786 2023-01-06 10:26:21.000000 aj-2.2.5/aj/security/totp.py
--rw-r--r--   0 eugene     (501) staff       (20)      802 2022-06-28 14:12:43.000000 aj-2.2.5/aj/security/verifier.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.322978 aj-2.2.5/aj/static/
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.330098 aj-2.2.5/aj/static/emails/
--rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-17 09:04:54.000000 aj-2.2.5/aj/static/emails/reset_email.html
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.330489 aj-2.2.5/aj/static/images/
--rw-r--r--   0 eugene     (501) staff       (20)    19273 2022-02-17 09:04:54.000000 aj-2.2.5/aj/static/images/Logo.png
--rw-r--r--   0 eugene     (501) staff       (20)     3612 2020-04-13 10:52:48.000000 aj-2.2.5/aj/static/images/error.jpeg
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.331569 aj-2.2.5/aj/util/
--rw-r--r--   0 eugene     (501) staff       (20)      340 2020-04-13 10:52:48.000000 aj-2.2.5/aj/util/__init__.py
--rw-r--r--   0 eugene     (501) staff       (20)      402 2020-05-02 13:26:29.000000 aj-2.2.5/aj/util/broadcast_queue.py
--rw-r--r--   0 eugene     (501) staff       (20)      708 2022-02-17 09:04:54.000000 aj-2.2.5/aj/util/lazy.py
--rw-r--r--   0 eugene     (501) staff       (20)     1577 2022-02-17 09:04:54.000000 aj-2.2.5/aj/util/misc.py
--rw-r--r--   0 eugene     (501) staff       (20)     1074 2020-05-02 13:26:29.000000 aj-2.2.5/aj/util/pidfile.py
--rw-r--r--   0 eugene     (501) staff       (20)      527 2020-04-13 10:52:48.000000 aj-2.2.5/aj/util/public.py
--rw-r--r--   0 eugene     (501) staff       (20)      373 2022-06-28 14:12:43.000000 aj-2.2.5/aj/util/strings.py
--rw-r--r--   0 eugene     (501) staff       (20)     2424 2022-06-28 14:12:43.000000 aj-2.2.5/aj/wsgi.py
-drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-05-08 04:10:12.327370 aj-2.2.5/aj.egg-info/
--rw-r--r--   0 eugene     (501) staff       (20)      176 2023-05-08 04:10:12.000000 aj-2.2.5/aj.egg-info/PKG-INFO
--rw-r--r--   0 eugene     (501) staff       (20)      827 2023-05-08 04:10:12.000000 aj-2.2.5/aj.egg-info/SOURCES.txt
--rw-r--r--   0 eugene     (501) staff       (20)        1 2023-05-08 04:10:12.000000 aj-2.2.5/aj.egg-info/dependency_links.txt
--rw-r--r--   0 eugene     (501) staff       (20)      369 2023-05-08 04:10:12.000000 aj-2.2.5/aj.egg-info/requires.txt
--rw-r--r--   0 eugene     (501) staff       (20)        3 2023-05-08 04:10:12.000000 aj-2.2.5/aj.egg-info/top_level.txt
--rw-r--r--   0 eugene     (501) staff       (20)      499 2023-05-08 04:08:59.000000 aj-2.2.5/requirements.txt
--rw-r--r--   0 eugene     (501) staff       (20)       67 2023-05-08 04:10:12.332008 aj-2.2.5/setup.cfg
--rwxr-xr-x   0 eugene     (501) staff       (20)      777 2023-05-08 04:08:59.000000 aj-2.2.5/setup.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.036677 aj-2.2.6/
+-rw-r--r--   0 eugene     (501) staff       (20)       99 2020-04-13 10:52:48.000000 aj-2.2.6/MANIFEST.in
+-rw-r--r--   0 eugene     (501) staff       (20)      176 2023-06-20 15:33:05.036744 aj-2.2.6/PKG-INFO
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.031122 aj-2.2.6/aj/
+-rw-r--r--   0 eugene     (501) staff       (20)     4243 2023-06-20 15:28:29.000000 aj-2.2.6/aj/__init__.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.032496 aj-2.2.6/aj/api/
+-rw-r--r--   0 eugene     (501) staff       (20)      188 2020-04-13 10:52:48.000000 aj-2.2.6/aj/api/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3940 2023-02-13 11:54:42.000000 aj-2.2.6/aj/api/endpoint.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7176 2023-02-13 11:54:42.000000 aj-2.2.6/aj/api/http.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4994 2022-02-17 09:04:54.000000 aj-2.2.6/aj/api/mail.py
+-rw-r--r--   0 eugene     (501) staff       (20)     8389 2022-06-28 14:12:43.000000 aj-2.2.6/aj/auth.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2161 2022-06-28 14:12:43.000000 aj-2.2.6/aj/compat.py
+-rw-r--r--   0 eugene     (501) staff       (20)    12255 2023-02-13 11:54:42.000000 aj-2.2.6/aj/config.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10353 2023-01-06 10:26:21.000000 aj-2.2.6/aj/core.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1958 2022-02-17 09:04:54.000000 aj-2.2.6/aj/entry.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.033952 aj-2.2.6/aj/gate/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 aj-2.2.6/aj/gate/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     6351 2023-01-06 10:26:21.000000 aj-2.2.6/aj/gate/gate.py
+-rw-r--r--   0 eugene     (501) staff       (20)     9700 2023-06-20 15:28:29.000000 aj-2.2.6/aj/gate/middleware.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2172 2023-06-20 15:28:29.000000 aj-2.2.6/aj/gate/session.py
+-rw-r--r--   0 eugene     (501) staff       (20)     3899 2022-02-17 09:04:54.000000 aj-2.2.6/aj/gate/stream.py
+-rw-r--r--   0 eugene     (501) staff       (20)     7857 2023-01-06 10:26:21.000000 aj-2.2.6/aj/gate/worker.py
+-rw-r--r--   0 eugene     (501) staff       (20)    13431 2023-02-13 11:54:42.000000 aj-2.2.6/aj/http.py
+-rw-r--r--   0 eugene     (501) staff       (20)      856 2022-06-28 14:12:43.000000 aj-2.2.6/aj/https_redirect.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4095 2022-06-28 14:12:43.000000 aj-2.2.6/aj/log.py
+-rw-r--r--   0 eugene     (501) staff       (20)    10728 2023-02-13 11:54:42.000000 aj-2.2.6/aj/plugins.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4533 2023-01-06 10:26:21.000000 aj-2.2.6/aj/routing.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.034805 aj-2.2.6/aj/security/
+-rw-r--r--   0 eugene     (501) staff       (20)        0 2020-04-13 10:52:48.000000 aj-2.2.6/aj/security/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)     4395 2022-02-17 09:04:54.000000 aj-2.2.6/aj/security/pwreset.py
+-rw-r--r--   0 eugene     (501) staff       (20)      786 2023-01-06 10:26:21.000000 aj-2.2.6/aj/security/totp.py
+-rw-r--r--   0 eugene     (501) staff       (20)      802 2022-06-28 14:12:43.000000 aj-2.2.6/aj/security/verifier.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.027635 aj-2.2.6/aj/static/
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.034989 aj-2.2.6/aj/static/emails/
+-rw-r--r--   0 eugene     (501) staff       (20)     1680 2022-02-17 09:04:54.000000 aj-2.2.6/aj/static/emails/reset_email.html
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.035477 aj-2.2.6/aj/static/images/
+-rw-r--r--   0 eugene     (501) staff       (20)    19273 2022-02-17 09:04:54.000000 aj-2.2.6/aj/static/images/Logo.png
+-rw-r--r--   0 eugene     (501) staff       (20)     3612 2020-04-13 10:52:48.000000 aj-2.2.6/aj/static/images/error.jpeg
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.036535 aj-2.2.6/aj/util/
+-rw-r--r--   0 eugene     (501) staff       (20)      340 2020-04-13 10:52:48.000000 aj-2.2.6/aj/util/__init__.py
+-rw-r--r--   0 eugene     (501) staff       (20)      402 2020-05-02 13:26:29.000000 aj-2.2.6/aj/util/broadcast_queue.py
+-rw-r--r--   0 eugene     (501) staff       (20)      708 2022-02-17 09:04:54.000000 aj-2.2.6/aj/util/lazy.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1577 2022-02-17 09:04:54.000000 aj-2.2.6/aj/util/misc.py
+-rw-r--r--   0 eugene     (501) staff       (20)     1074 2020-05-02 13:26:29.000000 aj-2.2.6/aj/util/pidfile.py
+-rw-r--r--   0 eugene     (501) staff       (20)      527 2020-04-13 10:52:48.000000 aj-2.2.6/aj/util/public.py
+-rw-r--r--   0 eugene     (501) staff       (20)      373 2022-06-28 14:12:43.000000 aj-2.2.6/aj/util/strings.py
+-rw-r--r--   0 eugene     (501) staff       (20)     2424 2022-06-28 14:12:43.000000 aj-2.2.6/aj/wsgi.py
+drwxr-xr-x   0 eugene     (501) staff       (20)        0 2023-06-20 15:33:05.031800 aj-2.2.6/aj.egg-info/
+-rw-r--r--   0 eugene     (501) staff       (20)      176 2023-06-20 15:33:05.000000 aj-2.2.6/aj.egg-info/PKG-INFO
+-rw-r--r--   0 eugene     (501) staff       (20)      827 2023-06-20 15:33:05.000000 aj-2.2.6/aj.egg-info/SOURCES.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        1 2023-06-20 15:33:05.000000 aj-2.2.6/aj.egg-info/dependency_links.txt
+-rw-r--r--   0 eugene     (501) staff       (20)      369 2023-06-20 15:33:05.000000 aj-2.2.6/aj.egg-info/requires.txt
+-rw-r--r--   0 eugene     (501) staff       (20)        3 2023-06-20 15:33:05.000000 aj-2.2.6/aj.egg-info/top_level.txt
+-rw-r--r--   0 eugene     (501) staff       (20)      499 2023-06-20 15:28:29.000000 aj-2.2.6/requirements.txt
+-rw-r--r--   0 eugene     (501) staff       (20)       67 2023-06-20 15:33:05.036963 aj-2.2.6/setup.cfg
+-rwxr-xr-x   0 eugene     (501) staff       (20)      777 2023-06-20 15:28:29.000000 aj-2.2.6/setup.py
```

### Comparing `aj-2.2.5/aj/__init__.py` & `aj-2.2.6/aj/__init__.py`

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

### Comparing `aj-2.2.5/aj/api/endpoint.py` & `aj-2.2.6/aj/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/api/http.py` & `aj-2.2.6/aj/api/http.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/api/mail.py` & `aj-2.2.6/aj/api/mail.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/auth.py` & `aj-2.2.6/aj/auth.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/compat.py` & `aj-2.2.6/aj/compat.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/config.py` & `aj-2.2.6/aj/config.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/core.py` & `aj-2.2.6/aj/core.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/entry.py` & `aj-2.2.6/aj/entry.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/gate/gate.py` & `aj-2.2.6/aj/gate/gate.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/gate/middleware.py` & `aj-2.2.6/aj/gate/middleware.py`

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

### Comparing `aj-2.2.5/aj/gate/session.py` & `aj-2.2.6/aj/gate/session.py`

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

### Comparing `aj-2.2.5/aj/gate/stream.py` & `aj-2.2.6/aj/gate/stream.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/gate/worker.py` & `aj-2.2.6/aj/gate/worker.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/http.py` & `aj-2.2.6/aj/http.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/https_redirect.py` & `aj-2.2.6/aj/https_redirect.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/log.py` & `aj-2.2.6/aj/log.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/plugins.py` & `aj-2.2.6/aj/plugins.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/routing.py` & `aj-2.2.6/aj/routing.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/security/pwreset.py` & `aj-2.2.6/aj/security/pwreset.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/security/totp.py` & `aj-2.2.6/aj/security/totp.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/security/verifier.py` & `aj-2.2.6/aj/security/verifier.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/static/emails/reset_email.html` & `aj-2.2.6/aj/static/emails/reset_email.html`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/static/images/Logo.png` & `aj-2.2.6/aj/static/images/Logo.png`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/static/images/error.jpeg` & `aj-2.2.6/aj/static/images/error.jpeg`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/util/lazy.py` & `aj-2.2.6/aj/util/lazy.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/util/misc.py` & `aj-2.2.6/aj/util/misc.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/util/pidfile.py` & `aj-2.2.6/aj/util/pidfile.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/util/public.py` & `aj-2.2.6/aj/util/public.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj/wsgi.py` & `aj-2.2.6/aj/wsgi.py`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/aj.egg-info/SOURCES.txt` & `aj-2.2.6/aj.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aj-2.2.5/setup.py` & `aj-2.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     __requires.append('git+git://github.com/schmir/gevent@pypy-hacks')
     __requires.append('git+git://github.com/gevent-on-pypy/pypycore ')
 else:
     __requires.append('gevent>=1')
 
 setup(
     name='aj',
-    version='2.2.5',
+    version='2.2.6',
     python_requires='>=3',
     install_requires=__requires,
     description='Web UI base toolkit',
     author='Eugene Pankov',
     author_email='e@ajenti.org',
     url='https://ajenti.org/',
     packages=find_packages(),
```

