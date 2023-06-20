# Comparing `tmp/user-management-api-0.3.tar.gz` & `tmp/user-management-api-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-management-api-0.3.tar", last modified: Tue Jun 20 14:24:54 2023, max compression
+gzip compressed data, was "user-management-api-0.4.tar", last modified: Tue Jun 20 14:32:29 2023, max compression
```

## Comparing `user-management-api-0.3.tar` & `user-management-api-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.909017 user-management-api-0.3/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:03:12.000000 user-management-api-0.3/LICENSE
--rw-rw-rw-   0        0        0      135 2023-06-20 14:04:38.000000 user-management-api-0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      509 2023-06-20 14:24:54.908017 user-management-api-0.3/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-20 14:02:23.000000 user-management-api-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 14:24:54.909017 user-management-api-0.3/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-06-20 14:22:00.000000 user-management-api-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.899016 user-management-api-0.3/user_management_api/
--rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/admin.py
--rw-rw-rw-   0        0        0      174 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/apps.py
--rw-rw-rw-   0        0        0      840 2023-06-15 11:15:54.000000 user-management-api-0.3/user_management_api/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.907016 user-management-api-0.3/user_management_api/migrations/
--rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/models.py
--rw-rw-rw-   0        0        0      132 2023-06-15 09:51:42.000000 user-management-api-0.3/user_management_api/pagination.py
--rw-rw-rw-   0        0        0     1246 2023-06-15 10:10:39.000000 user-management-api-0.3/user_management_api/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/tests.py
--rw-rw-rw-   0        0        0      430 2023-06-20 14:21:25.000000 user-management-api-0.3/user_management_api/urls.py
--rw-rw-rw-   0        0        0     2964 2023-06-15 11:28:21.000000 user-management-api-0.3/user_management_api/views.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.906016 user-management-api-0.3/user_management_api.egg-info/
--rw-rw-rw-   0        0        0      509 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:32:29.068754 user-management-api-0.4/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:03:12.000000 user-management-api-0.4/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-06-20 14:04:38.000000 user-management-api-0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      509 2023-06-20 14:32:29.068754 user-management-api-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:02:23.000000 user-management-api-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:32:29.068754 user-management-api-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-06-20 14:32:16.000000 user-management-api-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:32:29.053662 user-management-api-0.4/user_management_api/
+-rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.4/user_management_api/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-07 12:31:25.000000 user-management-api-0.4/user_management_api/admin.py
+-rw-rw-rw-   0        0        0      174 2023-03-07 12:31:25.000000 user-management-api-0.4/user_management_api/apps.py
+-rw-rw-rw-   0        0        0      840 2023-06-15 11:15:54.000000 user-management-api-0.4/user_management_api/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:32:29.067755 user-management-api-0.4/user_management_api/migrations/
+-rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.4/user_management_api/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-03-07 12:31:25.000000 user-management-api-0.4/user_management_api/models.py
+-rw-rw-rw-   0        0        0      132 2023-06-15 09:51:42.000000 user-management-api-0.4/user_management_api/pagination.py
+-rw-rw-rw-   0        0        0     1246 2023-06-15 10:10:39.000000 user-management-api-0.4/user_management_api/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-07 12:31:25.000000 user-management-api-0.4/user_management_api/tests.py
+-rw-rw-rw-   0        0        0      430 2023-06-20 14:21:25.000000 user-management-api-0.4/user_management_api/urls.py
+-rw-rw-rw-   0        0        0     2959 2023-06-20 14:31:23.000000 user-management-api-0.4/user_management_api/views.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:32:29.065755 user-management-api-0.4/user_management_api.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-06-20 14:32:28.000000 user-management-api-0.4/user_management_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-20 14:32:28.000000 user-management-api-0.4/user_management_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:32:28.000000 user-management-api-0.4/user_management_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-20 14:32:28.000000 user-management-api-0.4/user_management_api.egg-info/top_level.txt
```

### Comparing `user-management-api-0.3/setup.py` & `user-management-api-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='user-management-api',
-    version='0.3',
+    version='0.4',
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
```

### Comparing `user-management-api-0.3/user_management_api/filters.py` & `user-management-api-0.4/user_management_api/filters.py`

 * *Files identical despite different names*

### Comparing `user-management-api-0.3/user_management_api/serializers.py` & `user-management-api-0.4/user_management_api/serializers.py`

 * *Files identical despite different names*

### Comparing `user-management-api-0.3/user_management_api/views.py` & `user-management-api-0.4/user_management_api/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from rest_framework.response import Response
 from rest_framework.permissions import IsAuthenticated
 # Create your views here.
 from django.contrib.auth import get_user_model
 from rest_framework.viewsets import ModelViewSet
 from rest_framework.permissions import IsAdminUser
 
-from store.pagination import DefaultPagination
+from .pagination import DefaultPagination
 from .filters import UserFilter, GroupFilter
 from .serializers import UserSerializer, UserCreateSerializer, PermissionSerializer
 from django.contrib.auth.models import Group, Permission
 from rest_framework import viewsets
 from .serializers import GroupSerializer
 
 User = get_user_model()
```

### Comparing `user-management-api-0.3/user_management_api.egg-info/SOURCES.txt` & `user-management-api-0.4/user_management_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

