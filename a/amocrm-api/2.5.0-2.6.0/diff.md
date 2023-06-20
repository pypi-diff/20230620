# Comparing `tmp/amocrm_api-2.5.0.tar.gz` & `tmp/amocrm_api-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/amocrm_api-2.5.0.tar", last modified: Sun Aug 28 20:12:52 2022, max compression
+gzip compressed data, was "amocrm_api-2.6.0.tar", last modified: Tue Jun 20 19:49:10 2023, max compression
```

## Comparing `amocrm_api-2.5.0.tar` & `amocrm_api-2.6.0.tar`

### file list

```diff
@@ -1,53 +1,54 @@
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.416976 amocrm_api-2.5.0/
--rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/LICENSE.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)     6723 2022-08-28 20:12:52.417092 amocrm_api-2.5.0/PKG-INFO
--rw-r--r--   0 pandadoc   (501) staff       (20)     5875 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/README.rst
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.406519 amocrm_api-2.5.0/amocrm/
--rw-r--r--   0 pandadoc   (501) staff       (20)      466 2022-08-28 20:09:07.000000 amocrm_api-2.5.0/amocrm/__init__.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.409977 amocrm_api-2.5.0/amocrm/v2/
--rw-r--r--   0 pandadoc   (501) staff       (20)      429 2022-08-28 20:10:58.000000 amocrm_api-2.5.0/amocrm/v2/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1524 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/account.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4638 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/cli.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.413533 amocrm_api-2.5.0/amocrm/v2/entity/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2493 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/call.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1086 2022-08-28 19:28:40.000000 amocrm_api-2.5.0/amocrm/v2/entity/company.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1082 2022-08-28 20:10:58.000000 amocrm_api-2.5.0/amocrm/v2/entity/contact.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     8199 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/custom_field.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1582 2022-08-28 20:10:58.000000 amocrm_api-2.5.0/amocrm/v2/entity/customer.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4932 2022-08-28 19:28:37.000000 amocrm_api-2.5.0/amocrm/v2/entity/events.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1959 2022-08-28 19:28:40.000000 amocrm_api-2.5.0/amocrm/v2/entity/lead.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2520 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/note.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1901 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/pipeline.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1796 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/tag.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2125 2022-08-28 20:10:58.000000 amocrm_api-2.5.0/amocrm/v2/entity/task.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      994 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/entity/user.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1011 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/exceptions.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4945 2022-08-28 19:52:07.000000 amocrm_api-2.5.0/amocrm/v2/fields.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2150 2022-08-28 20:10:58.000000 amocrm_api-2.5.0/amocrm/v2/filters.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     5067 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/interaction.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      882 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/links.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1120 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/manager.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2286 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/model.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      377 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/register.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     5626 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/amocrm/v2/tokens.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.414678 amocrm_api-2.5.0/amocrm_api.egg-info/
--rw-r--r--   0 pandadoc   (501) staff       (20)     6723 2022-08-28 20:12:52.000000 amocrm_api-2.5.0/amocrm_api.egg-info/PKG-INFO
--rw-r--r--   0 pandadoc   (501) staff       (20)     1057 2022-08-28 20:12:52.000000 amocrm_api-2.5.0/amocrm_api.egg-info/SOURCES.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        1 2022-08-28 20:12:52.000000 amocrm_api-2.5.0/amocrm_api.egg-info/dependency_links.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       48 2022-08-28 20:12:52.000000 amocrm_api-2.5.0/amocrm_api.egg-info/entry_points.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       37 2022-08-28 20:12:52.000000 amocrm_api-2.5.0/amocrm_api.egg-info/requires.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       13 2022-08-28 20:12:52.000000 amocrm_api-2.5.0/amocrm_api.egg-info/top_level.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)       80 2022-08-28 20:12:52.417429 amocrm_api-2.5.0/setup.cfg
--rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/setup.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.415832 amocrm_api-2.5.0/tests/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      688 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/conftest.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2022-08-28 20:12:52.416781 amocrm_api-2.5.0/tests/data/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/data/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      683 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/data/companies.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4540 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/data/contacts.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1440 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/data/users.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2993 2022-08-28 20:10:58.000000 amocrm_api-2.5.0/tests/test_contacts.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      512 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/test_user.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      554 2022-05-31 17:55:19.000000 amocrm_api-2.5.0/tests/test_utils.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.553098 amocrm_api-2.6.0/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/LICENSE.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6723 2023-06-20 19:49:10.553216 amocrm_api-2.6.0/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5875 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/README.rst
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.541085 amocrm_api-2.6.0/amocrm/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      466 2023-06-20 19:45:32.000000 amocrm_api-2.6.0/amocrm/__init__.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.545102 amocrm_api-2.6.0/amocrm/v2/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      429 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1524 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/account.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4638 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/cli.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.549187 amocrm_api-2.6.0/amocrm/v2/entity/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2493 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/call.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1086 2022-08-28 19:28:40.000000 amocrm_api-2.6.0/amocrm/v2/entity/company.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1082 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/entity/contact.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8199 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/custom_field.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1582 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/entity/customer.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4932 2022-08-28 19:28:37.000000 amocrm_api-2.6.0/amocrm/v2/entity/events.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1959 2022-08-28 19:28:40.000000 amocrm_api-2.6.0/amocrm/v2/entity/lead.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      908 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/entity/list.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2520 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/note.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1901 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/pipeline.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1852 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/entity/tag.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2125 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/entity/task.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      994 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/entity/user.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1011 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/exceptions.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4945 2022-08-28 19:52:07.000000 amocrm_api-2.6.0/amocrm/v2/fields.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2150 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/amocrm/v2/filters.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5075 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/interaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      885 2023-06-20 19:44:04.000000 amocrm_api-2.6.0/amocrm/v2/links.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1120 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/manager.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2286 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/model.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      377 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/register.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5626 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/amocrm/v2/tokens.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.550663 amocrm_api-2.6.0/amocrm_api.egg-info/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6723 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1082 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/SOURCES.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/dependency_links.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       48 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/entry_points.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       37 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/requires.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       13 2023-06-20 19:49:10.000000 amocrm_api-2.6.0/amocrm_api.egg-info/top_level.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)       80 2023-06-20 19:49:10.553587 amocrm_api-2.6.0/setup.cfg
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/setup.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.551905 amocrm_api-2.6.0/tests/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      688 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/conftest.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-06-20 19:49:10.552865 amocrm_api-2.6.0/tests/data/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      683 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/companies.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4540 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/contacts.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1440 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/data/users.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2993 2022-08-28 20:10:58.000000 amocrm_api-2.6.0/tests/test_contacts.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      512 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/test_user.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      554 2022-05-31 17:55:19.000000 amocrm_api-2.6.0/tests/test_utils.py
```

### Comparing `amocrm_api-2.5.0/LICENSE.txt` & `amocrm_api-2.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/PKG-INFO` & `amocrm_api-2.6.0/amocrm_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: amocrm_api
-Version: 2.5.0
+Name: amocrm-api
+Version: 2.6.0
 Summary: Python API for Amocrm
 Home-page: https://github.com/Krukov/amocrm_api
-Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.5.0
+Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.6.0
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `amocrm_api-2.5.0/README.rst` & `amocrm_api-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/account.py` & `amocrm_api-2.6.0/amocrm/v2/account.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/cli.py` & `amocrm_api-2.6.0/amocrm/v2/cli.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/call.py` & `amocrm_api-2.6.0/amocrm/v2/entity/call.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/company.py` & `amocrm_api-2.6.0/amocrm/v2/entity/company.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/contact.py` & `amocrm_api-2.6.0/amocrm/v2/entity/contact.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/custom_field.py` & `amocrm_api-2.6.0/amocrm/v2/entity/custom_field.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/customer.py` & `amocrm_api-2.6.0/amocrm/v2/entity/customer.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/events.py` & `amocrm_api-2.6.0/amocrm/v2/entity/events.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/lead.py` & `amocrm_api-2.6.0/amocrm/v2/entity/lead.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/note.py` & `amocrm_api-2.6.0/amocrm/v2/entity/note.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/pipeline.py` & `amocrm_api-2.6.0/amocrm/v2/entity/pipeline.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/tag.py` & `amocrm_api-2.6.0/amocrm/v2/entity/tag.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from .. import fields, manager, model
 from ..interaction import GenericInteraction
 
 
 class Tag(model.Model):
     name = fields._Field("name")
 
-    leads = manager.Manager(GenericInteraction(path="leads/tags"))
-    contacts = manager.Manager(GenericInteraction(path="contacts/tags"))
-    companies = manager.Manager(GenericInteraction(path="companies/tags"))
-    customers = manager.Manager(GenericInteraction(path="customers/tags"))
+    leads = manager.Manager(GenericInteraction(path="leads/tags", field="tags"))
+    contacts = manager.Manager(GenericInteraction(path="contacts/tags", field="tags"))
+    companies = manager.Manager(GenericInteraction(path="companies/tags", field="tags"))
+    customers = manager.Manager(GenericInteraction(path="customers/tags", field="tags"))
 
 
 class _TagsList:
     def __init__(self, tags, on_change):
         """
         BAD CODE THERE
         self._tags is mutable object and this class and arch play with it
```

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/task.py` & `amocrm_api-2.6.0/amocrm/v2/entity/task.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/entity/user.py` & `amocrm_api-2.6.0/amocrm/v2/entity/user.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/exceptions.py` & `amocrm_api-2.6.0/amocrm/v2/exceptions.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/fields.py` & `amocrm_api-2.6.0/amocrm/v2/fields.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/filters.py` & `amocrm_api-2.6.0/amocrm/v2/filters.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/interaction.py` & `amocrm_api-2.6.0/amocrm/v2/interaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
         while True:
             response, _ = self._list(
                 path, page, include=include, query=query, filters=filters, order=order, limit=limit
             )
             if response is None:
                 return
             yield response["_embedded"]
