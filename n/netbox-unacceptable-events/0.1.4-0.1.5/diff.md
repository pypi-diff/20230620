# Comparing `tmp/netbox-unacceptable-events-0.1.4.tar.gz` & `tmp/netbox-unacceptable-events-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-unacceptable-events-0.1.4.tar", last modified: Fri Jun  2 09:08:57 2023, max compression
+gzip compressed data, was "netbox-unacceptable-events-0.1.5.tar", last modified: Tue Jun 20 07:42:13 2023, max compression
```

## Comparing `netbox-unacceptable-events-0.1.4.tar` & `netbox-unacceptable-events-0.1.5.tar`

### file list

```diff
@@ -1,41 +1,45 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/
--rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-01-16 15:39:22.000000 netbox-unacceptable-events-0.1.4/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)       34 2023-01-17 08:39:39.000000 netbox-unacceptable-events-0.1.4/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)      972 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      306 2023-01-18 07:35:37.000000 netbox-unacceptable-events-0.1.4/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.860792 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)      972 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1039 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-17 07:10:02.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-06-02 09:08:57.000000 netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.864792 netbox-unacceptable-events-0.1.4/ptuevents/
--rw-rw-r--   0 user      (1000) user      (1000)      404 2023-01-17 08:39:52.000000 netbox-unacceptable-events-0.1.4/ptuevents/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.864792 netbox-unacceptable-events-0.1.4/ptuevents/api/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-24 15:50:18.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     5004 2023-01-18 07:20:21.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/serializers.py
--rw-rw-r--   0 user      (1000) user      (1000)      500 2023-01-17 13:07:51.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     1442 2023-01-19 22:25:09.000000 netbox-unacceptable-events-0.1.4/ptuevents/api/views.py
--rw-rw-r--   0 user      (1000) user      (1000)     1817 2023-01-19 22:26:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/filtersets.py
--rw-rw-r--   0 user      (1000) user      (1000)     1582 2023-05-26 10:25:54.000000 netbox-unacceptable-events-0.1.4/ptuevents/forms.py
--rw-rw-r--   0 user      (1000) user      (1000)     1665 2023-01-19 21:37:38.000000 netbox-unacceptable-events-0.1.4/ptuevents/graphql.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/ptuevents/migrations/
--rw-rw-r--   0 user      (1000) user      (1000)     5433 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/migrations/0001_initial.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/migrations/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4736 2023-05-26 08:55:41.000000 netbox-unacceptable-events-0.1.4/ptuevents/models.py
--rw-rw-r--   0 user      (1000) user      (1000)     1223 2023-01-17 13:21:59.000000 netbox-unacceptable-events-0.1.4/ptuevents/navigation.py
--rw-rw-r--   0 user      (1000) user      (1000)     2179 2023-01-17 13:49:46.000000 netbox-unacceptable-events-0.1.4/ptuevents/tables.py
--rw-rw-r--   0 user      (1000) user      (1000)     3877 2023-01-17 14:20:24.000000 netbox-unacceptable-events-0.1.4/ptuevents/template_content.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.860792 netbox-unacceptable-events-0.1.4/ptuevents/templates/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/
--rw-rw-r--   0 user      (1000) user      (1000)      604 2023-01-19 22:10:16.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_assignment_edit.html
--rw-rw-r--   0 user      (1000) user      (1000)     1395 2023-01-17 14:25:11.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_panel.html
--rw-rw-r--   0 user      (1000) user      (1000)     1419 2023-01-17 14:07:22.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptappsystem.html
--rw-rw-r--   0 user      (1000) user      (1000)      748 2023-01-17 13:09:14.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent.html
--rw-rw-r--   0 user      (1000) user      (1000)      600 2023-01-17 13:42:03.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
--rw-rw-r--   0 user      (1000) user      (1000)     1502 2023-01-17 13:38:27.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_panel.html
--rw-rw-r--   0 user      (1000) user      (1000)      708 2023-01-17 11:14:00.000000 netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptueventrelation.html
--rw-rw-r--   0 user      (1000) user      (1000)     3081 2023-01-17 13:21:06.000000 netbox-unacceptable-events-0.1.4/ptuevents/urls.py
--rw-rw-r--   0 user      (1000) user      (1000)     5741 2023-01-17 14:28:01.000000 netbox-unacceptable-events-0.1.4/ptuevents/views.py
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-02 09:08:57.868792 netbox-unacceptable-events-0.1.4/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     1014 2023-06-02 07:56:30.000000 netbox-unacceptable-events-0.1.4/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.227031 netbox-unacceptable-events-0.1.5/
+-rw-rw-r--   0 user      (1000) user      (1000)    11357 2023-01-16 15:39:22.000000 netbox-unacceptable-events-0.1.5/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)       34 2023-01-17 08:39:39.000000 netbox-unacceptable-events-0.1.5/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1004 2023-06-20 07:42:13.227031 netbox-unacceptable-events-0.1.5/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      338 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.215031 netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1004 2023-06-20 07:42:13.000000 netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1254 2023-06-20 07:42:13.000000 netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-06-20 07:42:13.000000 netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-01-17 07:10:02.000000 netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-06-20 07:42:13.000000 netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.219030 netbox-unacceptable-events-0.1.5/ptuevents/
+-rw-rw-r--   0 user      (1000) user      (1000)      427 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.223030 netbox-unacceptable-events-0.1.5/ptuevents/api/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-05-24 15:50:18.000000 netbox-unacceptable-events-0.1.5/ptuevents/api/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     8038 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/api/serializers.py
+-rw-rw-r--   0 user      (1000) user      (1000)      704 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/api/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2175 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/api/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2894 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/filtersets.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2592 2023-06-20 07:34:43.000000 netbox-unacceptable-events-0.1.5/ptuevents/forms.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1665 2023-01-19 21:37:38.000000 netbox-unacceptable-events-0.1.5/ptuevents/graphql.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.223030 netbox-unacceptable-events-0.1.5/ptuevents/migrations/
+-rw-rw-r--   0 user      (1000) user      (1000)     9718 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/migrations/0001_initial.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2023-01-17 13:35:06.000000 netbox-unacceptable-events-0.1.5/ptuevents/migrations/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9781 2023-06-20 07:34:19.000000 netbox-unacceptable-events-0.1.5/ptuevents/models.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1920 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/navigation.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3632 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/tables.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3866 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/template_content.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.207031 netbox-unacceptable-events-0.1.5/ptuevents/templates/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-06-20 07:42:13.227031 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/
+-rw-rw-r--   0 user      (1000) user      (1000)      604 2023-01-19 22:10:16.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/appsystem_assignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1395 2023-01-17 14:25:11.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/appsystem_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1419 2023-01-17 14:07:22.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptappsystem.html
+-rw-rw-r--   0 user      (1000) user      (1000)      748 2023-01-17 13:09:14.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptuevent.html
+-rw-rw-r--   0 user      (1000) user      (1000)      600 2023-01-17 13:42:03.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1502 2023-01-17 13:38:27.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptuevent_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)      708 2023-01-17 11:14:00.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptueventrelation.html
+-rw-rw-r--   0 user      (1000) user      (1000)     2312 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptusers.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1752 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptworkstations.html
+-rw-rw-r--   0 user      (1000) user      (1000)      567 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptworkstations_assignment_edit.html
+-rw-rw-r--   0 user      (1000) user      (1000)     1411 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptworkstations_panel.html
+-rw-rw-r--   0 user      (1000) user      (1000)     4823 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/urls.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10554 2023-06-20 07:33:08.000000 netbox-unacceptable-events-0.1.5/ptuevents/views.py
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-06-20 07:42:13.231031 netbox-unacceptable-events-0.1.5/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     1014 2023-06-20 07:40:35.000000 netbox-unacceptable-events-0.1.5/setup.py
```

### Comparing `netbox-unacceptable-events-0.1.4/LICENSE` & `netbox-unacceptable-events-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/PKG-INFO` & `netbox-unacceptable-events-0.1.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-unacceptable-events
-Version: 0.1.4
+Version: 0.1.5
 Summary: Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events
 Download-URL: https://pypi.org/project/netbox-unacceptable-events/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# netbox-plugin-unacceptable-events
