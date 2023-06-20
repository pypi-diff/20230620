# Comparing `tmp/user-management-api-0.1.tar.gz` & `tmp/user-management-api-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "user-management-api-0.1.tar", last modified: Sun Jun 18 12:02:03 2023, max compression
+gzip compressed data, was "user-management-api-0.2.tar", last modified: Tue Jun 20 14:11:14 2023, max compression
```

## Comparing `user-management-api-0.1.tar` & `user-management-api-0.2.tar`

### file list

```diff
@@ -1,12 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-18 12:02:03.579388 user-management-api-0.1/
--rw-rw-rw-   0        0        0      135 2023-06-18 11:56:45.000000 user-management-api-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      486 2023-06-18 12:02:03.578389 user-management-api-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-18 12:02:03.560384 user-management-api-0.1/migrations/
--rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.1/migrations/__init__.py
--rw-rw-rw-   0        0        0       42 2023-06-18 12:02:03.579388 user-management-api-0.1/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-06-18 11:59:10.000000 user-management-api-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-18 12:02:03.577384 user-management-api-0.1/user_management_api.egg-info/
--rw-rw-rw-   0        0        0      486 2023-06-18 12:02:03.000000 user-management-api-0.1/user_management_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      215 2023-06-18 12:02:03.000000 user-management-api-0.1/user_management_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-18 12:02:03.000000 user-management-api-0.1/user_management_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-06-18 12:02:03.000000 user-management-api-0.1/user_management_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.990476 user-management-api-0.2/
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:03:12.000000 user-management-api-0.2/LICENSE
+-rw-rw-rw-   0        0        0      135 2023-06-20 14:04:38.000000 user-management-api-0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      509 2023-06-20 14:11:14.989477 user-management-api-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-20 14:02:23.000000 user-management-api-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-20 14:11:14.990476 user-management-api-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-06-20 14:09:18.000000 user-management-api-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.968475 user-management-api-0.2/user_management_api/
+-rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/admin.py
+-rw-rw-rw-   0        0        0      174 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/apps.py
+-rw-rw-rw-   0        0        0      840 2023-06-15 11:15:54.000000 user-management-api-0.2/user_management_api/filters.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.988476 user-management-api-0.2/user_management_api/migrations/
+-rw-rw-rw-   0        0        0        0 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/models.py
+-rw-rw-rw-   0        0        0      132 2023-06-15 09:51:42.000000 user-management-api-0.2/user_management_api/pagination.py
+-rw-rw-rw-   0        0        0     1246 2023-06-15 10:10:39.000000 user-management-api-0.2/user_management_api/serializers.py
+-rw-rw-rw-   0        0        0       63 2023-03-07 12:31:25.000000 user-management-api-0.2/user_management_api/tests.py
+-rw-rw-rw-   0        0        0      437 2023-06-20 14:11:04.000000 user-management-api-0.2/user_management_api/urls.py
+-rw-rw-rw-   0        0        0     2964 2023-06-15 11:28:21.000000 user-management-api-0.2/user_management_api/views.py
+drwxrwxrwx   0        0        0        0 2023-06-20 14:11:14.987476 user-management-api-0.2/user_management_api.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-06-20 14:11:14.000000 user-management-api-0.2/user_management_api.egg-info/top_level.txt
```

### Comparing `user-management-api-0.1/setup.py` & `user-management-api-0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='user-management-api',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     include_package_data=True,
     classifiers=[
         'Environment :: Web Environment',
         'Framework :: Django',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
```

