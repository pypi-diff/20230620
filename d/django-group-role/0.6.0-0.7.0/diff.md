# Comparing `tmp/django-group-role-0.6.0.tar.gz` & `tmp/django-group-role-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-group-role-0.6.0.tar", last modified: Thu Apr 13 07:52:14 2023, max compression
+gzip compressed data, was "django-group-role-0.7.0.tar", last modified: Tue Jun 20 08:21:21 2023, max compression
```

## Comparing `django-group-role-0.6.0.tar` & `django-group-role-0.7.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.640677 django-group-role-0.6.0/
--rw-rw-r--   0 davide    (1000) davide    (1000)    11357 2021-11-22 11:09:44.000000 django-group-role-0.6.0/LICENSE
--rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-04-13 07:52:14.640677 django-group-role-0.6.0/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)     3888 2022-08-24 08:14:24.000000 django-group-role-0.6.0/README.md
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.632677 django-group-role-0.6.0/django_group_role/
--rw-rw-r--   0 davide    (1000) davide    (1000)      729 2023-04-13 07:36:23.000000 django-group-role-0.6.0/django_group_role/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      164 2023-04-12 15:35:54.000000 django-group-role-0.6.0/django_group_role/apps.py
--rw-rw-r--   0 davide    (1000) davide    (1000)      151 2021-11-26 11:53:38.000000 django-group-role-0.6.0/django_group_role/exceptions.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.636677 django-group-role-0.6.0/django_group_role/management/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:23.000000 django-group-role-0.6.0/django_group_role/management/__init__.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.636677 django-group-role-0.6.0/django_group_role/management/commands/
--rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:32.000000 django-group-role-0.6.0/django_group_role/management/commands/__init__.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2381 2023-04-13 07:24:41.000000 django-group-role-0.6.0/django_group_role/management/commands/populate_roles.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     6621 2023-04-13 07:27:32.000000 django-group-role-0.6.0/django_group_role/roles.py
--rw-rw-r--   0 davide    (1000) davide    (1000)       89 2022-08-24 08:05:10.000000 django-group-role-0.6.0/django_group_role/signals.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1210 2023-04-12 15:41:34.000000 django-group-role-0.6.0/django_group_role/test.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1693 2023-04-13 06:58:22.000000 django-group-role-0.6.0/django_group_role/utils.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.636677 django-group-role-0.6.0/django_group_role.egg-info/
--rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/PKG-INFO
--rw-rw-r--   0 davide    (1000) davide    (1000)      731 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/SOURCES.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/dependency_links.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       35 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/requires.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)       18 2023-04-13 07:52:14.000000 django-group-role-0.6.0/django_group_role.egg-info/top_level.txt
--rw-rw-r--   0 davide    (1000) davide    (1000)     1742 2023-04-13 07:52:14.640677 django-group-role-0.6.0/setup.cfg
--rw-rw-r--   0 davide    (1000) davide    (1000)       60 2023-04-12 15:21:16.000000 django-group-role-0.6.0/setup.py
-drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-04-13 07:52:14.640677 django-group-role-0.6.0/tests/
--rw-rw-r--   0 davide    (1000) davide    (1000)     9417 2023-04-13 07:08:45.000000 django-group-role-0.6.0/tests/test_command.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1358 2023-04-13 07:09:32.000000 django-group-role-0.6.0/tests/test_configuration.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     1794 2023-04-04 15:25:30.000000 django-group-role-0.6.0/tests/test_database.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2881 2023-04-13 07:04:33.000000 django-group-role-0.6.0/tests/test_definitions.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     2996 2023-04-12 15:43:16.000000 django-group-role-0.6.0/tests/test_testing_utils.py
--rw-rw-r--   0 davide    (1000) davide    (1000)     4203 2023-04-13 07:04:18.000000 django-group-role-0.6.0/tests/test_utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-20 08:21:21.314589 django-group-role-0.7.0/
+-rw-rw-r--   0 davide    (1000) davide    (1000)    11357 2021-11-22 11:09:44.000000 django-group-role-0.7.0/LICENSE
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-06-20 08:21:21.314589 django-group-role-0.7.0/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)     3888 2022-08-24 08:14:24.000000 django-group-role-0.7.0/README.md
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-20 08:21:21.310589 django-group-role-0.7.0/django_group_role/
+-rw-rw-r--   0 davide    (1000) davide    (1000)      729 2023-06-20 08:14:46.000000 django-group-role-0.7.0/django_group_role/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      164 2023-04-12 15:35:54.000000 django-group-role-0.7.0/django_group_role/apps.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)      151 2021-11-26 11:53:38.000000 django-group-role-0.7.0/django_group_role/exceptions.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-20 08:21:21.314589 django-group-role-0.7.0/django_group_role/management/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:23.000000 django-group-role-0.7.0/django_group_role/management/__init__.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-20 08:21:21.314589 django-group-role-0.7.0/django_group_role/management/commands/
+-rw-rw-r--   0 davide    (1000) davide    (1000)        0 2021-11-19 14:59:32.000000 django-group-role-0.7.0/django_group_role/management/commands/__init__.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2381 2023-04-13 07:24:41.000000 django-group-role-0.7.0/django_group_role/management/commands/populate_roles.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     5551 2023-06-20 08:05:46.000000 django-group-role-0.7.0/django_group_role/roles.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)       89 2022-08-24 08:05:10.000000 django-group-role-0.7.0/django_group_role/signals.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1210 2023-04-12 15:41:34.000000 django-group-role-0.7.0/django_group_role/test.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2460 2023-06-20 08:05:46.000000 django-group-role-0.7.0/django_group_role/utils.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-20 08:21:21.314589 django-group-role-0.7.0/django_group_role.egg-info/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4909 2023-06-20 08:21:21.000000 django-group-role-0.7.0/django_group_role.egg-info/PKG-INFO
+-rw-rw-r--   0 davide    (1000) davide    (1000)      731 2023-06-20 08:21:21.000000 django-group-role-0.7.0/django_group_role.egg-info/SOURCES.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)        1 2023-06-20 08:21:21.000000 django-group-role-0.7.0/django_group_role.egg-info/dependency_links.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       12 2023-06-20 08:21:21.000000 django-group-role-0.7.0/django_group_role.egg-info/requires.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)       18 2023-06-20 08:21:21.000000 django-group-role-0.7.0/django_group_role.egg-info/top_level.txt
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1741 2023-06-20 08:21:21.314589 django-group-role-0.7.0/setup.cfg
+-rw-rw-r--   0 davide    (1000) davide    (1000)       60 2023-04-12 15:21:16.000000 django-group-role-0.7.0/setup.py
+drwxrwxr-x   0 davide    (1000) davide    (1000)        0 2023-06-20 08:21:21.314589 django-group-role-0.7.0/tests/
+-rw-rw-r--   0 davide    (1000) davide    (1000)     9421 2023-06-20 08:05:46.000000 django-group-role-0.7.0/tests/test_command.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1358 2023-04-13 07:09:32.000000 django-group-role-0.7.0/tests/test_configuration.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     1794 2023-06-19 09:26:50.000000 django-group-role-0.7.0/tests/test_database.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2881 2023-06-19 09:26:50.000000 django-group-role-0.7.0/tests/test_definitions.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     2996 2023-06-19 09:26:50.000000 django-group-role-0.7.0/tests/test_testing_utils.py
+-rw-rw-r--   0 davide    (1000) davide    (1000)     4203 2023-04-13 07:04:18.000000 django-group-role-0.7.0/tests/test_utils.py
```

### Comparing `django-group-role-0.6.0/LICENSE` & `django-group-role-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/PKG-INFO` & `django-group-role-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-group-role
-Version: 0.6.0
+Version: 0.7.0
 Summary: Django Group-based roles
 Home-page: https://github.com/certego/django-group-role
 Author: Davide Setti
 Project-URL: Bug Tracker, https://github.com/certego/django-group-role/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-group-role-0.6.0/README.md` & `django-group-role-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/django_group_role/__init__.py` & `django-group-role-0.7.0/django_group_role/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
         # the role is not registered thus we assume the user
         # cannot have that role
         return False
 
     return user.groups.filter(name=role.name).exists()
 
 
