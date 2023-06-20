# Comparing `tmp/django-forbid-0.1.5.tar.gz` & `tmp/django-forbid-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-forbid-0.1.5.tar", last modified: Sat Jun 17 16:59:34 2023, max compression
+gzip compressed data, was "django-forbid-0.1.6.tar", last modified: Tue Jun 20 15:23:57 2023, max compression
```

## Comparing `django-forbid-0.1.5.tar` & `django-forbid-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-17 16:59:24.000000 django-forbid-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-17 16:59:24.000000 django-forbid-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-17 16:59:34.531720 django-forbid-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-17 16:59:24.000000 django-forbid-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-17 16:59:24.000000 django-forbid-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-17 16:59:34.535720 django-forbid-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-17 16:59:24.000000 django-forbid-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid/skills/
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/forbid_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/forbid_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/skills/forbid_network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-17 16:59:24.000000 django-forbid-0.1.5/src/django_forbid/templates/timezone.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-17 16:59:34.531720 django-forbid-0.1.5/src/django_forbid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-17 16:59:34.000000 django-forbid-0.1.5/src/django_forbid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:57.016050 django-forbid-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-20 15:23:47.000000 django-forbid-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 15:23:47.000000 django-forbid-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-20 15:23:57.020050 django-forbid-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-20 15:23:47.000000 django-forbid-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-20 15:23:47.000000 django-forbid-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-20 15:23:57.020050 django-forbid-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-20 15:23:47.000000 django-forbid-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:57.016050 django-forbid-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:57.016050 django-forbid-0.1.6/src/django_forbid/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:57.016050 django-forbid-0.1.6/src/django_forbid/skills/
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/skills/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/skills/forbid_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/skills/forbid_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/skills/forbid_network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:57.016050 django-forbid-0.1.6/src/django_forbid/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-20 15:23:47.000000 django-forbid-0.1.6/src/django_forbid/templates/timezone.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 15:23:57.016050 django-forbid-0.1.6/src/django_forbid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6041 2023-06-20 15:23:56.000000 django-forbid-0.1.6/src/django_forbid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-06-20 15:23:56.000000 django-forbid-0.1.6/src/django_forbid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:23:56.000000 django-forbid-0.1.6/src/django_forbid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 15:23:56.000000 django-forbid-0.1.6/src/django_forbid.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-20 15:23:56.000000 django-forbid-0.1.6/src/django_forbid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-20 15:23:56.000000 django-forbid-0.1.6/src/django_forbid.egg-info/top_level.txt
```

### Comparing `django-forbid-0.1.5/LICENSE` & `django-forbid-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.5/PKG-INFO` & `django-forbid-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.5
+Version: 0.1.6
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
@@ -15,16 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `django-forbid-0.1.5/README.md` & `django-forbid-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.5/setup.cfg` & `django-forbid-0.1.6/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 	Operating System :: OS Independent
 	Development Status :: 5 - Production/Stable
 	Framework :: Django
 	Framework :: Django :: 2.1
 	Framework :: Django :: 2.2
 	Framework :: Django :: 3.1
 	Framework :: Django :: 3.2
-	Framework :: Django :: 4.0
 	Framework :: Django :: 4.1
+	Framework :: Django :: 4.2
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `django-forbid-0.1.5/src/django_forbid/middleware.py` & `django-forbid-0.1.6/src/django_forbid/middleware.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.5/src/django_forbid/skills/__init__.py` & `django-forbid-0.1.6/src/django_forbid/skills/__init__.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.5/src/django_forbid/skills/forbid_device.py` & `django-forbid-0.1.6/src/django_forbid/skills/forbid_device.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,28 +19,33 @@
             "smart speaker": "speaker",
             "feature phone": "phone",
             "car browser": "car",
         }
 
         devices = Settings.get("DEVICES", [])
         device_type = request.session.get("DEVICE")
+        http_ua = request.META.get("HTTP_USER_AGENT")
+        verified_ua = request.session.get("VERIFIED_UA", "")
 
-        # Skip if DEVICES empty.
-        if not devices:
+        # Skips if DEVICES empty or user agent is verified.
+        if not devices or verified_ua == http_ua:
             return self.get_response(request)
 
         if not device_type:
-            http_ua = request.META.get("HTTP_USER_AGENT")
             device_detector = DeviceDetector(http_ua)
             device_detector = device_detector.parse()
             device = device_detector.device_type()
             device_type = device_aliases.get(device, device)
             request.session["DEVICE"] = device_type
 
         if Access(devices).grants(device_type):
+            request.session["VERIFIED_UA"] = http_ua
             return self.get_response(request)
 
+        # Erases the user agent from the session.
+        request.session["VERIFIED_UA"] = ""
+
         # Redirects to the FORBIDDEN_DEV URL if set.
         if Settings.has("OPTIONS.URL.FORBIDDEN_DEV"):
             return redirect(Settings.get("OPTIONS.URL.FORBIDDEN_DEV"))
 
         return HttpResponseForbidden()
```

### Comparing `django-forbid-0.1.5/src/django_forbid/skills/forbid_location.py` & `django-forbid-0.1.6/src/django_forbid/skills/forbid_location.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,16 @@
         city = dict()
         geoip = GeoIP2()
         address = request.META.get("REMOTE_ADDR")
         address = request.META.get("HTTP_X_FORWARDED_FOR", address)
         client_ip = address.split(",")[0].strip()
         verified_ip = request.session.get("VERIFIED_IP", "")
 
-        if verified_ip and verified_ip == client_ip:
+        # Skips if user IP is verified.
+        if verified_ip == client_ip:
             return self.get_response(request)
 
         try:
             city = geoip.city(client_ip)
 
             countries = Settings.get("COUNTRIES", [])
             territories = Settings.get("TERRITORIES", [])
```

### Comparing `django-forbid-0.1.5/src/django_forbid/skills/forbid_network.py` & `django-forbid-0.1.6/src/django_forbid/skills/forbid_network.py`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.5/src/django_forbid/templates/timezone.html` & `django-forbid-0.1.6/src/django_forbid/templates/timezone.html`

 * *Files identical despite different names*

### Comparing `django-forbid-0.1.5/src/django_forbid.egg-info/PKG-INFO` & `django-forbid-0.1.6/src/django_forbid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-forbid
-Version: 0.1.5
+Version: 0.1.6
 Summary: Secure your Django app by controlling the access - grant or deny user access based on device and location, including VPN detection.
 Author: Artyom Vancyan
 Author-email: artyom@pysnippet.org
 License: MIT
 Project-URL: Documentation, https://docs.pysnippet.org/django-forbid/
 Project-URL: Source Code, https://github.com/pysnippet/django-forbid/
 Keywords: python,django,permit,forbid,access,device,secure,country,control,security,location,territory,vpn,detection,django-forbid
@@ -15,16 +15,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
-Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `django-forbid-0.1.5/src/django_forbid.egg-info/SOURCES.txt` & `django-forbid-0.1.6/src/django_forbid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

