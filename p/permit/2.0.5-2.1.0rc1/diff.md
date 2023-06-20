# Comparing `tmp/permit-2.0.5.tar.gz` & `tmp/permit-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "permit-2.0.5.tar", last modified: Tue Jun 13 07:23:11 2023, max compression
+gzip compressed data, was "permit-2.1.0rc1.tar", last modified: Tue Jun 20 18:53:02 2023, max compression
```

## Comparing `permit-2.0.5.tar` & `permit-2.1.0rc1.tar`

### file list

```diff
@@ -1,59 +1,64 @@
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.562352 permit-2.0.5/
--rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.0.5/LICENSE
--rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.0.5/MANIFEST.in
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-13 07:23:11.562226 permit-2.0.5/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.0.5/README.md
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.558046 permit-2.0.5/permit/
--rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.0.5/permit/__init__.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.560785 permit-2.0.5/permit/api/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.0.5/permit/api/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     4185 2023-06-07 19:13:45.000000 permit-2.0.5/permit/api/api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)    11803 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/base.py
--rw-r--r--   0 asafc      (501) staff       (20)     3862 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/condition_set_rules.py
--rw-r--r--   0 asafc      (501) staff       (20)     6060 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/condition_sets.py
--rw-r--r--   0 asafc      (501) staff       (20)     8347 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/context.py
--rw-r--r--   0 asafc      (501) staff       (20)     6493 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/deprecated.py
--rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.0.5/permit/api/elements.py
--rw-r--r--   0 asafc      (501) staff       (20)     9660 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/environments.py
--rw-r--r--   0 asafc      (501) staff       (20)   137660 2023-06-07 19:13:45.000000 permit-2.0.5/permit/api/models.py
--rw-r--r--   0 asafc      (501) staff       (20)     5706 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/projects.py
--rw-r--r--   0 asafc      (501) staff       (20)     5975 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resource_action_groups.py
--rw-r--r--   0 asafc      (501) staff       (20)     6667 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resource_actions.py
--rw-r--r--   0 asafc      (501) staff       (20)     6990 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resource_attributes.py
--rw-r--r--   0 asafc      (501) staff       (20)     6656 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/resources.py
--rw-r--r--   0 asafc      (501) staff       (20)     5784 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/role_assignments.py
--rw-r--r--   0 asafc      (501) staff       (20)     7383 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/roles.py
--rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.0.5/permit/api/sync_api_client.py
--rw-r--r--   0 asafc      (501) staff       (20)     7447 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/tenants.py
--rw-r--r--   0 asafc      (501) staff       (20)     9737 2023-06-13 07:23:03.000000 permit-2.0.5/permit/api/users.py
--rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.0.5/permit/config.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.561059 permit-2.0.5/permit/enforcement/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.5/permit/enforcement/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     7440 2023-06-13 07:23:03.000000 permit-2.0.5/permit/enforcement/enforcer.py
--rw-r--r--   0 asafc      (501) staff       (20)      742 2022-10-01 21:14:31.000000 permit-2.0.5/permit/enforcement/interfaces.py
--rw-r--r--   0 asafc      (501) staff       (20)     3125 2023-06-13 07:23:03.000000 permit-2.0.5/permit/exceptions.py
--rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.0.5/permit/logger.py
--rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.0.5/permit/permit.py
--rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.0.5/permit/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.561517 permit-2.0.5/permit/utils/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.5/permit/utils/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.0.5/permit/utils/context.py
--rw-r--r--   0 asafc      (501) staff       (20)      625 2023-06-13 07:23:03.000000 permit-2.0.5/permit/utils/deprecation.py
--rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.0.5/permit/utils/dicts.py
--rw-r--r--   0 asafc      (501) staff       (20)     1130 2023-06-13 07:23:03.000000 permit-2.0.5/permit/utils/sync.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.558717 permit-2.0.5/permit.egg-info/
--rw-r--r--   0 asafc      (501) staff       (20)      478 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/PKG-INFO
--rw-r--r--   0 asafc      (501) staff       (20)     1170 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/SOURCES.txt
--rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/dependency_links.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/requires.txt
--rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-13 07:23:11.000000 permit-2.0.5/permit.egg-info/top_level.txt
--rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.0.5/requirements.txt
--rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-13 07:23:11.562388 permit-2.0.5/setup.cfg
--rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-13 07:23:03.000000 permit-2.0.5/setup.py
-drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-13 07:23:11.562077 permit-2.0.5/tests/
--rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.0.5/tests/__init__.py
--rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.0.5/tests/conftest.py
--rw-r--r--   0 asafc      (501) staff       (20)     9506 2023-06-13 07:23:03.000000 permit-2.0.5/tests/test_abac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8890 2023-06-11 08:57:33.000000 permit-2.0.5/tests/test_rbac_e2e.py
--rw-r--r--   0 asafc      (501) staff       (20)     8811 2023-06-12 11:54:30.000000 permit-2.0.5/tests/test_rbac_e2e_sync.py
--rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.0.5/tests/utils.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.495433 permit-2.1.0rc1/
+-rw-r--r--   0 asafc      (501) staff       (20)    11357 2023-05-22 06:43:35.000000 permit-2.1.0rc1/LICENSE
+-rw-r--r--   0 asafc      (501) staff       (20)       30 2022-10-01 21:14:31.000000 permit-2.1.0rc1/MANIFEST.in
+-rw-r--r--   0 asafc      (501) staff       (20)      481 2023-06-20 18:53:02.495302 permit-2.1.0rc1/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)      268 2023-05-22 06:43:35.000000 permit-2.1.0rc1/README.md
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.489837 permit-2.1.0rc1/permit/
+-rw-r--r--   0 asafc      (501) staff       (20)      373 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/__init__.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.493183 permit-2.1.0rc1/permit/api/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/api/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5619 2023-06-15 09:37:28.000000 permit-2.1.0rc1/permit/api/api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)    11803 2023-06-15 09:35:27.000000 permit-2.1.0rc1/permit/api/base.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3862 2023-06-15 09:35:27.000000 permit-2.1.0rc1/permit/api/condition_set_rules.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6060 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/condition_sets.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8347 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6493 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/deprecated.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1946 2023-05-22 12:10:06.000000 permit-2.1.0rc1/permit/api/elements.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9660 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/environments.py
+-rw-r--r--   0 asafc      (501) staff       (20)   157002 2023-06-20 15:27:01.000000 permit-2.1.0rc1/permit/api/models.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5706 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/projects.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3258 2023-06-15 09:42:10.000000 permit-2.1.0rc1/permit/api/relationship_tuples.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7018 2023-06-15 09:36:51.000000 permit-2.1.0rc1/permit/api/resource_action_groups.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6667 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/resource_actions.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6990 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/resource_attributes.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6266 2023-06-15 09:48:58.000000 permit-2.1.0rc1/permit/api/resource_instances.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5783 2023-06-15 09:49:43.000000 permit-2.1.0rc1/permit/api/resource_relations.py
+-rw-r--r--   0 asafc      (501) staff       (20)    12276 2023-06-15 09:50:25.000000 permit-2.1.0rc1/permit/api/resource_roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6656 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/resources.py
+-rw-r--r--   0 asafc      (501) staff       (20)     6107 2023-06-15 09:37:28.000000 permit-2.1.0rc1/permit/api/role_assignments.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7383 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/roles.py
+-rw-r--r--   0 asafc      (501) staff       (20)     5318 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/api/sync_api_client.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7447 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/tenants.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9737 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/api/users.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2039 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/config.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.493466 permit-2.1.0rc1/permit/enforcement/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.1.0rc1/permit/enforcement/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     7440 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/enforcement/enforcer.py
+-rw-r--r--   0 asafc      (501) staff       (20)      793 2023-06-15 09:37:28.000000 permit-2.1.0rc1/permit/enforcement/interfaces.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3125 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/exceptions.py
+-rw-r--r--   0 asafc      (501) staff       (20)      212 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/logger.py
+-rw-r--r--   0 asafc      (501) staff       (20)     3116 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/permit.py
+-rw-r--r--   0 asafc      (501) staff       (20)     2494 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.494004 permit-2.1.0rc1/permit/utils/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.1.0rc1/permit/utils/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)      836 2023-05-22 06:43:35.000000 permit-2.1.0rc1/permit/utils/context.py
+-rw-r--r--   0 asafc      (501) staff       (20)      625 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/utils/deprecation.py
+-rw-r--r--   0 asafc      (501) staff       (20)      444 2022-10-01 21:14:31.000000 permit-2.1.0rc1/permit/utils/dicts.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1130 2023-06-15 09:35:28.000000 permit-2.1.0rc1/permit/utils/sync.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.490304 permit-2.1.0rc1/permit.egg-info/
+-rw-r--r--   0 asafc      (501) staff       (20)      481 2023-06-20 18:53:02.000000 permit-2.1.0rc1/permit.egg-info/PKG-INFO
+-rw-r--r--   0 asafc      (501) staff       (20)     1323 2023-06-20 18:53:02.000000 permit-2.1.0rc1/permit.egg-info/SOURCES.txt
+-rw-r--r--   0 asafc      (501) staff       (20)        1 2023-06-20 18:53:02.000000 permit-2.1.0rc1/permit.egg-info/dependency_links.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-06-20 18:53:02.000000 permit-2.1.0rc1/permit.egg-info/requires.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       13 2023-06-20 18:53:02.000000 permit-2.1.0rc1/permit.egg-info/top_level.txt
+-rw-r--r--   0 asafc      (501) staff       (20)      107 2023-05-22 06:43:35.000000 permit-2.1.0rc1/requirements.txt
+-rw-r--r--   0 asafc      (501) staff       (20)       38 2023-06-20 18:53:02.495483 permit-2.1.0rc1/setup.cfg
+-rw-r--r--   0 asafc      (501) staff       (20)      796 2023-06-20 18:52:02.000000 permit-2.1.0rc1/setup.py
+drwxr-xr-x   0 asafc      (501) staff       (20)        0 2023-06-20 18:53:02.495147 permit-2.1.0rc1/tests/
+-rw-r--r--   0 asafc      (501) staff       (20)        0 2022-10-01 21:14:31.000000 permit-2.1.0rc1/tests/__init__.py
+-rw-r--r--   0 asafc      (501) staff       (20)     1191 2023-05-22 11:43:03.000000 permit-2.1.0rc1/tests/conftest.py
+-rw-r--r--   0 asafc      (501) staff       (20)     9506 2023-06-15 09:35:28.000000 permit-2.1.0rc1/tests/test_abac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8913 2023-06-20 16:51:45.000000 permit-2.1.0rc1/tests/test_rbac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)     8834 2023-06-20 16:52:18.000000 permit-2.1.0rc1/tests/test_rbac_e2e_sync.py
+-rw-r--r--   0 asafc      (501) staff       (20)    25709 2023-06-20 17:33:30.000000 permit-2.1.0rc1/tests/test_rebac_e2e.py
+-rw-r--r--   0 asafc      (501) staff       (20)      323 2023-05-22 06:43:35.000000 permit-2.1.0rc1/tests/utils.py
```

### Comparing `permit-2.0.5/LICENSE` & `permit-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/base.py` & `permit-2.1.0rc1/permit/api/base.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/condition_set_rules.py` & `permit-2.1.0rc1/permit/api/condition_set_rules.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/condition_sets.py` & `permit-2.1.0rc1/permit/api/condition_sets.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/context.py` & `permit-2.1.0rc1/permit/api/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/deprecated.py` & `permit-2.1.0rc1/permit/api/deprecated.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/elements.py` & `permit-2.1.0rc1/permit/api/elements.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/environments.py` & `permit-2.1.0rc1/permit/api/environments.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/models.py` & `permit-2.1.0rc1/permit/api/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
-#   filename:  https://api.stg.permit.io/v2/openapi.json
-#   timestamp: 2023-05-21T09:11:01+00:00
+#   filename:  https://api.permit.io/v2/openapi.json
+#   timestamp: 2023-05-31T09:43:34+00:00
 
 from __future__ import annotations
 
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 from uuid import UUID
@@ -453,14 +453,119 @@
     periodic_update_interval: Optional[float] = Field(
         None,
         description="Polling interval to refresh data from data source",
         title="Periodic Update Interval",
     )
 
 
