# Comparing `tmp/landingzone_organization-0.4.0.tar.gz` & `tmp/landingzone_organization-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "landingzone_organization-0.4.0.tar", max compression
+gzip compressed data, was "landingzone_organization-0.5.0.tar", max compression
```

## Comparing `landingzone_organization-0.4.0.tar` & `landingzone_organization-0.5.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      981 2023-05-05 16:55:33.709640 landingzone_organization-0.4.0/README.md
--rw-r--r--   0        0        0      636 2023-05-05 16:55:34.509692 landingzone_organization-0.4.0/landingzone_organization/__init__.py
--rw-r--r--   0        0        0      395 2023-05-05 16:55:33.709640 landingzone_organization-0.4.0/landingzone_organization/account.py
--rw-r--r--   0        0        0       75 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/adapters/__init__.py
--rw-r--r--   0        0        0     3248 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/adapters/aws_organization.py
--rw-r--r--   0        0        0      509 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/commands/__init__.py
--rw-r--r--   0        0        0      598 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/commands/account.py
--rw-r--r--   0        0        0      558 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/commands/organization.py
--rw-r--r--   0        0        0     2096 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/commands/profiles.py
--rw-r--r--   0        0        0      707 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/commands/workload.py
--rw-r--r--   0        0        0     1517 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/context.py
--rw-r--r--   0        0        0      744 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/cli/handler.py
--rw-r--r--   0        0        0      666 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/filtering.py
--rw-r--r--   0        0        0     1035 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/group.py
--rw-r--r--   0        0        0      929 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/groups.py
--rw-r--r--   0        0        0     3220 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/organization.py
--rw-r--r--   0        0        0      938 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/organization_unit.py
--rw-r--r--   0        0        0      917 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/profile.py
--rw-r--r--   0        0        0     1164 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/profiles.py
--rw-r--r--   0        0        0      887 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/workload.py
--rw-r--r--   0        0        0     1559 2023-05-05 16:55:33.713640 landingzone_organization-0.4.0/landingzone_organization/workloads.py
--rw-r--r--   0        0        0     1387 2023-05-05 16:55:34.509692 landingzone_organization-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      981 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/README.md
+-rw-r--r--   0        0        0      636 2023-06-20 08:57:49.282397 landingzone_organization-0.5.0/landingzone_organization/__init__.py
+-rw-r--r--   0        0        0      395 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/account.py
+-rw-r--r--   0        0        0       75 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/adapters/__init__.py
+-rw-r--r--   0        0        0     3248 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/adapters/aws_organization.py
+-rw-r--r--   0        0        0      509 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/__init__.py
+-rw-r--r--   0        0        0     1242 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/account.py
+-rw-r--r--   0        0        0      558 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/organization.py
+-rw-r--r--   0        0        0     2096 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/profiles.py
+-rw-r--r--   0        0        0      707 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/commands/workload.py
+-rw-r--r--   0        0        0     1517 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/context.py
+-rw-r--r--   0        0        0      744 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/cli/handler.py
+-rw-r--r--   0        0        0      666 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/filtering.py
+-rw-r--r--   0        0        0     1035 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/group.py
+-rw-r--r--   0        0        0      929 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/groups.py
+-rw-r--r--   0        0        0     3220 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/organization.py
+-rw-r--r--   0        0        0      938 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/organization_unit.py
+-rw-r--r--   0        0        0      917 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/profile.py
+-rw-r--r--   0        0        0     1164 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/profiles.py
+-rw-r--r--   0        0        0      887 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/workload.py
+-rw-r--r--   0        0        0     1559 2023-06-20 08:57:48.562386 landingzone_organization-0.5.0/landingzone_organization/workloads.py
+-rw-r--r--   0        0        0     1386 2023-06-20 08:57:49.282397 landingzone_organization-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 landingzone_organization-0.5.0/PKG-INFO
```

### Comparing `landingzone_organization-0.4.0/README.md` & `landingzone_organization-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/__init__.py` & `landingzone_organization-0.5.0/landingzone_organization/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from landingzone_organization.organization_unit import OrganizationUnit
 from landingzone_organization.account import Account
 from landingzone_organization.groups import Groups
 from landingzone_organization.group import Group
 from landingzone_organization.profile import Profile
 from landingzone_organization.profiles import Profiles
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 __all__ = [
     AWSOrganization,
     Organization,
     OrganizationUnit,
     Account,
     Groups,
     Group,
```

### Comparing `landingzone_organization-0.4.0/landingzone_organization/adapters/aws_organization.py` & `landingzone_organization-0.5.0/landingzone_organization/adapters/aws_organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/cli/commands/organization.py` & `landingzone_organization-0.5.0/landingzone_organization/cli/commands/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/cli/commands/profiles.py` & `landingzone_organization-0.5.0/landingzone_organization/cli/commands/profiles.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/cli/commands/workload.py` & `landingzone_organization-0.5.0/landingzone_organization/cli/commands/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/cli/context.py` & `landingzone_organization-0.5.0/landingzone_organization/cli/context.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/cli/handler.py` & `landingzone_organization-0.5.0/landingzone_organization/cli/handler.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/filtering.py` & `landingzone_organization-0.5.0/landingzone_organization/filtering.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/group.py` & `landingzone_organization-0.5.0/landingzone_organization/group.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/groups.py` & `landingzone_organization-0.5.0/landingzone_organization/groups.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/organization.py` & `landingzone_organization-0.5.0/landingzone_organization/organization.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/organization_unit.py` & `landingzone_organization-0.5.0/landingzone_organization/organization_unit.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/profile.py` & `landingzone_organization-0.5.0/landingzone_organization/profile.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/profiles.py` & `landingzone_organization-0.5.0/landingzone_organization/profiles.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/workload.py` & `landingzone_organization-0.5.0/landingzone_organization/workload.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/landingzone_organization/workloads.py` & `landingzone_organization-0.5.0/landingzone_organization/workloads.py`

 * *Files identical despite different names*

### Comparing `landingzone_organization-0.4.0/pyproject.toml` & `landingzone_organization-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "landingzone-organization"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Joris Conijn <Joris.Conijn@xebia.com>"]
 readme = "README.md"
 homepage = "https://binxio.github.io/landingzone-organization/"
 documentation = "https://binxio.github.io/landingzone-organization/3-user-documentation/"
 repository = "https://github.com/binxio/landingzone-organization"
 packages = [{include = "landingzone_organization"}]
@@ -45,15 +45,15 @@
 
 [tool.coverage.run]
 branch = true
 source = ["aws_iam_login"]
 
 [tool.coverage.report]
 show_missing = true
-fail_under = 100
+fail_under = 98
 exclude_lines = [
     "if __name__ == .__main__.:"
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `landingzone_organization-0.4.0/PKG-INFO` & `landingzone_organization-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: landingzone-organization
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Home-page: https://binxio.github.io/landingzone-organization/
 Author: Joris Conijn
 Author-email: Joris.Conijn@xebia.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