-__version__ = (0, 6, 0)
+__version__ = (0, 7, 0)
```

### Comparing `django-group-role-0.6.0/django_group_role/management/commands/populate_roles.py` & `django-group-role-0.7.0/django_group_role/management/commands/populate_roles.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/django_group_role/roles.py` & `django-group-role-0.7.0/django_group_role/roles.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-from functools import reduce, partialmethod
 import inspect
+from contextlib import nullcontext, suppress
+from functools import partialmethod, reduce
 from importlib import import_module
-from django.core.exceptions import ImproperlyConfigured, MultipleObjectsReturned
+
+from django.core.exceptions import ImproperlyConfigured
 from django.utils.functional import cached_property
+
 from .exceptions import BadRoleException
 from .signals import post_role_setup, pre_role_setup
-from .utils import map_permissions
+from .utils import get_permission, map_permissions
 
 
 class _RoleRegistry(dict):
     def __delitem__(self, v):
         raise NotImplementedError
 
     def __setitem__(self, k, v):
@@ -65,60 +68,35 @@
     @cached_property
     def group(self):
         from django.contrib.auth.models import Group
 
         group, _created = Group.objects.get_or_create(name=self.name)
         return group
 
+    @classmethod
+    def iter_perms(cls, catch=False):
+        context = suppress(BadRoleException) if catch else nullcontext()
+        for app_label, app_perms in cls._permissions.items():
+            for modelname, perms in app_perms.items():
+                for perm in sorted(perms):
+                    with context:
+                        yield get_permission(perm, app_label, modelname)
+
     def setup_permissions(self, clear=False):
         """Assignes declared permissions to this role group.
 
         Args:
             clear (bool, optional): If passed as True also clears existing
                 permissions bound to this role. Defaults to False.
         """