+class DerivedRoleRule(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    relation: str = Field(..., title="Relation")
+    related_resource: str = Field(..., title="Related Resource")
+    related_role: str = Field(..., title="Related Role")
+
+
+class PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    no_direct_roles_on_object: Optional[bool] = Field(
+        False,
+        description="If true, the derived role will not take action if the resource has any direct role",
+        title="No Direct Roles On Object",
+    )
+
+
+class DerivedRoleRuleCreate(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    role: str = Field(
+        ...,
+        description="the role key that needs to exist on the related resource (from the relation)",
+        title="Role",
+    )
+    on_resource: str = Field(
+        ...,
+        description="the resource key that needs to exist on the related role (from the relation)",
+        title="On Resource",
+    )
+    linked_by_relation: str = Field(
+        ...,
+        description="the relation key that needs to exist between the resource and the related resource",
+        title="Linked By Relation",
+    )
+    when: Optional[PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings] = Field(
+        default_factory=lambda: PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings.parse_obj(
+            {"no_direct_roles_on_object": False}
+        ),
+        description="the settings of the derived role rule",
+        title="When",
+    )
+
+
+class DerivedRoleRuleDelete(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    role: str = Field(
+        ...,
+        description="the role key that needs to exist on the related resource (from the relation)",
+        title="Role",
+    )
+    on_resource: str = Field(
+        ...,
+        description="the resource key that needs to exist on the related role (from the relation)",
+        title="On Resource",
+    )
+    linked_by_relation: str = Field(
+        ...,
+        description="the relation key that needs to exist between the resource and the related resource",
+        title="Linked By Relation",
+    )
+
+
+class DerivedRoleRuleRead(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    role_id: UUID = Field(
+        ...,
+        description="the role id that needs to exist on the related resource (from the relation)",
+        title="Role Id",
+    )
+    resource_id: UUID = Field(
+        ...,
+        description="the resource id that needs to exist on the related role (from the relation)",
+        title="Resource Id",
+    )
+    relation_id: UUID = Field(
+        ...,
+        description="the relation id that needs to exist between the resource and the related resource",
+        title="Relation Id",
+    )
+    role: str = Field(
+        ...,
+        description="the role key that needs to exist on the related resource (from the relation)",
+        title="Role",
+    )
+    on_resource: str = Field(
+        ...,
+        description="the resource key that needs to exist on the related role (from the relation)",
+        title="On Resource",
+    )
+    linked_by_relation: str = Field(
+        ...,
+        description="the relation key that needs to exist between the resource and the related resource",
+        title="Linked By Relation",
+    )
+
+
 class DevLogin(BaseModel):
     class Config:
         extra = Extra.allow
 
     username: str = Field(
         ...,
         description="an email address from which to create a DEV MODE session",
@@ -484,14 +589,65 @@
     LEVEL_2 = "LEVEL_2"
     LEVEL_3 = "LEVEL_3"
     LEVEL_4 = "LEVEL_4"
     HIDDEN = "HIDDEN"
     UNCONFIGURED = "UNCONFIGURED"
 
 
+class PermitBackendSchemasSchemaOpalDataDerivedRoleSettings(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    superseded_by_direct_role: Optional[bool] = Field(
+        False, title="Superseded By Direct Role"
+    )
+
+
+class DerivedRole(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    conditions: Optional[str] = Field(None, title="Conditions")
+    settings: PermitBackendSchemasSchemaOpalDataDerivedRoleSettings
+    rules: List[DerivedRoleRule] = Field(..., title="Rules")
+
+
+class DerivedRoleBlockEdit(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    when: Optional[PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings] = Field(
+        default_factory=lambda: PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings.parse_obj(
+            {"no_direct_roles_on_object": False}
+        ),
+        description="the settings of the derived role",
+        title="When",
+    )
+    users_with_role: Optional[List[DerivedRoleRuleCreate]] = Field(
+        [], description="the rules of the derived role", title="Users With Role"
+    )
+
+
+class DerivedRoleBlockRead(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    when: Optional[PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings] = Field(
+        default_factory=lambda: PermitBackendSchemasSchemaDerivedRoleDerivedRoleSettings.parse_obj(
+            {"no_direct_roles_on_object": False}
+        ),
+        description="the settings of the derived role",
+        title="When",
+    )
+    id: UUID = Field(..., description="The unique id of the derived_role", title="Id")
+    users_with_role: Optional[List[DerivedRoleRuleRead]] = Field(
+        [], description="the rules of the derived role", title="Users With Role"
+    )
+
+
 class ElementsRoleRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str = Field(..., description="The name of the role", title="Name")
     description: Optional[str] = Field(
         None,
@@ -504,14 +660,19 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
+    granted_to: Optional[DerivedRoleBlockRead] = Field(
+        {},
+        description="\n        A derived role defintion block, typically contained whithin a role definition.\n        The derived role is a role that is derived from the role definition.\n        ",
+        title="Granted To",
+    )
     key: str = Field(
         ...,
         description="A URL-friendly name of the role (i.e: slug). You will be able to query later using this key instead of the id (UUID) of the role.",
         title="Key",
     )
     id: UUID = Field(..., description="Unique id of the role", title="Id")
     organization_id: UUID = Field(
@@ -1321,30 +1482,213 @@
     active_policy_repo_id: Optional[UUID] = Field(
         None,
         description="the id of the policy repo to use for this project",
         title="Active Policy Repo Id",
     )
 
 
-class RelationsBlock(BaseModel):
-    pass
+class RelationBlockRead(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    resource_id: UUID = Field(
+        ..., description="Unique id of the relation", title="Resource Id"
+    )
+    resource: str = Field(..., description="The resource key", title="Resource")
+
+
+class RelationCreate(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    key: constr(regex=r"^[A-Za-z0-9\-_]+$") = Field(
+        ...,
+        description="A URL-friendly name of the relation (i.e: slug). You will be able to query later using this key instead of the id (UUID) of the relation.",
+        title="Key",
+    )
+    name: str = Field(..., description="The name of the relation", title="Name")
+    description: Optional[str] = Field(
+        None,
+        description="An optional longer description of what this relation respresents in your system",
+        title="Description",
+    )
+    subject_resource: str = Field(
+        ..., description="The subject resource ID or key", title="Subject Resource"
+    )
+
+
+class RelationRead(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    description: Optional[str] = Field(
+        None,
+        description="An optional longer description of what this relation respresents in your system",
+        title="Description",
+    )
+    subject_resource: str = Field(
+        ..., description="The subject resource ID or key", title="Subject Resource"
+    )
+    key: str = Field(
+        ...,
+        description="A URL-friendly name of the relation (i.e: slug). You will be able to query later using this key instead of the id (UUID) of the relation.",
+        title="Key",
+    )
+    name: str = Field(..., description="The name of the relation", title="Name")
+    id: UUID = Field(..., description="Unique id of the relation", title="Id")
+    organization_id: UUID = Field(
+        ...,
+        description="Unique id of the organization that the relation belongs to.",
+        title="Organization Id",
+    )
+    project_id: UUID = Field(
+        ...,
+        description="Unique id of the project that the relation belongs to.",
+        title="Project Id",
+    )
+    environment_id: UUID = Field(
+        ...,
+        description="Unique id of the environment that the relation belongs to.",
+        title="Environment Id",
+    )
+    created_at: datetime = Field(
+        ...,
+        description="Date and time when the relation was created (ISO_8601 format).",
+        title="Created At",
+    )
+    updated_at: datetime = Field(
+        ...,
+        description="Date and time when the relation was last updated/modified (ISO_8601 format).",
+        title="Updated At",
+    )
+    object_resource_id: UUID = Field(
+        ..., description="The object resource id", title="Object Resource Id"
+    )
+    object_resource: str = Field(
+        ..., description="The object resource key", title="Object Resource"
+    )
+    subject_resource_id: UUID = Field(
+        ..., description="The subject resource id", title="Subject Resource Id"
+    )
+
+
+class RelationshipTupleCreate(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    subject: str = Field(
+        ...,
+        description="the resource instance assigned the new relation (accepts either the resource instance id or resource_key:resource_instance_key)",
+        title="Subject",
+    )
+    relation: str = Field(
+        ...,
+        description="the relation to assign between the subject and object",
+        title="Relation",
+    )
+    object: str = Field(
+        ...,
+        description="the resource instance on which the new relation is assigned (accepts either the resource instance id or resource_key:resource_instance_key)",
+        title="Object",
+    )
+    tenant: Optional[str] = Field(
+        None,
+        description="The tenant the subject and object belong to, if the resource instances don't exist yet, the tenant is required to create them. otherwise it is ignored",
+        title="Tenant",
+    )
+
 
+class RelationshipTupleDelete(BaseModel):
     class Config:
         extra = Extra.allow
 
+    subject: str = Field(
+        ...,
+        description="the resource instance assigned the new relation (accepts either the resource instance id or resource_key:resource_instance_key)",
+        title="Subject",
+    )
+    relation: str = Field(
+        ...,
+        description="the relation to assign between the subject and object",
+        title="Relation",
+    )
+    object: str = Field(
+        ...,
+        description="the resource instance on which the new relation is assigned (accepts either the resource instance id or resource_key:resource_instance_key)",
+        title="Object",
+    )
+
 
 class RelationshipTupleObj(BaseModel):
     class Config:
         extra = Extra.allow
 
     subject_str: str = Field(..., title="Subject Str")
     relation_str: str = Field(..., title="Relation Str")
     object_str: str = Field(..., title="Object Str")
 
 
+class RelationshipTupleRead(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    id: UUID = Field(..., description="Unique id of the relationship tuple", title="Id")
+    subject: str = Field(
+        ...,
+        description="resource_key:resource_instance_key of the subject",
+        title="Subject",
+    )
+    relation: str = Field(
+        ..., description="key of the assigned relation", title="Relation"
+    )
+    object: str = Field(
+        ...,
+        description="resource_key:resource_instance_key of the object",
+        title="Object",
+    )
+    tenant: str = Field(..., description="")
+    subject_id: UUID = Field(
+        ..., description="Unique id of the subject", title="Subject Id"
+    )
+    relation_id: UUID = Field(
+        ..., description="Unique id of the relation", title="Relation Id"
+    )
+    object_id: UUID = Field(
+        ..., description="Unique id of the object", title="Object Id"
+    )
+    tenant_id: UUID = Field(
+        ..., description="Unique id of the tenant", title="Tenant Id"
+    )
+    organization_id: UUID = Field(
+        ...,
+        description="Unique id of the organization that the relationship tuple belongs to.",
+        title="Organization Id",
+    )
+    project_id: UUID = Field(
+        ...,
+        description="Unique id of the project that the relationship tuple belongs to.",
+        title="Project Id",
+    )
+    environment_id: UUID = Field(
+        ...,
+        description="Unique id of the environment that the relationship tuple belongs to.",
+        title="Environment Id",
+    )
+    created_at: datetime = Field(
+        ...,
+        description="Date and time when the relationship tuple was created (ISO_8601 format).",
+        title="Created At",
+    )
+    updated_at: datetime = Field(
+        ...,
+        description="Date and time when the relationship tuple was created (ISO_8601 format).",
+        title="Updated At",
+    )
+
+
 class RemoveRolePermissions(BaseModel):
     class Config:
         extra = Extra.allow
 
     permissions: List[str] = Field(
         ...,
         description='List of permissions to remove from the role. If a permission is not found it is skipped. Each permission can be either a resource action id, or `{resource_key}:{action_key}`,i.e: the "permission name".',
@@ -1447,14 +1791,34 @@
     updated_at: datetime = Field(
         ...,
         description="Date and time when the action group was last updated/modified (ISO_8601 format).",
         title="Updated At",
     )
 
 
+class ResourceActionGroupUpdate(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    name: Optional[str] = Field(
+        None, description="The name of the action group", title="Name"
+    )
+    description: Optional[str] = Field(
+        None,
+        description="An optional longer description of what this action group represents in your system",
+        title="Description",
+    )
+    attributes: Optional[Dict[str, Any]] = Field(
+        None,
+        description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this action group. This metadata can be used to filter action groups using query parameters with attr_ prefix",
+        title="Attributes",
+    )
+    actions: Optional[List[str]] = Field([], title="Actions")
+
+
 class ResourceActionRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str = Field(..., description="The name of the action", title="Name")
     description: Optional[str] = Field(
         None,
@@ -1752,14 +2116,19 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
+    granted_to: Optional[DerivedRoleBlockEdit] = Field(
+        None,
+        description="Derived role that inherit will be applied on this role",
+        title="Granted To",
+    )
 
 
 class ResourceRoleRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: str = Field(..., description="The name of the role", title="Name")
@@ -1774,14 +2143,19 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
+    granted_to: Optional[DerivedRoleBlockRead] = Field(
+        None,
+        description="Derived role that inherit will be applied on this role",
+        title="Granted To",
+    )
     key: str = Field(
         ...,
         description="A URL-friendly name of the role (i.e: slug). You will be able to query later using this key instead of the id (UUID) of the role.",
         title="Key",
     )
     id: UUID = Field(..., description="Unique id of the role", title="Id")
     organization_id: UUID = Field(
@@ -1800,14 +2174,19 @@
         title="Environment Id",
     )
     resource_id: UUID = Field(
         ...,
         description="Unique id of the resource that the role belongs to.",
         title="Resource Id",
     )
+    resource: str = Field(
+        ...,
+        description="The unique resource key that the role belongs to.",
+        title="Resource",
+    )
     created_at: datetime = Field(
         ...,
         description="Date and time when the role was created (ISO_8601 format).",
         title="Created At",
     )
     updated_at: datetime = Field(
         ...,
@@ -1832,21 +2211,27 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
+    granted_to: Optional[DerivedRoleBlockEdit] = Field(
+        None,
+        description="Derived role that inherit will be applied on this role",
+        title="Granted To",
+    )
 
 
 class ResourceTypeData(BaseModel):
     class Config:
         extra = Extra.allow
 
     actions: List[str] = Field(..., title="Actions")
+    derived_roles: Dict[str, DerivedRole] = Field(..., title="Derived Roles")
 
 
 class ResourceTypeObj(BaseModel):
     class Config:
         extra = Extra.allow
 
     id: UUID = Field(..., title="Id")
@@ -1862,35 +2247,58 @@
         extra = Extra.allow
 
     role: str = Field(
         ...,
         description="the role that will be assigned (accepts either the role id or the role key)",
         title="Role",
     )
-    tenant: str = Field(
-        ...,
+    tenant: Optional[str] = Field(
+        None,
         description="the tenant the role is associated with (accepts either the tenant id or the tenant key)",
         title="Tenant",
     )
+    resource_instance: Optional[str] = Field(
+        None,
+        description="the resource instance the role is associated with (accepts either the resource instance id or key using this format resource_type:resource_instance)",
+        title="Resource Instance",
+    )
     user: str = Field(
         ...,
         description="the user the role will be assigned to (accepts either the user id or the user key)",
         title="User",
     )
 
 
 class RoleAssignmentRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     id: UUID = Field(..., description="Unique id of the role assignment", title="Id")
     user: str = Field(..., description="the user the role is assigned to", title="User")
     role: str = Field(..., description="the role that is assigned", title="Role")
-    tenant: str = Field(
-        ..., description="the tenant the role is associated with", title="Tenant"
+    tenant: Optional[str] = Field(
+        None, description="the tenant the role is associated with", title="Tenant"
+    )
+    resource: Optional[str] = Field(
+        None,
+        description="the resource type the role is associated with",
+        title="Resource",
+    )
+    resource_instance: Optional[str] = Field(
+        None,
+        description="the resource instance the role is associated with",
+        title="Resource Instance",
+    )
+    resource_id: Optional[UUID] = Field(
+        None, description="Unique id of the resource type", title="Resource Id"
+    )
+    resource_instance_id: Optional[UUID] = Field(
+        None,
+        description="Unique id of the resource instance",
+        title="Resource Instance Id",
     )
     user_id: UUID = Field(..., description="Unique id of the user", title="User Id")
     role_id: UUID = Field(..., description="Unique id of the role", title="Role Id")
     tenant_id: UUID = Field(
         ..., description="Unique id of the tenant", title="Tenant Id"
     )
     organization_id: UUID = Field(
@@ -1920,40 +2328,56 @@
         extra = Extra.allow
 
     role: str = Field(
         ...,
         description="the role that will be unassigned (accepts either the role id or the role key)",
         title="Role",
     )
-    tenant: str = Field(
-        ...,
+    tenant: Optional[str] = Field(
+        None,
         description="the tenant the role is associated with (accepts either the tenant id or the tenant key)",
         title="Tenant",
     )
+    resource_instance: Optional[str] = Field(
+        None,
+        description="the resource instance the role is associated with (accepts either the resource instance id or key using this format resource_type:resource_instance)",
+        title="Resource Instance",
+    )
     user: str = Field(
         ...,
         description="the user the role will be unassigned from (accepts either the user id or the user key)",
         title="User",
     )
 
 
-class RoleBlock(BaseModel):
+class RoleBlockEditable(BaseModel):
     class Config:
         extra = Extra.allow
 
+    name: str = Field(..., description="The name of the role", title="Name")
     description: Optional[str] = Field(
         None,
         description="optional description string explaining what this role represents, or what permissions are granted to it.",
         title="Description",
     )
     permissions: Optional[List[str]] = Field(
         None,
         description="list of action keys that define what actions this resource role is permitted to do",
         title="Permissions",
     )
+    attributes: Optional[Dict[str, Any]] = Field(
+        None,
+        description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
+        title="Attributes",
+    )
+    granted_to: Optional[DerivedRoleBlockEdit] = Field(
+        None,
+        description="Derived role that inherit will be applied on this role",
+        title="Granted To",
+    )
 
 
 class RoleCreate(BaseModel):
     class Config:
         extra = Extra.allow
 
     key: constr(regex=r"^[A-Za-z0-9\-_]+$") = Field(
@@ -1973,14 +2397,19 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
+    granted_to: Optional[DerivedRoleBlockEdit] = Field(
+        None,
+        description="Derived role that inherit will be applied on this role",
+        title="Granted To",
+    )
 
 
 class RoleData(BaseModel):
     class Config:
         extra = Extra.allow
 
     grants: Optional[Dict[str, List[str]]] = Field(None, title="Grants")
@@ -2002,14 +2431,19 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
+    granted_to: Optional[DerivedRoleBlockRead] = Field(
+        {},
+        description="\n        A derived role defintion block, typically contained whithin a role definition.\n        The derived role is a role that is derived from the role definition.\n        ",
+        title="Granted To",
+    )
     key: str = Field(
         ...,
         description="A URL-friendly name of the role (i.e: slug). You will be able to query later using this key instead of the id (UUID) of the role.",
         title="Key",
     )
     id: UUID = Field(..., description="Unique id of the role", title="Id")
     organization_id: UUID = Field(
@@ -2055,21 +2489,19 @@
         title="Permissions",
     )
     attributes: Optional[Dict[str, Any]] = Field(
         None,
         description="optional dictionary of key-value pairs that can be used to store arbitrary metadata about this role. This metadata can be used to filter role using query parameters with attr_ prefix, currently supports only 'equals' operator",
         title="Attributes",
     )
-
-
-class RolesBlock(BaseModel):
-    pass
-
-    class Config:
-        extra = Extra.allow
+    granted_to: Optional[DerivedRoleBlockEdit] = Field(
+        None,
+        description="Derived role that inherit will be applied on this role",
+        title="Granted To",
+    )
 
 
 class SSHAuthData(BaseModel):
     class Config:
         extra = Extra.allow
 
     auth_type: Optional[Literal["ssh"]] = Field("ssh", title="Auth Type")
@@ -2369,35 +2801,45 @@
         extra = Extra.allow
 
     role: str = Field(
         ...,
         description="the role that will be assigned (accepts either the role id or the role key)",
         title="Role",
     )
-    tenant: str = Field(
-        ...,
+    tenant: Optional[str] = Field(
+        None,
         description="the tenant the role is associated with (accepts either the tenant id or the tenant key)",
         title="Tenant",
     )
+    resource_instance: Optional[str] = Field(
+        None,
+        description="the resource instance the role is associated with (accepts either the resource instance id or key using this format resource_type:resource_instance)",
+        title="Resource Instance",
+    )
 
 
 class UserRoleRemove(BaseModel):
     class Config:
         extra = Extra.allow
 
     role: str = Field(
         ...,
         description="the role that will be unassigned (accepts either the role id or the role key)",
         title="Role",
     )
-    tenant: str = Field(
-        ...,
+    tenant: Optional[str] = Field(
+        None,
         description="the tenant the role is associated with (accepts either the tenant id or the tenant key)",
         title="Tenant",
     )
+    resource_instance: Optional[str] = Field(
+        None,
+        description="the resource instance the role is associated with (accepts either the resource instance id or key using this format resource_type:resource_instance)",
+        title="Resource Instance",
+    )
 
 
 class UserStatus(str, Enum):
     active = "active"
     pending = "pending"
 
 
@@ -2996,16 +3438,22 @@
 
     users: Dict[str, UserData] = Field(..., title="Users")
     tenants: Dict[str, TenantData] = Field(..., title="Tenants")
     roles: Dict[str, RoleData] = Field(..., title="Roles")
     condition_set_rules: Dict[str, Dict[str, Dict[str, List[str]]]] = Field(
         ..., title="Condition Set Rules"
     )
+    relationships: Dict[str, Dict[str, Dict[str, List[str]]]] = Field(
+        ..., title="Relationships"
+    )
     resource_types: Dict[str, ResourceTypeData] = Field(..., title="Resource Types")
     condition_sets: Dict[str, ConditionSetData] = Field(..., title="Condition Sets")
+    role_assignments: Dict[str, Dict[str, List[str]]] = Field(
+        ..., title="Role Assignments"
+    )
 
 
 class HTTPValidationError(BaseModel):
     class Config:
         extra = Extra.allow
 
     detail: Optional[List[ValidationError]] = Field(None, title="Detail")
@@ -3335,14 +3783,23 @@
         extra = Extra.allow
 
     data: List[RoleRead] = Field(..., description="List of Roles", title="Data")
     total_count: conint(ge=0) = Field(..., title="Total Count")
     page_count: Optional[conint(ge=0)] = Field(0, title="Page Count")
 
 
+class PaginatedResultRelationRead(BaseModel):
+    class Config:
+        extra = Extra.allow
+
+    data: List[RelationRead] = Field(..., description="List of Relations", title="Data")
+    total_count: conint(ge=0) = Field(..., title="Total Count")
+    page_count: Optional[conint(ge=0)] = Field(0, title="Page Count")
+
+
 class PaginatedResultTenantRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     data: List[TenantRead] = Field(..., description="List of Tenants", title="Data")
     total_count: conint(ge=0) = Field(..., title="Total Count")
     page_count: Optional[conint(ge=0)] = Field(0, title="Page Count")
@@ -3551,14 +4008,28 @@
         title="Actions",
     )
     attributes: Optional[Dict[str, AttributeBlockEditable]] = Field(
         None,
         description="Attributes that each resource of this type defines, and can be used in your ABAC policies.",
         title="Attributes",
     )
+    roles: Optional[
+        Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), RoleBlockEditable]
+    ] = Field(
+        None,
+        description="Roles defined on this resource. The key is the role name, and the value contains the role properties such as granted permissions, base roles, etc.",
+        title="Roles",
+    )
+    relations: Optional[
+        Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), constr(regex=r"^[A-Za-z0-9\-_]+$")]
+    ] = Field(
+        None,
+        description="Relations to other resources. The key is the relation key, and the value is the related resource.",
+        title="Relations",
+    )
 
 
 class ResourceRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     key: str = Field(
@@ -3605,18 +4076,28 @@
     )
     actions: Optional[Dict[str, ActionBlockRead]] = Field(
         {},
         description="\n        A actions definition block, typically contained within a resource type definition block.\n        The actions represents the ways you can interact with a protected resource.\n        ",
         title="Actions",
     )
     attributes: Optional[Dict[str, AttributeBlockRead]] = Field(
-        {},
+        None,
         description="Attributes that each resource of this type defines, and can be used in your ABAC policies.",
         title="Attributes",
     )
+    roles: Optional[Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), ResourceRoleRead]] = Field(
+        None,
+        description="Roles defined on this resource. The key is the role name, and the value contains the role properties such as granted permissions, etc.",
+        title="Roles",
+    )
+    relations: Optional[Dict[str, RelationBlockRead]] = Field(
+        {},
+        description="\n        A relations definition block, typically contained within a resource type definition block.\n        The relations represents the ways you can interact with a protected resource.\n        ",
+        title="Relations",
+    )
     action_groups: Optional[Dict[str, List[str]]] = Field({}, title="Action Groups")
 
 
 class ResourceReplace(BaseModel):
     class Config:
         extra = Extra.allow
 
@@ -3637,14 +4118,28 @@
         title="Actions",
     )
     attributes: Optional[Dict[str, AttributeBlockEditable]] = Field(
         None,
         description="Attributes that each resource of this type defines, and can be used in your ABAC policies.",
         title="Attributes",
     )
+    roles: Optional[
+        Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), RoleBlockEditable]
+    ] = Field(
+        None,
+        description="Roles defined on this resource. The key is the role name, and the value contains the role properties such as granted permissions, base roles, etc.",
+        title="Roles",
+    )
+    relations: Optional[
+        Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), constr(regex=r"^[A-Za-z0-9\-_]+$")]
+    ] = Field(
+        None,
+        description="Relations to other resources. The key is the relation key, and the value is the related resource.",
+        title="Relations",
+    )
 
 
 class ResourceUpdate(BaseModel):
     class Config:
         extra = Extra.allow
 
     name: Optional[str] = Field(
@@ -3666,14 +4161,28 @@
         title="Actions",
     )
     attributes: Optional[Dict[str, AttributeBlockEditable]] = Field(
         None,
         description="Attributes that each resource of this type defines, and can be used in your ABAC policies.",
         title="Attributes",
     )
+    roles: Optional[
+        Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), RoleBlockEditable]
+    ] = Field(
+        None,
+        description="Roles defined on this resource. The key is the role name, and the value contains the role properties such as granted permissions, base roles, etc.",
+        title="Roles",
+    )
+    relations: Optional[
+        Dict[constr(regex=r"^[A-Za-z0-9\-_]+$"), constr(regex=r"^[A-Za-z0-9\-_]+$")]
+    ] = Field(
+        None,
+        description="Relations to other resources. The key is the relation key, and the value is the related resource.",
+        title="Relations",
+    )
 
 
 class ScopeConfigRead(BaseModel):
     class Config:
         extra = Extra.allow
 
     data: Optional[OpalCommonSchemasDataDataSourceConfig] = None
```

### Comparing `permit-2.0.5/permit/api/projects.py` & `permit-2.1.0rc1/permit/api/projects.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/resource_action_groups.py` & `permit-2.1.0rc1/permit/api/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,163 +6,192 @@
     BasePermitApi,
     SimpleHttpClient,
     pagination_params,
     required_context,
     required_permissions,
 )
 from .context import ApiContextLevel, ApiKeyAccessLevel
-from .models import ResourceActionGroupCreate, ResourceActionGroupRead
+from .models import ResourceCreate, ResourceRead, ResourceReplace, ResourceUpdate
 
 
-class ResourceActionGroupsApi(BasePermitApi):
+class ResourcesApi(BasePermitApi):
     @property
-    def __action_groups(self) -> SimpleHttpClient:
+    def __resources(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/resources".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def list(
-        self, resource_key: str, page: int = 1, per_page: int = 100
-    ) -> List[ResourceActionGroupRead]:
+    async def list(self, page: int = 1, per_page: int = 100) -> List[ResourceRead]:
         """
-        Retrieves a list of action groups.
+        Retrieves a list of resources.
 
         Args:
-            resource_key: The key of the resource to filter on.
             page: The page number to fetch (default: 1).
             per_page: How many items to fetch per page (default: 100).
 
         Returns:
-            an array of action groups.
+            an array of resources.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__action_groups.get(
-            f"/{resource_key}/action_groups",
-            model=List[ResourceActionGroupRead],
+        return await self.__resources.get(
+            "",
+            model=List[ResourceRead],
             params=pagination_params(page, per_page),
         )
 
-    async def _get(self, resource_key: str, group_key: str) -> ResourceActionGroupRead:
-        return await self.__action_groups.get(
-            f"/{resource_key}/action_groups/{group_key}",
-            model=ResourceActionGroupRead,
-        )
+    async def _get(self, resource_key: str) -> ResourceRead:
+        return await self.__resources.get(f"/{resource_key}", model=ResourceRead)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def get(self, resource_key: str, group_key: str) -> ResourceActionGroupRead:
+    async def get(self, resource_key: str) -> ResourceRead:
         """
-        Retrieves a action group by its key.
+        Retrieves a resource by its key.
 
         Args:
-            resource_key: The key of the resource the action group belongs to.
-            group_key: The key of the action group.
+            resource_key: The key of the resource.
 
         Returns:
-            the action group.
+            the resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self._get(resource_key, group_key)
+        return await self._get(resource_key)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def get_by_key(
-        self, resource_key: str, group_key: str
-    ) -> ResourceActionGroupRead:
+    async def get_by_key(self, resource_key: str) -> ResourceRead:
         """
-        Retrieves a action group by its key.
+        Retrieves a resource by its key.
         Alias for the get method.
 
         Args:
-            resource_key: The key of the resource the action group belongs to.
-            group_key: The key of the action group.
+            resource_key: The key of the resource.
 
         Returns:
-            the action group.
+            the resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self._get(resource_key, group_key)
+        return await self._get(resource_key)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def get_by_id(
-        self, resource_id: str, group_id: str
-    ) -> ResourceActionGroupRead:
+    async def get_by_id(self, resource_id: str) -> ResourceRead:
         """
-        Retrieves a action group by its ID.
+        Retrieves a resource by its ID.
         Alias for the get method.
 
         Args:
-            resource_key: The ID of the resource the action group belongs to.
-            group_id: The ID of the action group.
+            resource_id: The ID of the resource.
+
+        Returns:
+            the resource.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self._get(resource_id)
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
+    @validate_arguments
+    async def create(self, resource_data: ResourceCreate) -> ResourceRead:
+        """
+        Creates a new resource.
+
+        Args:
+            resource_data: The data for the new resource.
 
         Returns:
-            the action group.
+            the created resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self._get(resource_id, group_id)
+        return await self.__resources.post("", model=ResourceRead, json=resource_data)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def create(
-        self, resource_key: str, group_data: ResourceActionGroupCreate
-    ) -> ResourceActionGroupRead:
+    async def update(
+        self, resource_key: str, resource_data: ResourceUpdate
+    ) -> ResourceRead:
         """
-        Creates a new action group.
+        Updates a resource.
 
         Args:
-            resource_key: The key of the resource under which the action group should be created.
-            group_data: The data for the new action group.
+            resource_key: The key of the resource.
+            resource_data: The updated data for the resource.
 
         Returns:
-            the created action group.
+            the updated resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__action_groups.post(
-            f"/{resource_key}/action_groups",
-            model=ResourceActionGroupRead,
-            json=group_data,
+        return await self.__resources.patch(
+            f"/{resource_key}",
+            model=ResourceRead,
+            json=resource_data,
         )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def delete(self, resource_key: str, group_key: str) -> None:
+    async def replace(
+        self, resource_key: str, resource_data: ResourceReplace
+    ) -> ResourceRead:
         """
-        Deletes a action group.
+        Creates a resource if no such resource exists, otherwise completely replaces the resource in place.
 
         Args:
-            resource_key: The key of the resource the action group belongs to.
-            group_key: The key of the action group to delete.
+            resource_key: The key of the resource.
+            resource_data: The updated data for the resource.
+
+        Returns:
+            the updated resource.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__action_groups.delete(
-            f"/{resource_key}/action_groups/{group_key}"
+        return await self.__resources.put(
+            f"/{resource_key}",
+            model=ResourceRead,
+            json=resource_data,
         )
+
+    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
+    @required_context(ApiContextLevel.ENVIRONMENT)
+    @validate_arguments
+    async def delete(self, resource_key: str) -> None:
+        """
+        Deletes a resource.
+
+        Args:
+            resource_key: The key of the resource to delete.
+
+        Raises:
+            PermitApiError: If the API returns an error HTTP status code.
+            PermitContextError: If the configured ApiContext does not match the required endpoint context.
+        """
+        return await self.__resources.delete(f"/{resource_key}")
```

### Comparing `permit-2.0.5/permit/api/resource_actions.py` & `permit-2.1.0rc1/permit/api/resource_actions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/resource_attributes.py` & `permit-2.1.0rc1/permit/api/resource_attributes.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/resources.py` & `permit-2.1.0rc1/permit/api/resource_action_groups.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,192 +6,194 @@
     BasePermitApi,
     SimpleHttpClient,
     pagination_params,
     required_context,
     required_permissions,
 )
 from .context import ApiContextLevel, ApiKeyAccessLevel
-from .models import ResourceCreate, ResourceRead, ResourceReplace, ResourceUpdate
+from .models import (
+    ResourceActionGroupCreate,
+    ResourceActionGroupRead,
+    ResourceActionGroupUpdate,
+)
 
 
-class ResourcesApi(BasePermitApi):
+class ResourceActionGroupsApi(BasePermitApi):
     @property
-    def __resources(self) -> SimpleHttpClient:
+    def __action_groups(self) -> SimpleHttpClient:
         return self._build_http_client(
             "/v2/schema/{proj_id}/{env_id}/resources".format(
                 proj_id=self.config.api_context.project,
                 env_id=self.config.api_context.environment,
             )
         )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def list(self, page: int = 1, per_page: int = 100) -> List[ResourceRead]:
+    async def list(
+        self, resource_key: str, page: int = 1, per_page: int = 100
+    ) -> List[ResourceActionGroupRead]:
         """
-        Retrieves a list of resources.
+        Retrieves a list of action groups.
 
         Args:
+            resource_key: The key of the resource to filter on.
             page: The page number to fetch (default: 1).
             per_page: How many items to fetch per page (default: 100).
 
         Returns:
-            an array of resources.
+            an array of action groups.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__resources.get(
-            "",
-            model=List[ResourceRead],
+        return await self.__action_groups.get(
+            f"/{resource_key}/action_groups",
+            model=List[ResourceActionGroupRead],
             params=pagination_params(page, per_page),
         )
 
-    async def _get(self, resource_key: str) -> ResourceRead:
-        return await self.__resources.get(f"/{resource_key}", model=ResourceRead)
+    async def _get(self, resource_key: str, group_key: str) -> ResourceActionGroupRead:
+        return await self.__action_groups.get(
+            f"/{resource_key}/action_groups/{group_key}",
+            model=ResourceActionGroupRead,
+        )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def get(self, resource_key: str) -> ResourceRead:
+    async def get(self, resource_key: str, group_key: str) -> ResourceActionGroupRead:
         """
-        Retrieves a resource by its key.
+        Retrieves a action group by its key.
 
         Args:
-            resource_key: The key of the resource.
+            resource_key: The key of the resource the action group belongs to.
+            group_key: The key of the action group.
 
         Returns:
-            the resource.
+            the action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self._get(resource_key)
+        return await self._get(resource_key, group_key)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def get_by_key(self, resource_key: str) -> ResourceRead:
+    async def get_by_key(
+        self, resource_key: str, group_key: str
+    ) -> ResourceActionGroupRead:
         """
-        Retrieves a resource by its key.
+        Retrieves a action group by its key.
         Alias for the get method.
 
         Args:
-            resource_key: The key of the resource.
+            resource_key: The key of the resource the action group belongs to.
+            group_key: The key of the action group.
 
         Returns:
-            the resource.
+            the action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self._get(resource_key)
+        return await self._get(resource_key, group_key)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def get_by_id(self, resource_id: str) -> ResourceRead:
+    async def get_by_id(
+        self, resource_id: str, group_id: str
+    ) -> ResourceActionGroupRead:
         """
-        Retrieves a resource by its ID.
+        Retrieves a action group by its ID.
         Alias for the get method.
 
         Args:
-            resource_id: The ID of the resource.
+            resource_key: The ID of the resource the action group belongs to.
+            group_id: The ID of the action group.
 
         Returns:
-            the resource.
+            the action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self._get(resource_id)
+        return await self._get(resource_id, group_id)
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def create(self, resource_data: ResourceCreate) -> ResourceRead:
+    async def create(
+        self, resource_key: str, group_data: ResourceActionGroupCreate
+    ) -> ResourceActionGroupRead:
         """
-        Creates a new resource.
+        Creates a new action group.
 
         Args:
-            resource_data: The data for the new resource.
+            resource_key: The key of the resource under which the action group should be created.
+            group_data: The data for the new action group.
 
         Returns:
-            the created resource.
+            the created action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__resources.post("", model=ResourceRead, json=resource_data)
+        return await self.__action_groups.post(
+            f"/{resource_key}/action_groups",
+            model=ResourceActionGroupRead,
+            json=group_data,
+        )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def update(
-        self, resource_key: str, resource_data: ResourceUpdate
-    ) -> ResourceRead:
+        self, resource_key: str, group_key: str, group_data: ResourceActionGroupUpdate
+    ) -> ResourceActionGroupRead:
         """
-        Updates a resource.
+        Updates an action group.
 
         Args:
-            resource_key: The key of the resource.
-            resource_data: The updated data for the resource.
+            resource_key: The key of the resource the action group belongs to.
+            group_key: The key of the action group.
+            group_data: The updated data for the action group.
 
         Returns:
-            the updated resource.
+            the updated action group.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__resources.patch(
-            f"/{resource_key}",
-            model=ResourceRead,
-            json=resource_data,
+        return await self.__action_groups.patch(
+            f"/{resource_key}/action_groups/{group_key}",
+            model=ResourceActionGroupRead,
+            json=group_data,
         )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
-    async def replace(
-        self, resource_key: str, resource_data: ResourceReplace
-    ) -> ResourceRead:
+    async def delete(self, resource_key: str, group_key: str) -> None:
         """
-        Creates a resource if no such resource exists, otherwise completely replaces the resource in place.
+        Deletes a action group.
 
         Args:
-            resource_key: The key of the resource.
-            resource_data: The updated data for the resource.
-
-        Returns:
-            the updated resource.
+            resource_key: The key of the resource the action group belongs to.
+            group_key: The key of the action group to delete.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
-        return await self.__resources.put(
-            f"/{resource_key}",
-            model=ResourceRead,
-            json=resource_data,
+        return await self.__action_groups.delete(
+            f"/{resource_key}/action_groups/{group_key}"
         )
-
-    @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
-    @required_context(ApiContextLevel.ENVIRONMENT)
-    @validate_arguments
-    async def delete(self, resource_key: str) -> None:
-        """
-        Deletes a resource.
-
-        Args:
-            resource_key: The key of the resource to delete.
-
-        Raises:
-            PermitApiError: If the API returns an error HTTP status code.
-            PermitContextError: If the configured ApiContext does not match the required endpoint context.
-        """
-        return await self.__resources.delete(f"/{resource_key}")
```

### Comparing `permit-2.0.5/permit/api/role_assignments.py` & `permit-2.1.0rc1/permit/api/role_assignments.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,43 +32,47 @@
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
     @required_context(ApiContextLevel.ENVIRONMENT)
     @validate_arguments
     async def list(
         self,
         user_key: Optional[str] = None,
-        tenant_key: Optional[str] = None,
         role_key: Optional[str] = None,
+        tenant_key: Optional[str] = None,
+        resource_instance_key: Optional[str] = None,
         page: int = 1,
         per_page: int = 100,
     ) -> List[RoleAssignmentRead]:
         """
         Retrieves a list of role assignments based on the specified filters.
 
         Args:
             user_key: if specified, only role granted to this user will be fetched.
-            tenant_key: if specified, only role granted within this tenant will be fetched.
             role_key: if specified, only assignments of this role will be fetched.
+            tenant_key: (for roles) if specified, only role granted within this tenant will be fetched.
+            resource_instance_key: (for resource roles) if specified, only roles granted with this instance as the object will be fetched.
             page: The page number to fetch (default: 1).
             per_page: How many items to fetch per page (default: 100).
 
         Returns:
             an array of role assignments.
 
         Raises:
             PermitApiError: If the API returns an error HTTP status code.
             PermitContextError: If the configured ApiContext does not match the required endpoint context.
         """
         params = pagination_params(page, per_page)
         if user_key is not None:
             params.update(dict(user=user_key))
-        if tenant_key is not None:
-            params.update(dict(tenant=tenant_key))
         if role_key is not None:
             params.update(dict(role=role_key))
+        if tenant_key is not None:
+            params.update(dict(tenant=tenant_key))
+        if resource_instance_key is not None:
+            params.update(dict(resource_instance=resource_instance_key))
         return await self.__role_assignments.get(
             "",
             model=List[RoleAssignmentRead],
             params=params,
         )
 
     @required_permissions(ApiKeyAccessLevel.ENVIRONMENT_LEVEL_API_KEY)
```

### Comparing `permit-2.0.5/permit/api/roles.py` & `permit-2.1.0rc1/permit/api/roles.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/sync_api_client.py` & `permit-2.1.0rc1/permit/api/sync_api_client.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/tenants.py` & `permit-2.1.0rc1/permit/api/tenants.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/api/users.py` & `permit-2.1.0rc1/permit/api/users.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/config.py` & `permit-2.1.0rc1/permit/config.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/enforcement/enforcer.py` & `permit-2.1.0rc1/permit/enforcement/enforcer.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/enforcement/interfaces.py` & `permit-2.1.0rc1/permit/enforcement/interfaces.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     roles: Optional[List[AssignedRole]]
     attributes: Optional[Dict]
 
 
 class ResourceInput(BaseModel):
     type: str  # namespace/type of resources/objects
     id: Optional[str]  # id of individual object
+    key: Optional[str]  # key of individual object
     tenant: Optional[str]  # tenant the resource belongs to
     attributes: Optional[Dict]  # extra resources attributes
     context: Optional[Dict]  # extra context
 
 
 class OpaResult(BaseModel):
     allow: bool
```

### Comparing `permit-2.0.5/permit/exceptions.py` & `permit-2.1.0rc1/permit/exceptions.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/permit.py` & `permit-2.1.0rc1/permit/permit.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/sync.py` & `permit-2.1.0rc1/permit/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/utils/context.py` & `permit-2.1.0rc1/permit/utils/context.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/utils/deprecation.py` & `permit-2.1.0rc1/permit/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit/utils/sync.py` & `permit-2.1.0rc1/permit/utils/sync.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/permit.egg-info/SOURCES.txt` & `permit-2.1.0rc1/permit.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -21,17 +21,21 @@
 permit/api/condition_sets.py
 permit/api/context.py
 permit/api/deprecated.py
 permit/api/elements.py
 permit/api/environments.py
 permit/api/models.py
 permit/api/projects.py
+permit/api/relationship_tuples.py
 permit/api/resource_action_groups.py
 permit/api/resource_actions.py
 permit/api/resource_attributes.py
+permit/api/resource_instances.py
+permit/api/resource_relations.py
+permit/api/resource_roles.py
 permit/api/resources.py
 permit/api/role_assignments.py
 permit/api/roles.py
 permit/api/sync_api_client.py
 permit/api/tenants.py
 permit/api/users.py
 permit/enforcement/__init__.py
@@ -43,8 +47,9 @@
 permit/utils/dicts.py
 permit/utils/sync.py
 tests/__init__.py
 tests/conftest.py
 tests/test_abac_e2e.py
 tests/test_rbac_e2e.py
 tests/test_rbac_e2e_sync.py
+tests/test_rebac_e2e.py
 tests/utils.py
```

### Comparing `permit-2.0.5/setup.py` & `permit-2.1.0rc1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
 
 setup(
     name="permit",
-    version="2.0.5",
+    version="2.1.0rc1",
     packages=find_packages(),
     author="Asaf Cohen",
     author_email="asaf@permit.io",
     license="Apache 2.0",
     python_requires=">=3.8",
     description="Permit.io python sdk",
     install_requires=get_requirements(),
```

### Comparing `permit-2.0.5/tests/conftest.py` & `permit-2.1.0rc1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/tests/test_abac_e2e.py` & `permit-2.1.0rc1/tests/test_abac_e2e.py`

 * *Files identical despite different names*

### Comparing `permit-2.0.5/tests/test_rbac_e2e.py` & `permit-2.1.0rc1/tests/test_rbac_e2e.py`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
                 "tenant": "tesla",
             }
         )
 
         assert ra.user_id == user.id
         assert ra.role_id == viewer.id
         assert ra.tenant_id == tenant.id
-        assert ra.user == user.email
+        assert ra.user == user.email or ra.user == user.key
         assert ra.role == viewer.key
         assert ra.tenant == tenant.key
 
         logger.info(
             "sleeping 2 seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(2)
```

### Comparing `permit-2.0.5/tests/test_rbac_e2e_sync.py` & `permit-2.1.0rc1/tests/test_rbac_e2e_sync.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
                 "tenant": "tesla",
             }
         )
 
         assert ra.user_id == user.id
         assert ra.role_id == viewer.id
         assert ra.tenant_id == tenant.id
-        assert ra.user == user.email
+        assert ra.user == user.email or ra.user == user.key
         assert ra.role == viewer.key
         assert ra.tenant == tenant.key
 
         logger.info(
             "sleeping 2 seconds before permit.check() to make sure all writes propagated from cloud to PDP"
         )
         time.sleep(2)
```

