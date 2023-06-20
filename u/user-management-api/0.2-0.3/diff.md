# Comparing `tmp/user-management-api-0.2.tar.gz` & `tmp/user-management-api-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-management-api-0.2.tar", last modified: Tue Jun 20 14:11:14 2023, max compression
+gzip compressed data, was "user-management-api-0.3.tar", last modified: Tue Jun 20 14:24:54 2023, max compression
```

## Comparing `user-management-api-0.2.tar` & `user-management-api-0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.990476 user-management-api-0.2/
--rw-rw-rw-   0        0        0        0 2023-06-20 14:03:12.000000 user-management-api-0.2/LICENSE
--rw-rw-rw-   0        0        0      135 2023-06-20 14:04:38.000000 user-management-api-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      509 2023-06-20 14:11:14.989477 user-management-api-0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-20 14:02:23.000000 user-management-api-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-20 14:11:14.990476 user-management-api-0.2/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-06-20 14:09:18.000000 user-management-api-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.968475 user-management-api-0.2/user_management_api/
--rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/__init__.py
--rw-rw-rw-   0        0        0       66 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/admin.py
--rw-rw-rw-   0        0        0      174 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/apps.py
--rw-rw-rw-   0        0        0      840 2023-06-15 11:15:54.000000 user-management-api-0.2/user_management_api/filters.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.988476 user-management-api-0.2/user_management_api/migrations/
--rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/models.py
--rw-rw-rw-   0        0        0      132 2023-06-15 09:51:42.000000 user-management-api-0.2/user_management_api/pagination.py
--rw-rw-rw-   0        0        0     1246 2023-06-15 10:10:39.000000 user-management-api-0.2/user_management_api/serializers.py
--rw-rw-rw-   0        0        0       63 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/tests.py
--rw-rw-rw-   0        0        0      437 2023-06-20 14:11:04.000000 user-management-api-0.2/user_management_api/urls.py
--rw-rw-rw-   0        0        0     2964 2023-06-15 11:28:21.000000 user-management-api-0.2/user_management_api/views.py
-drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.987476 user-management-api-0.2/user_management_api.egg-info/
--rw-rw-rw-   0        0        0      509 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.909017 user-management-api-0.3/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:03:12.000000 user-management-api-0.3/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-06-20 14:04:38.000000 user-management-api-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      509 2023-06-20 14:24:54.908017 user-management-api-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:02:23.000000 user-management-api-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:24:54.909017 user-management-api-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-06-20 14:22:00.000000 user-management-api-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.899016 user-management-api-0.3/user_management_api/
+-rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/admin.py
+-rw-rw-rw-   0        0        0      174 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/apps.py
+-rw-rw-rw-   0        0        0      840 2023-06-15 11:15:54.000000 user-management-api-0.3/user_management_api/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.907016 user-management-api-0.3/user_management_api/migrations/
+-rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/models.py
+-rw-rw-rw-   0        0        0      132 2023-06-15 09:51:42.000000 user-management-api-0.3/user_management_api/pagination.py
+-rw-rw-rw-   0        0        0     1246 2023-06-15 10:10:39.000000 user-management-api-0.3/user_management_api/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-07 12:31:25.000000 user-management-api-0.3/user_management_api/tests.py
+-rw-rw-rw-   0        0        0      430 2023-06-20 14:21:25.000000 user-management-api-0.3/user_management_api/urls.py
+-rw-rw-rw-   0        0        0     2964 2023-06-15 11:28:21.000000 user-management-api-0.3/user_management_api/views.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:24:54.906016 user-management-api-0.3/user_management_api.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-20 14:24:54.000000 user-management-api-0.3/user_management_api.egg-info/top_level.txt
```

### Comparing `user-management-api-0.2/setup.py` & `user-management-api-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='user-management-api',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
```

### Comparing `user-management-api-0.2/user_management_api/filters.py` & `user-management-api-0.3/user_management_api/filters.py`

 * *Files identical despite different names*

### Comparing `user-management-api-0.2/user_management_api/serializers.py` & `user-management-api-0.3/user_management_api/serializers.py`

 * *Files identical despite different names*

### Comparing `user-management-api-0.2/user_management_api/views.py` & `user-management-api-0.3/user_management_api/views.py`

 * *Files identical despite different names*

### Comparing `user-management-api-0.2/user_management_api.egg-info/SOURCES.txt` & `user-management-api-0.3/user_management_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