-        from django.contrib.auth.models import Permission
-        from guardian.shortcuts import assign_perm
-
         pre_role_setup.send(self.__class__, role=self, clear=clear)
         if clear:
-            self.group.permissions.clear()
-
-        for app_label, app_perms in self._permissions.items():
-            for modelname, perms in app_perms.items():
-                if modelname == "_codenames":
-                    # handle codenames permissions
-                    for perm in perms:
-                        perm = f"{app_label}.{perm}"
-                        try:
-                            assign_perm(perm, self.group)
-                        except (
-                            ValueError,
-                            Permission.DoesNotExist,
-                            MultipleObjectsReturned,
-                        ):
-                            raise BadRoleException(
-                                f"Permission {perm} cannot be bound to role",
-                                perm,
-                            )
-                else:
-                    # model-grouped perms
-                    for perm in perms:
-                        try:
-                            perm = Permission.objects.get_by_natural_key(
-                                perm, app_label, modelname
-                            )
-                        except (ValueError, Permission.DoesNotExist):
-                            raise BadRoleException(
-                                f"Permission {perm} ({app_label}) cannot be bound to role",
-                                f"{app_label}.{perm}",
-                            )
-                        else:
-                            assign_perm(perm, self.group)
-
+            self.group.permissions.set(self.iter_perms())
+        else:
+            self.group.permissions.add(*self.iter_perms())
         post_role_setup.send(self.__class__, role=self)
 
     # wrappers for group methods
     def _wrap_group_method(self, method, *args, **kwargs):
         method = getattr(self.group.user_set, method)
         return method(*args, **kwargs)
```

### Comparing `django-group-role-0.6.0/django_group_role/test.py` & `django-group-role-0.7.0/django_group_role/test.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/django_group_role/utils.py` & `django-group-role-0.7.0/django_group_role/utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from collections import defaultdict
 from functools import reduce
 
