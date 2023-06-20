# Comparing `tmp/django_anon_lockout-2.0.0.tar.gz` & `tmp/django_anon_lockout-2.1.0.tar.gz`

## Comparing `django_anon_lockout-2.0.0.tar` & `django_anon_lockout-2.1.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/__init__.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/admin.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/apps.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/conf.py
--rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/handlers.py
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/models.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/utils.py
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/migrations/0001_initial.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/migrations/0002_accesssession_successes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/anon_lockout/migrations/__init__.py
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/.gitignore
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/LICENSE
--rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/README.md
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 django_anon_lockout-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/__init__.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/admin.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/apps.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/conf.py
+-rw-r--r--   0        0        0     2596 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/handlers.py
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/models.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/management/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/management/commands/delete_lockout_data.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/management/commands/invalidate_lockouts.py
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/migrations/0001_initial.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/migrations/0002_accesssession_successes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/anon_lockout/migrations/__init__.py
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/LICENSE
+-rw-r--r--   0        0        0     3711 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/README.md
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4266 2020-02-02 00:00:00.000000 django_anon_lockout-2.1.0/PKG-INFO
```

### Comparing `django_anon_lockout-2.0.0/anon_lockout/handlers.py` & `django_anon_lockout-2.1.0/anon_lockout/handlers.py`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-2.0.0/anon_lockout/models.py` & `django_anon_lockout-2.1.0/anon_lockout/models.py`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-2.0.0/anon_lockout/migrations/0001_initial.py` & `django_anon_lockout-2.1.0/anon_lockout/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-2.0.0/.gitignore` & `django_anon_lockout-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-2.0.0/LICENSE` & `django_anon_lockout-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-2.0.0/README.md` & `django_anon_lockout-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_anon_lockout-2.0.0/pyproject.toml` & `django_anon_lockout-2.1.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/anon_lockout"
 ]
 
 [project]
 name = "django-anon-lockout"
-version = "2.0.0"
+version = "2.1.0"
 authors = [
   { name="Erlend Paulsen Skaaden", email="erlendskaaden@gmail.com" },
 ]
 description = "Django module for anonymous lockout"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `django_anon_lockout-2.0.0/PKG-INFO` & `django_anon_lockout-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-anon-lockout
-Version: 2.0.0
+Version: 2.1.0
 Summary: Django module for anonymous lockout
 Project-URL: Homepage, https://github.com/erlendps/django-anon-lockout
 Project-URL: Bug Tracker, https://github.com/erlendps/django-anon-lockout/issues
 Author-email: Erlend Paulsen Skaaden <erlendskaaden@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