+# netbox-plugin-unacceptable-events-users-computers
 
 
 ```bash
-pip3 install netbox-unacceptable-events
+pip3 install netbox-unacceptable-events-users-computers
 ```
 
 
 
 Добавить в файле netbox/netbox/configuration.py
 
 ```
```

### Comparing `netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/PKG-INFO` & `netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-unacceptable-events
-Version: 0.1.4
+Version: 0.1.5
 Summary: Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events
 Download-URL: https://pypi.org/project/netbox-unacceptable-events/
 Author: Oleg Senchenko
 Author-email: senchenkoob@mail.ru
 Maintainer: Oleg Senchenko
 Maintainer-email: senchenkoob@mail.ru
 License: MIT
@@ -12,19 +12,19 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# netbox-plugin-unacceptable-events
+# netbox-plugin-unacceptable-events-users-computers
 
 
 ```bash
-pip3 install netbox-unacceptable-events
+pip3 install netbox-unacceptable-events-users-computers
 ```
 
 
 
 Добавить в файле netbox/netbox/configuration.py
 
 ```
```

### Comparing `netbox-unacceptable-events-0.1.4/netbox_unacceptable_events.egg-info/SOURCES.txt` & `netbox-unacceptable-events-0.1.5/netbox_unacceptable_events.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -25,8 +25,12 @@
 ptuevents/migrations/__init__.py
 ptuevents/templates/ptuevents/appsystem_assignment_edit.html
 ptuevents/templates/ptuevents/appsystem_panel.html
 ptuevents/templates/ptuevents/ptappsystem.html
 ptuevents/templates/ptuevents/ptuevent.html
 ptuevents/templates/ptuevents/ptuevent_assignment_edit.html
 ptuevents/templates/ptuevents/ptuevent_panel.html