+from django.core.exceptions import MultipleObjectsReturned
+
+from .exceptions import BadRoleException
+
 
 def _map_permissions(perm_map, permissions):
     if not permissions:
         return perm_map
 
     assert isinstance(
         permissions, (list, tuple, set, dict)
@@ -40,7 +44,28 @@
     return perm_map
 
 
 def map_permissions(*permissions_list):
     perm_map = defaultdict(lambda: defaultdict(set))
     # turn back defaultdicto into dict to avoid false matches
     return dict(reduce(_map_permissions, permissions_list, perm_map))
+
+
+def get_permission(codename: str, app_label: str, model: str):
+    from django.contrib.auth.models import Permission
+
+    try:
+        if model == "_codenames":
+            return Permission.objects.get(
+                codename=codename, content_type__app_label=app_label
+            )
+        else:
+            return Permission.objects.get_by_natural_key(codename, app_label, model)
+    except (
+        ValueError,
+        Permission.DoesNotExist,
+        MultipleObjectsReturned,
+    ) as ex:
+        raise BadRoleException(
+            f"Permission {codename} ({app_label}) cannot be bound to role",
+            f"{app_label}.{codename}",
+        ) from ex
```

### Comparing `django-group-role-0.6.0/django_group_role.egg-info/PKG-INFO` & `django-group-role-0.7.0/django_group_role.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-group-role
-Version: 0.6.0
+Version: 0.7.0
 Summary: Django Group-based roles
 Home-page: https://github.com/certego/django-group-role
 Author: Davide Setti
 Project-URL: Bug Tracker, https://github.com/certego/django-group-role/issues
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `django-group-role-0.6.0/django_group_role.egg-info/SOURCES.txt` & `django-group-role-0.7.0/django_group_role.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/setup.cfg` & `django-group-role-0.7.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-group-role
-version = 0.6.0
+version = 0.7.0
 author = Davide Setti
 description = Django Group-based roles
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/certego/django-group-role
 project_urls = 
 	Bug Tracker = https://github.com/certego/django-group-role/issues
@@ -24,23 +24,21 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Intended Audience :: Developers
 
 [options]
 packages = find:
 python_requires = >=3.7
-setup_requires = 
-	pytest-runner
 install_requires = 
 	Django>=3.2
-	django-guardian~=2.4.0
 tests_require = 
 	pytest
 	pytest-django
 	pytest-cov
+	django-guardian~=2.4.0
 
 [options.packages.find]
 exclude = tests
 
 [aliases]
 test = pytest
 
@@ -61,15 +59,17 @@
 envlist = 
 	py{37,38,39,310}-django32
 	py{38,39,310,311}-django{40,41,42}
 	py{310,311}-djangomaster
 
 [testenv]
 usedevelop = true
-commands = python setup.py test
+extras = tests
+whitelist_externals = py.test
+commands = py.test
 deps = 
 	django32: Django>=3.2,<3.3
 	django32: Django>=3.2,<3.3
 	django40: Django>=4.0,<4.1
 	django41: Django>=4.1,<4.2
 	django42: Django>=4.2,<4.3
 	djangomaster: https://github.com/django/django/archive/main.tar.gz
```

### Comparing `django-group-role-0.6.0/tests/test_command.py` & `django-group-role-0.7.0/tests/test_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                 'Setting permissions for role "Group Managers"...',
                 'Role "Group Managers" setup completed!',
                 'Setting permissions for role "Top-Managers"...',
                 'Role "Top-Managers" setup completed!',
                 'Setting permissions for role "Erasers"...',
                 'Unable to bound permission to "Erasers" (Permission broken (auth) cannot be bound to role)',
                 'Setting permissions for role "Broken"...',
-                'Unable to bound permission to "Broken" (Permission auth.non_existing_perm cannot be bound to role)',
+                'Unable to bound permission to "Broken" (Permission non_existing_perm (auth) cannot be bound to role)',
                 "",
             ],
         )
         self.assertEqual(Group.objects.all().count(), 7)
         group = Group.objects.get_by_natural_key("Users")
         self.assertQuerysetEqual(
             group.permissions.all(),
@@ -108,15 +108,15 @@
                 'Setting permissions for role "Group Managers"...',
                 'Role "Group Managers" setup completed!',
                 'Setting permissions for role "Top-Managers"...',
                 'Role "Top-Managers" setup completed!',
                 'Setting permissions for role "Erasers"...',
                 'Unable to bound permission to "Erasers" (Permission broken (auth) cannot be bound to role)',
                 'Setting permissions for role "Broken"...',
-                'Unable to bound permission to "Broken" (Permission auth.non_existing_perm cannot be bound to role)',
+                'Unable to bound permission to "Broken" (Permission non_existing_perm (auth) cannot be bound to role)',
                 "",
             ],
         )
         self.assertEqual(Group.objects.all().count(), 7)
         group = Group.objects.get_by_natural_key("Users")
         self.assertQuerysetEqual(
             group.permissions.all(),
```

### Comparing `django-group-role-0.6.0/tests/test_configuration.py` & `django-group-role-0.7.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/tests/test_database.py` & `django-group-role-0.7.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/tests/test_definitions.py` & `django-group-role-0.7.0/tests/test_definitions.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/tests/test_testing_utils.py` & `django-group-role-0.7.0/tests/test_testing_utils.py`

 * *Files identical despite different names*

### Comparing `django-group-role-0.6.0/tests/test_utils.py` & `django-group-role-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

