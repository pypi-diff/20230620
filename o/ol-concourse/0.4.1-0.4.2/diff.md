# Comparing `tmp/ol-concourse-0.4.1.tar.gz` & `tmp/ol-concourse-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ol-concourse-0.4.1.tar", last modified: Tue Jun 13 20:00:40 2023, max compression
+gzip compressed data, was "ol-concourse-0.4.2.tar", last modified: Tue Jun 20 18:39:17 2023, max compression
```

## Comparing `ol-concourse-0.4.1.tar` & `ol-concourse-0.4.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/MANIFEST.in
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       86 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/PKG-INFO
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      762 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/backend_shim.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/ol_concourse/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/__init__.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/ol_concourse/lib/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/__init__.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       34 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/constants.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1038 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/containers.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/ol_concourse/lib/jobs/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11721 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/jobs/infrastructure.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/ol_concourse/lib/models/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/models/__init__.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3678 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/models/fragment.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)   106719 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/models/pipeline.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      303 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/models/resource.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1188 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/notifications.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2088 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/resource_types.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     4073 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/resources.py
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3199 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/ol_concourse/lib/tasks.py
-drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/ol_concourse.egg-info/
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       86 2023-06-13 20:00:40.000000 ol-concourse-0.4.1/ol_concourse.egg-info/PKG-INFO
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      684 2023-06-13 20:00:40.000000 ol-concourse-0.4.1/ol_concourse.egg-info/SOURCES.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-06-13 20:00:40.000000 ol-concourse-0.4.1/ol_concourse.egg-info/dependency_links.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-06-13 20:00:40.000000 ol-concourse-0.4.1/ol_concourse.egg-info/namespace_packages.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2023-06-13 20:00:40.000000 ol-concourse-0.4.1/ol_concourse.egg-info/requires.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       13 2023-06-13 20:00:40.000000 ol-concourse-0.4.1/ol_concourse.egg-info/top_level.txt
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-06-13 20:00:40.233833 ol-concourse-0.4.1/setup.cfg
--rw-r--r--   0 tmacey    (1000) tmacey    (1000)      498 2023-06-13 20:00:39.000000 ol-concourse-0.4.1/setup.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       12 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/MANIFEST.in
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       79 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      762 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/backend_shim.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.927447 ol-concourse-0.4.2/ol_concourse/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/__init__.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/ol_concourse/lib/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       34 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/constants.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1038 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/containers.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/ol_concourse/lib/jobs/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)    11721 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/jobs/infrastructure.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/ol_concourse/lib/models/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/models/__init__.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3678 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/models/fragment.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)   106719 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/models/pipeline.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      303 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/models/resource.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     1191 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/notifications.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     2088 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/resource_types.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     4073 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/resources.py
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)     3199 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse/lib/tasks.py
+drwxr-xr-x   0 tmacey    (1000) tmacey    (1000)        0 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/ol_concourse.egg-info/
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       79 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse.egg-info/PKG-INFO
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      684 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse.egg-info/SOURCES.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse.egg-info/dependency_links.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)        1 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse.egg-info/namespace_packages.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       19 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse.egg-info/requires.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       13 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/ol_concourse.egg-info/top_level.txt
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)       38 2023-06-20 18:39:17.930781 ol-concourse-0.4.2/setup.cfg
+-rw-r--r--   0 tmacey    (1000) tmacey    (1000)      491 2023-06-20 18:39:17.000000 ol-concourse-0.4.2/setup.py
```

### Comparing `ol-concourse-0.4.1/backend_shim.py` & `ol-concourse-0.4.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/containers.py` & `ol-concourse-0.4.2/ol_concourse/lib/containers.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/jobs/infrastructure.py` & `ol-concourse-0.4.2/ol_concourse/lib/jobs/infrastructure.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/models/fragment.py` & `ol-concourse-0.4.2/ol_concourse/lib/models/fragment.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/models/pipeline.py` & `ol-concourse-0.4.2/ol_concourse/lib/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/notifications.py` & `ol-concourse-0.4.2/ol_concourse/lib/notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     title: str,
     body: str,
     alert_type: Optional[str] = "default",
 ) -> PutStep:
     """Generate a PutStep for sending notifications (to just slack, for now).
 
     :param resource: The slack_notification_resource object for the pipeline.
-        See src/concourse/lib/resources.py
+        See src/ol_concourse/lib/resources.py
     :param title: The text to send to slack as the 'title' of the notification. The bold
         main line.
     :param body: The text to send to slack as the 'body' of the notification. Additional
         details that are hidden when the alert is collapsed.
     :param alert_type: The type of alert to send. Determined the color of the alert
         in slack.
         See: https://github.com/arbourd/concourse-slack-alert-resource#alert-types.
```

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/resource_types.py` & `ol-concourse-0.4.2/ol_concourse/lib/resource_types.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/resources.py` & `ol-concourse-0.4.2/ol_concourse/lib/resources.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse/lib/tasks.py` & `ol-concourse-0.4.2/ol_concourse/lib/tasks.py`

 * *Files identical despite different names*

### Comparing `ol-concourse-0.4.1/ol_concourse.egg-info/SOURCES.txt` & `ol-concourse-0.4.2/ol_concourse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