-ptuevents/templates/ptuevents/ptueventrelation.html
+ptuevents/templates/ptuevents/ptueventrelation.html
+ptuevents/templates/ptuevents/ptusers.html
+ptuevents/templates/ptuevents/ptworkstations.html
+ptuevents/templates/ptuevents/ptworkstations_assignment_edit.html
+ptuevents/templates/ptuevents/ptworkstations_panel.html
```

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/api/serializers.py` & `netbox-unacceptable-events-0.1.5/ptuevents/api/serializers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from rest_framework import serializers
 from netbox.api.serializers import NetBoxModelSerializer, WritableNestedSerializer
-from ..models import PTUEventRelation, PTUEvent, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment
+from ..models import PTUEventRelation, PTUEvent, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment, PTUsers, PTWorkstations, PTWorkstationsAssignment
 from django.contrib.auth.models import ContentType
 from drf_yasg.utils import swagger_serializer_method
 from netbox.api.fields import ChoiceField, ContentTypeField
 from utilities.api import get_serializer_for_model
 
 
 class NestedPTUEventSerializer(WritableNestedSerializer):
@@ -131,7 +131,87 @@
 
     @swagger_serializer_method(serializer_or_field=serializers.DictField)
     def get_object(self, instance):
         serializer = get_serializer_for_model(
             instance.content_type.model_class(), prefix='Nested')
         context = {'request': self.context['request']}
         return serializer(instance.object, context=context).data
+
+
+class NestedPTUsersSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:ptuevents-api:ptusers-detail'
+    )
+
+    class Meta:
+        model = PTUsers
+        fields = ('id', 'url', 'display', 'name', 'description',
+                  'firstname', 'lastname', 'status', 'sAMAccountName',
+                  'ad_guid', 'vpnIPaddress', 'ad_description',
+                  'position', 'department')
+
+
+class PTUsersSerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:ptuevents-api:ptusers-detail'
+    )
+
+    class Meta:
+        model = PTUsers
+        fields = ('id', 'url', 'display', 'name', 'description',
+                  'firstname', 'lastname', 'status', 'sAMAccountName',
+                  'ad_guid', 'vpnIPaddress', 'ad_description',
+                  'position', 'department')
+
+
+class NestedPTWorkstationsSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:ptuevents-api:ptworkstations-detail'
+    )
+
+    class Meta:
+        model = PTWorkstations
+        fields = ('id', 'url', 'display', 'name', 'description',
+                  'CN', 'DistinguishedName', 'ad_guid', 'ad_description')
+
+
+class PTWorkstationsSerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+        view_name='plugins-api:ptuevents-api:ptworkstations-detail'
+    )
+
+    class Meta:
+        model = PTWorkstations
+        fields = ('id', 'url', 'display', 'name', 'description',
+                  'CN', 'DistinguishedName', 'ad_guid', 'ad_description')
+
+
+class NestedPTWorkstationsAssignmentSerializer(WritableNestedSerializer):
+    url = serializers.HyperlinkedIdentityField(
+            view_name='plugins-api:ptuevents-api:ptworkstations-detail')
+
+    class Meta:
+        model = PTWorkstations
+        fields = ('id', 'url', 'display', 'name', 'description',
+                  'CN', 'DistinguishedName', 'ad_guid', 'ad_description')
+
+
+class PTWorkstationsAssignmentSerializer(NetBoxModelSerializer):
+    url = serializers.HyperlinkedIdentityField(
+            view_name='plugins-api:ptuevents-api:ptworkstationsassignment-detail')
+    content_type = ContentTypeField(queryset=ContentType.objects.all())
+    object = serializers.SerializerMethodField(read_only=True)
+    pt_workstations = NestedPTWorkstationsAssignmentSerializer()
+
+    class Meta:
+        model = PTWorkstationsAssignment
+        fields = [
+            'id', 'url', 'display', 'content_type', 'object_id', 'object', 'pt_workstations', 'created', 'last_updated',
+        ]
+
+    @swagger_serializer_method(serializer_or_field=serializers.DictField)
+    def get_object(self, instance):
+        serializer = get_serializer_for_model(
+            instance.content_type.model_class(), prefix='Nested')
+        context = {'request': self.context['request']}
+        return serializer(instance.object, context=context).data
+
```

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/api/views.py` & `netbox-unacceptable-events-0.1.5/ptuevents/api/views.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .serializers import PTAppSystemSerializer, PTAppSystemAssignmentSerializer
 from netbox.api.viewsets import NetBoxModelViewSet
