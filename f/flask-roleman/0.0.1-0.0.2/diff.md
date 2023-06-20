# Comparing `tmp/flask-roleman-0.0.1.tar.gz` & `tmp/flask-roleman-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-roleman-0.0.1.tar", last modified: Mon Jun 19 18:20:43 2023, max compression
+gzip compressed data, was "flask-roleman-0.0.2.tar", last modified: Tue Jun 20 21:21:18 2023, max compression
```

## Comparing `flask-roleman-0.0.1.tar` & `flask-roleman-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-19 18:20:43.025916 flask-roleman-0.0.1/
--rw-r--r--   0 human     (1000) human     (1000)      537 2023-06-19 18:20:43.022583 flask-roleman-0.0.1/PKG-INFO
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-19 18:20:43.022583 flask-roleman-0.0.1/flask_roleman/
--rw-r--r--   0 human     (1000) human     (1000)     5342 2023-06-17 19:43:54.000000 flask-roleman-0.0.1/flask_roleman/__init__.py
-drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-19 18:20:43.022583 flask-roleman-0.0.1/flask_roleman.egg-info/
--rw-r--r--   0 human     (1000) human     (1000)      537 2023-06-19 18:20:43.000000 flask-roleman-0.0.1/flask_roleman.egg-info/PKG-INFO
--rw-r--r--   0 human     (1000) human     (1000)      218 2023-06-19 18:20:43.000000 flask-roleman-0.0.1/flask_roleman.egg-info/SOURCES.txt
--rw-r--r--   0 human     (1000) human     (1000)        1 2023-06-19 18:20:43.000000 flask-roleman-0.0.1/flask_roleman.egg-info/dependency_links.txt
--rw-r--r--   0 human     (1000) human     (1000)       35 2023-06-19 18:20:43.000000 flask-roleman-0.0.1/flask_roleman.egg-info/requires.txt
--rw-r--r--   0 human     (1000) human     (1000)       14 2023-06-19 18:20:43.000000 flask-roleman-0.0.1/flask_roleman.egg-info/top_level.txt
--rw-r--r--   0 human     (1000) human     (1000)       38 2023-06-19 18:20:43.025916 flask-roleman-0.0.1/setup.cfg
--rw-r--r--   0 human     (1000) human     (1000)      857 2023-06-19 18:13:41.000000 flask-roleman-0.0.1/setup.py
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/
+-rw-r--r--   0 human     (1000) human     (1000)     4044 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/PKG-INFO
+-rw-r--r--   0 human     (1000) human     (1000)     3466 2023-06-20 21:10:19.000000 flask-roleman-0.0.2/README.md
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-20 21:21:18.607631 flask-roleman-0.0.2/flask_roleman/
+-rw-r--r--   0 human     (1000) human     (1000)     4978 2023-06-20 21:11:34.000000 flask-roleman-0.0.2/flask_roleman/__init__.py
+drwxr-xr-x   0 human     (1000) human     (1000)        0 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/flask_roleman.egg-info/
+-rw-r--r--   0 human     (1000) human     (1000)     4044 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/PKG-INFO
+-rw-r--r--   0 human     (1000) human     (1000)      228 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/SOURCES.txt
+-rw-r--r--   0 human     (1000) human     (1000)        1 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/dependency_links.txt
+-rw-r--r--   0 human     (1000) human     (1000)       35 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/requires.txt
+-rw-r--r--   0 human     (1000) human     (1000)       14 2023-06-20 21:21:18.000000 flask-roleman-0.0.2/flask_roleman.egg-info/top_level.txt
+-rw-r--r--   0 human     (1000) human     (1000)       38 2023-06-20 21:21:18.610964 flask-roleman-0.0.2/setup.cfg
+-rw-r--r--   0 human     (1000) human     (1000)     1032 2023-06-20 21:20:51.000000 flask-roleman-0.0.2/setup.py
```

### Comparing `flask-roleman-0.0.1/flask_roleman/__init__.py` & `flask-roleman-0.0.2/flask_roleman/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-# t.me/elhasnaouymed
 from flask import abort
 from flask_login import current_user
-from flask_sqlalchemy import SQLAlchemy as _SQLAlchemy
+from flask_sqlalchemy import SQLAlchemy as _SQLAlchemy, model as _model
+
+
+_Role: _model.Model | None = None  # holds the Role Model class to be accessed from ManMixing
 
 
 class RoleMan:
     SECONDARY_TABLE_NAME = 'user_role'  # name of the secondary relationship table on the database
     ROLE_TABLE_NAME = 'role'  # name of the table that will hold the roles
 
     def __init__(self, db: _SQLAlchemy = None, user_table_name: str = 'user', user_table_class_name: str = 'User'):
@@ -18,16 +20,14 @@
         self._initialized = False  # used within the object (private and protected)
         # > set the default values
         self._db = None
         self._user_table_name = user_table_name
         self._user_table_class_name = user_table_class_name
         self.UserRole = None
         self.Role = None
-        self.RoelManMixing = None
-        self._init_role_man_mixing()
 
         # check whether to initialize now or not
         if db and (isinstance(db, _SQLAlchemy) or issubclass(type(db), _SQLAlchemy)):
             self.init_database(db, user_table_name, user_table_class_name)
 
     def init_database(self, db: _SQLAlchemy, user_table_name: str = None, user_table_class_name: str = None):
         """
@@ -70,51 +70,45 @@
             def __init__(self, name: str):
                 self.name = name.lower()
 
             def __repr__(self):
                 return f'<Role "{self.name}">'
 
         self.Role = Role
+        global _Role
+        _Role = Role
 
-    def _init_role_man_mixing(self):
-        """
-        This method will create the Mixing class for User table to inherit from
-        :return: None
-        """
-        master = self
 
-        class RoleManMixing:
-            roles = None  # just to not get the AttributeError from User, when accessing the relationship, before initializing this class
+class RoleManMixing:
+    roles = None  # just to not get the AttributeError from User, when accessing the relationship, before initializing this class
 
-            def has_role(self, role):
-                if isinstance(role, str):
-                    role = master.Role.query.filter_by(name=role.lower()).first()
-                #
-                if not role:
+    def has_role(self, role):
+        if isinstance(role, str):
+            role = _Role.query.filter_by(name=role.lower()).first()
+        #
+        if not role:
+            return False
+        #
+        return self in role.users
+
+    def has_roles(self, *roles_seq):
+        def _has_one_role(*_rls):
+            # checks if the user has at least one role of many (OR Gate)
+            for rl in _rls:
+                if self.has_role(rl):
+                    return True
+            return False
+
+        for role_value in roles_seq:
+            if isinstance(role_value, (list, tuple, set)):
+                if not _has_one_role(*role_value):
                     return False
-                #
-                return self in role.users
-
-            def has_roles(self, *roles_seq):
-                def _has_one_role(*_rls):
-                    # checks if the user has at least one role of many (OR Gate)
-                    for rl in _rls:
-                        if self.has_role(rl):
-                            return True
-                    return False
-
-                for role_value in roles_seq:
-                    if isinstance(role_value, (list, tuple, set)):
-                        if not _has_one_role(*role_value):
-                            return False
-                    elif not self.has_role(role_value):
-                        return False
-                return True
-
-        self.RoelManMixing = RoleManMixing
+            elif not self.has_role(role_value):
+                return False
+        return True
 
 
 def roles_required(*roles):
     """
     This decorator is used before routes, to ensure that the current_user has the authorization to access that route
     :param role: role as str or Role object
     :return: None
```

