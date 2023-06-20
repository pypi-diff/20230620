# Comparing `tmp/Cashooo-1.1.1.tar.gz` & `tmp/cashooo-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Cashooo-1.1.1.tar", last modified: Thu Jun 15 21:08:20 2023, max compression
+gzip compressed data, was "cashooo-1.1.2.tar", last modified: Tue Jun 20 05:40:45 2023, max compression
```

## Comparing `Cashooo-1.1.1.tar` & `cashooo-1.1.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 21:08:20.522106 Cashooo-1.1.1/
-drwxrwxrwx   0        0        0        0 2023-06-15 21:08:20.438551 Cashooo-1.1.1/Cashooo/
--rw-rw-rw-   0        0        0       66 2023-06-15 20:50:02.000000 Cashooo-1.1.1/Cashooo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:08:20.512119 Cashooo-1.1.1/Cashooo/mylibrary/
--rw-rw-rw-   0        0        0        0 2023-06-15 21:08:04.000000 Cashooo-1.1.1/Cashooo/mylibrary/__init__.py
--rw-rw-rw-   0        0        0       66 2023-06-15 20:00:33.000000 Cashooo-1.1.1/Cashooo/mylibrary/admin.py
--rw-rw-rw-   0        0        0      167 2023-06-15 20:54:48.000000 Cashooo-1.1.1/Cashooo/mylibrary/apps.py
--rw-rw-rw-   0        0        0      619 2023-06-15 20:00:42.000000 Cashooo-1.1.1/Cashooo/mylibrary/custom_error.py
--rw-rw-rw-   0        0        0      392 2023-06-15 20:00:45.000000 Cashooo-1.1.1/Cashooo/mylibrary/database_connection_error.py
--rw-rw-rw-   0        0        0     2306 2023-06-15 20:00:48.000000 Cashooo-1.1.1/Cashooo/mylibrary/middleware.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:08:20.516111 Cashooo-1.1.1/Cashooo/mylibrary/migrations/
--rw-rw-rw-   0        0        0        0 2023-06-15 19:48:05.000000 Cashooo-1.1.1/Cashooo/mylibrary/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-06-15 19:48:05.000000 Cashooo-1.1.1/Cashooo/mylibrary/models.py
--rw-rw-rw-   0        0        0       63 2023-06-15 19:48:05.000000 Cashooo-1.1.1/Cashooo/mylibrary/tests.py
--rw-rw-rw-   0        0        0      289 2023-06-15 19:52:03.000000 Cashooo-1.1.1/Cashooo/mylibrary/views.py
-drwxrwxrwx   0        0        0        0 2023-06-15 21:08:20.476535 Cashooo-1.1.1/Cashooo.egg-info/
--rw-rw-rw-   0        0        0      332 2023-06-15 21:08:20.000000 Cashooo-1.1.1/Cashooo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      501 2023-06-15 21:08:20.000000 Cashooo-1.1.1/Cashooo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 21:08:20.000000 Cashooo-1.1.1/Cashooo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-06-15 21:08:20.000000 Cashooo-1.1.1/Cashooo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-15 21:08:20.000000 Cashooo-1.1.1/Cashooo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      332 2023-06-15 21:08:20.520109 Cashooo-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-06-15 21:08:20.522106 Cashooo-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0      511 2023-06-15 21:08:12.000000 Cashooo-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.207818 cashooo-1.1.2/
+-rw-rw-rw-   0        0        0      332 2023-06-20 05:40:45.204369 cashooo-1.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.082512 cashooo-1.1.2/casho/
+-rw-rw-rw-   0        0        0       92 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.092345 cashooo-1.1.2/casho/mylibrary/
+-rw-rw-rw-   0        0        0       71 2023-06-20 05:31:34.000000 cashooo-1.1.2/casho/mylibrary/__init__.py
+-rw-rw-rw-   0        0        0      165 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.107443 cashooo-1.1.2/casho/mylibrary/errors/
+-rw-rw-rw-   0        0        0      114 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/errors/__init__.py
+-rw-rw-rw-   0        0        0      619 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/errors/custom_error.py
+-rw-rw-rw-   0        0        0      392 2023-06-18 09:23:40.000000 cashooo-1.1.2/casho/mylibrary/errors/database_connection_error.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.119814 cashooo-1.1.2/casho/mylibrary/middlewares/
+-rw-rw-rw-   0        0        0       97 2023-06-18 09:23:41.000000 cashooo-1.1.2/casho/mylibrary/middlewares/__init__.py
+-rw-rw-rw-   0        0        0      626 2023-06-18 09:23:41.000000 cashooo-1.1.2/casho/mylibrary/middlewares/errorhandler.py
+-rw-rw-rw-   0        0        0     1713 2023-06-18 09:23:41.000000 cashooo-1.1.2/casho/mylibrary/middlewares/healthcheck.py
+drwxrwxrwx   0        0        0        0 2023-06-20 05:40:45.199098 cashooo-1.1.2/cashooo.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      485 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-20 05:40:44.000000 cashooo-1.1.2/cashooo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 05:40:45.210359 cashooo-1.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      538 2023-06-20 05:27:25.000000 cashooo-1.1.2/setup.py
```

### Comparing `Cashooo-1.1.1/Cashooo/mylibrary/custom_error.py` & `cashooo-1.1.2/casho/mylibrary/errors/custom_error.py`

 * *Files identical despite different names*

### Comparing `Cashooo-1.1.1/Cashooo/mylibrary/middleware.py` & `cashooo-1.1.2/casho/mylibrary/middlewares/healthcheck.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,14 @@
 # middleware.py
 import logging
 from django.http import JsonResponse, HttpResponseServerError
-from .custom_error import CustomError
 
 logger = logging.getLogger()
 
 
-class ErrorHandlingMiddleware:
-    def __init__(self, get_response):
-        self.get_response = get_response
-
-    def __call__(self, request):
-        response = self.get_response(request)
-        return response
-
-    def process_exception(self, request, exception):
-        if isinstance(exception, CustomError):
-            return JsonResponse({'errors': exception.serialize_errors()}, safe=False, status=exception.status_code)
-        else:
-            return JsonResponse([{'message': 'something went wrong.'}], safe=False, status=400)
 
 
 class HealthCheckMiddleware(object):
     def __init__(self, get_response):
         self.get_response = get_response
         # One-time configuration and initialization.
```