-from ..models import PTUEventRelation, PTUEvent, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment
-from .serializers import PTUEventRelationSerializer, PTUEventSerializer, PTUEventAssignmentSerializer
+from ..models import PTUEventRelation, PTUEvent, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment, PTUsers, PTWorkstations, PTWorkstationsAssignment
+from .serializers import PTUEventRelationSerializer, PTUEventSerializer, PTUEventAssignmentSerializer, PTUsersSerializer, PTWorkstationsSerializer, PTWorkstationsAssignmentSerializer
 from .. import filtersets
 
 
 class PTUEventListViewSet(NetBoxModelViewSet):
     queryset = PTUEvent.objects.prefetch_related('tags')
     serializer_class = PTUEventSerializer
 
@@ -29,7 +29,25 @@
 
 
 class PTAppSystemAssignmentViewSet(NetBoxModelViewSet):
     queryset = PTAppSystemAssignment.objects.prefetch_related(
         'object', 'app_system')
     serializer_class = PTAppSystemAssignmentSerializer
     filterset_class = filtersets.PTAppSystemAssignmentFilterSet
+
+
+class PTUsersListViewSet(NetBoxModelViewSet):
+    queryset = PTUsers.objects.prefetch_related('tags')
+    serializer_class = PTUsersSerializer
+
+
+class PTWorkstationsListViewSet(NetBoxModelViewSet):
+    queryset = PTWorkstations.objects.prefetch_related('tags')
+    serializer_class = PTWorkstationsSerializer
+
+
+class PTWorkstationsAssignmentViewSet(NetBoxModelViewSet):
+    queryset = PTWorkstationsAssignment.objects.prefetch_related(
+        'object', 'pt_workstations')
+    serializer_class = PTWorkstationsAssignmentSerializer
+    filterset_class = filtersets.PTWorkstationsAssignmentFilterSet
+
```

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/graphql.py` & `netbox-unacceptable-events-0.1.5/ptuevents/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/navigation.py` & `netbox-unacceptable-events-0.1.5/ptuevents/navigation.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,32 @@
         link='plugins:ptuevents:ptappsystem_add',
         title='Add',
         icon_class='mdi mdi-plus-thick',
         color=ButtonColorChoices.GREEN
     )
 ]
 
+PTUsers_buttons = [
+    PluginMenuButton(
+        link='plugins:ptuevents:ptusers_add',
+        title='Add',
+        icon_class='mdi mdi-plus-thick',
+        color=ButtonColorChoices.GREEN
+    )
+]
+
+PTWorkstations_buttons = [
+    PluginMenuButton(
+        link='plugins:ptuevents:ptworkstations_add',
+        title='Add',
+        icon_class='mdi mdi-plus-thick',
+        color=ButtonColorChoices.GREEN
+    )
+]
+
 menu_items = (
     PluginMenuItem(
         link='plugins:ptuevents:ptuevent_list',
         link_text='Events',
         buttons=PTUEvent_buttons
     ),
     PluginMenuItem(
@@ -41,8 +59,18 @@
         buttons=PTUEvent_rel_buttons
     ),
     PluginMenuItem(
         link='plugins:ptuevents:ptappsystem_list',
         link_text='App Systems',
         buttons=appsystem_buttons
     ),
+    PluginMenuItem(
+        link='plugins:ptuevents:ptusers_list',
+        link_text='Users',
+        buttons=PTUsers_buttons
+    ),
+    PluginMenuItem(
+        link='plugins:ptuevents:ptworkstations_list',
+        link_text='Workstations',
+        buttons=PTWorkstations_buttons
+    ),
 )
```

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/tables.py` & `netbox-unacceptable-events-0.1.5/ptuevents/tables.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import django_tables2 as tables
 from netbox.tables import NetBoxTable, columns