-            if "next" not in response["_links"]:
+            if "next" not in response.get("_links", []):
                 return
             page += 1
 
 
 class GenericInteraction(BaseInteraction):
     path = ""
     field = None
```

### Comparing `amocrm_api-2.5.0/amocrm/v2/links.py` & `amocrm_api-2.6.0/amocrm/v2/links.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,12 +10,12 @@
         return self._set("link", for_entity, to_entity)
 
     def _set(self, direction, for_entity, to_entity, main=False, metadata=None):
         path = "{}/{}/{}".format(for_entity._path, for_entity.id, direction)
         data = {"to_entity_id": to_entity.id, "to_entity_type": to_entity._path}
         if main:
             metadata = metadata or {}
-            metadata["main"] = True
+            metadata["is_main"] = True
         data["metadata"] = metadata
         response, status = self.request("post", path, data=[data])
         if status == 400:
             raise exceptions.ValidationError(response)
```

### Comparing `amocrm_api-2.5.0/amocrm/v2/manager.py` & `amocrm_api-2.6.0/amocrm/v2/manager.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/model.py` & `amocrm_api-2.6.0/amocrm/v2/model.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm/v2/tokens.py` & `amocrm_api-2.6.0/amocrm/v2/tokens.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/amocrm_api.egg-info/PKG-INFO` & `amocrm_api-2.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: amocrm-api
-Version: 2.5.0
+Name: amocrm_api
+Version: 2.6.0
 Summary: Python API for Amocrm
 Home-page: https://github.com/Krukov/amocrm_api
-Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.5.0
+Download-URL: https://github.com/Krukov/amocrm_api/tarball/2.6.0
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT license
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `amocrm_api-2.5.0/amocrm_api.egg-info/SOURCES.txt` & `amocrm_api-2.6.0/amocrm_api.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 amocrm/v2/entity/call.py
 amocrm/v2/entity/company.py
 amocrm/v2/entity/contact.py
 amocrm/v2/entity/custom_field.py
 amocrm/v2/entity/customer.py
 amocrm/v2/entity/events.py
 amocrm/v2/entity/lead.py
+amocrm/v2/entity/list.py
 amocrm/v2/entity/note.py
 amocrm/v2/entity/pipeline.py
 amocrm/v2/entity/tag.py
 amocrm/v2/entity/task.py
 amocrm/v2/entity/user.py
 amocrm_api.egg-info/PKG-INFO
 amocrm_api.egg-info/SOURCES.txt
```

### Comparing `amocrm_api-2.5.0/setup.py` & `amocrm_api-2.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/conftest.py` & `amocrm_api-2.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/data/companies.py` & `amocrm_api-2.6.0/tests/data/companies.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/data/contacts.py` & `amocrm_api-2.6.0/tests/data/contacts.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/data/users.py` & `amocrm_api-2.6.0/tests/data/users.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/test_contacts.py` & `amocrm_api-2.6.0/tests/test_contacts.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/test_user.py` & `amocrm_api-2.6.0/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `amocrm_api-2.5.0/tests/test_utils.py` & `amocrm_api-2.6.0/tests/test_utils.py`

 * *Files identical despite different names*