-from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment
+from .models import PTUEvent, PTUEventRelation, PTUEventAssignment, PTAppSystem, PTAppSystemAssignment, PTWorkstations, PTUsers
 
 
 class PTUEventTable(NetBoxTable):
     name = tables.Column(
         linkify=True
     )
     # default_action = ChoiceFieldColumn()
@@ -65,7 +65,48 @@
     app_system = tables.Column(linkify=True)
     actions = columns.ActionsColumn(actions=('edit', 'delete'))
 
     class Meta(NetBoxTable.Meta):
         model = PTAppSystemAssignment
         fields = ('pk', 'content_type', 'object', 'app_system', 'actions')
         default_columns = ('pk', 'content_type', 'object', 'app_system')
+
+
+class PTUsersTable(NetBoxTable):
+    name = tables.Column(
+        linkify=True
+    )
+
+    class Meta(NetBoxTable.Meta):
+        model = PTUsers
+        fields = ('pk', 'name', 'sAMAccountName',
+                  'status',
+                  'firstname',
+                  'lastname', 'ad_guid', 'ad_description', 'position', 'department', 'comment',
+                  'vpnIPaddress', 'description')
+        default_columns = ('name', 'sAMAccountName',
+                  'status',
+                  'firstname',
+                  'lastname', 'ad_guid', 'description')
+
+
+class PTWorkstationsTable(NetBoxTable):
+    name = tables.Column(linkify=True)
+
+    class Meta(NetBoxTable.Meta):
+        model = PTWorkstations
+        fields = ('pk', 'name', 'CN', 'DistinguishedName', 'ad_description', 'description')
+        default_columns = ('name', 'CN', 'DistinguishedName', 'ad_description', 'description')
+
+
+class PTWorkstationsAssignmentTable(NetBoxTable):
+    content_type = columns.ContentTypeColumn(verbose_name='Object type')
+    object = tables.Column(linkify=True, orderable=False)
+    app_system = tables.Column(linkify=True)
+    actions = columns.ActionsColumn(actions=('edit', 'delete'))
+
+    class Meta(NetBoxTable.Meta):
+        model = PTAppSystemAssignment
+        fields = ('pk', 'content_type', 'object', 'pt_workstations', 'actions')
+        default_columns = ('pk', 'content_type', 'object', 'pt_workstations')
+
+
```

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/template_content.py` & `netbox-unacceptable-events-0.1.5/ptuevents/template_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from extras.plugins import PluginTemplateExtension
 from django.contrib.contenttypes.models import ContentType
-from .models import PTUEventAssignment, PTAppSystemAssignment, PTAppSystem
+from .models import PTUEventAssignment, PTAppSystemAssignment
 
 
 class PTUEventVMPanel(PluginTemplateExtension):
     model = 'virtualization.virtualmachine'
 
     def right_page(self):
         vm = self.context['object']
@@ -20,14 +20,15 @@
             })
 
         return self.render('ptuevents/ptuevent_panel.html', extra_context={
             'PTUEvents': PTUEvents
         })
 
 
+
 # class PTUEventAppSystemPanel(PluginTemplateExtension):
 #     model = 'PTUEvents.PTAppSystem'
 
 #     def right_page(self):
 #         app_system = self.context['object']
 #         content_type_id = ContentType.objects.get_for_model(
 #             model=app_system).id
@@ -109,7 +110,8 @@
         return self.render('ptuevents/appsystem_panel.html', extra_context={
             'app_systems': AppSystems
         })
 
 
 template_extensions = [AppSystemVMPanel, AppSystemDevicePanel, PTUEventVMPanel,
                        PTUEventDevicePanel]
+
```

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_assignment_edit.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/appsystem_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/appsystem_panel.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/appsystem_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptappsystem.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptappsystem.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptuevent.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptuevent_assignment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptuevent_panel.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptuevent_panel.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/ptuevents/templates/ptuevents/ptueventrelation.html` & `netbox-unacceptable-events-0.1.5/ptuevents/templates/ptuevents/ptueventrelation.html`

 * *Files identical despite different names*

### Comparing `netbox-unacceptable-events-0.1.4/setup.py` & `netbox-unacceptable-events-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='netbox-unacceptable-events',
-    version='0.1.4',
+    version='0.1.5',
     description='Netbox plugin. Assign devices and virtual machines and application systems to information security unacceptable events',
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     download_url='https://pypi.org/project/netbox-unacceptable-events/',
     packages=find_packages(),
     include_package_data=True,
```

