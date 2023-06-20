# Comparing `tmp/django-anorganization-0.1.0rc1.tar.gz` & `tmp/django-anorganization-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-anorganization-0.1.0rc1.tar", last modified: Mon Feb 20 04:11:28 2023, max compression
+gzip compressed data, was "django-anorganization-0.1.0rc3.tar", last modified: Tue Jun 20 03:34:05 2023, max compression
```

## Comparing `django-anorganization-0.1.0rc1.tar` & `django-anorganization-0.1.0rc3.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-20 04:11:28.980397 django-anorganization-0.1.0rc1/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3257 2023-02-09 02:19:08.000000 django-anorganization-0.1.0rc1/.gitignore
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      556 2023-02-02 02:49:22.000000 django-anorganization-0.1.0rc1/LICENSE
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       68 2023-02-17 08:09:49.000000 django-anorganization-0.1.0rc1/MANIFEST.in
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2647 2023-02-20 04:11:28.980397 django-anorganization-0.1.0rc1/PKG-INFO
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1461 2023-02-20 03:59:49.000000 django-anorganization-0.1.0rc1/README.rst
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-20 04:11:28.976397 django-anorganization-0.1.0rc1/anorganization/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      151 2023-02-17 08:09:28.000000 django-anorganization-0.1.0rc1/anorganization/apps.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-20 04:11:28.976397 django-anorganization-0.1.0rc1/anorganization/graphqls/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      470 2023-02-20 02:34:56.000000 django-anorganization-0.1.0rc1/anorganization/graphqls/membership.graphql
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      378 2023-02-18 08:53:45.000000 django-anorganization-0.1.0rc1/anorganization/graphqls/organization.graphql
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-20 04:11:28.976397 django-anorganization-0.1.0rc1/anorganization/migrations/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2598 2023-02-20 02:34:38.000000 django-anorganization-0.1.0rc1/anorganization/migrations/0001_initial.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      569 2023-02-20 03:15:27.000000 django-anorganization-0.1.0rc1/anorganization/migrations/0002_alter_membership_attributes_and_more.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-02-17 08:16:21.000000 django-anorganization-0.1.0rc1/anorganization/migrations/__init__.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      570 2023-02-17 09:02:21.000000 django-anorganization-0.1.0rc1/anorganization/mixins.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2249 2023-02-20 02:35:28.000000 django-anorganization-0.1.0rc1/anorganization/models.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3873 2023-02-20 03:29:03.000000 django-anorganization-0.1.0rc1/anorganization/resolvers.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      108 2023-02-09 03:33:10.000000 django-anorganization-0.1.0rc1/anorganization/tests.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      883 2023-02-18 10:10:35.000000 django-anorganization-0.1.0rc1/anorganization/utils.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-20 04:11:28.976397 django-anorganization-0.1.0rc1/django_anorganization.egg-info/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2647 2023-02-20 04:11:28.000000 django-anorganization-0.1.0rc1/django_anorganization.egg-info/PKG-INFO
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      719 2023-02-20 04:11:28.000000 django-anorganization-0.1.0rc1/django_anorganization.egg-info/SOURCES.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)        1 2023-02-20 04:11:28.000000 django-anorganization-0.1.0rc1/django_anorganization.egg-info/dependency_links.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      196 2023-02-20 04:11:28.000000 django-anorganization-0.1.0rc1/django_anorganization.egg-info/requires.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       26 2023-02-20 04:11:28.000000 django-anorganization-0.1.0rc1/django_anorganization.egg-info/top_level.txt
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1818 2023-02-20 03:59:51.000000 django-anorganization-0.1.0rc1/pyproject.toml
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       38 2023-02-20 04:11:28.980397 django-anorganization-0.1.0rc1/setup.cfg
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)       86 2023-02-02 02:49:22.000000 django-anorganization-0.1.0rc1/setup.py
-drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-02-20 04:11:28.976397 django-anorganization-0.1.0rc1/tests/
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)      472 2023-02-20 03:12:40.000000 django-anorganization-0.1.0rc1/tests/conftest.py
--rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2849 2023-02-20 03:28:38.000000 django-anorganization-0.1.0rc1/tests/test_resolvers.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 03:34:05.530133 django-anorganization-0.1.0rc3/
+-rwxr-xr-x   0 cchiut    (1000) cchiut    (1000)      464 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/.editorconfig
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3257 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/.gitignore
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      556 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/LICENSE
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       68 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/MANIFEST.in
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3638 2023-06-20 03:34:05.530133 django-anorganization-0.1.0rc3/PKG-INFO
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2386 2023-06-20 03:29:40.000000 django-anorganization-0.1.0rc3/README.rst
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 03:34:05.522133 django-anorganization-0.1.0rc3/anorganization/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      151 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/apps.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 03:34:05.526133 django-anorganization-0.1.0rc3/anorganization/graphqls/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1298 2023-06-20 03:07:10.000000 django-anorganization-0.1.0rc3/anorganization/graphqls/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3587 2023-06-20 02:54:29.000000 django-anorganization-0.1.0rc3/anorganization/graphqls/bindables.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3178 2023-06-20 03:01:08.000000 django-anorganization-0.1.0rc3/anorganization/graphqls/bindables_sync.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      470 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/graphqls/membership.graphql
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      398 2023-06-20 02:51:03.000000 django-anorganization-0.1.0rc3/anorganization/graphqls/organization.graphql
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1568 2023-06-20 03:01:35.000000 django-anorganization-0.1.0rc3/anorganization/graphqls/type_defs.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 03:34:05.526133 django-anorganization-0.1.0rc3/anorganization/migrations/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2441 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/migrations/0001_initial.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      569 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/migrations/0002_alter_membership_attributes_and_more.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/migrations/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      627 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/mixins.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2152 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/models.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3873 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/resolvers.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      108 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/tests.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      883 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/anorganization/utils.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 03:34:05.526133 django-anorganization-0.1.0rc3/django_anorganization.egg-info/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     3638 2023-06-20 03:34:05.000000 django-anorganization-0.1.0rc3/django_anorganization.egg-info/PKG-INFO
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      903 2023-06-20 03:34:05.000000 django-anorganization-0.1.0rc3/django_anorganization.egg-info/SOURCES.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        1 2023-06-20 03:34:05.000000 django-anorganization-0.1.0rc3/django_anorganization.egg-info/dependency_links.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      207 2023-06-20 03:34:05.000000 django-anorganization-0.1.0rc3/django_anorganization.egg-info/requires.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       26 2023-06-20 03:34:05.000000 django-anorganization-0.1.0rc3/django_anorganization.egg-info/top_level.txt
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     1874 2023-06-20 02:28:14.000000 django-anorganization-0.1.0rc3/pyproject.toml
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       38 2023-06-20 03:34:05.530133 django-anorganization-0.1.0rc3/setup.cfg
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)       86 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/setup.py
+drwxr-xr-x   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 03:34:05.530133 django-anorganization-0.1.0rc3/tests/
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)        0 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/tests/__init__.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)      472 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/tests/conftest.py
+-rw-r--r--   0 cchiut    (1000) cchiut    (1000)     2849 2023-06-20 02:20:35.000000 django-anorganization-0.1.0rc3/tests/test_resolvers.py
```

### Comparing `django-anorganization-0.1.0rc1/.gitignore` & `django-anorganization-0.1.0rc3/.gitignore`

 * *Files identical despite different names*

### Comparing `django-anorganization-0.1.0rc1/LICENSE` & `django-anorganization-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-anorganization-0.1.0rc1/README.rst` & `django-anorganization-0.1.0rc3/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 
 ------------
 Requirements
 ------------
 
 * Python 3.10+
 * django 4.0+
-* ariadne 0.16.0+
-* ariadne-relay 0.1.0a8+
 * pillow 9.4.0+
 
 --------
 Settings
 --------
 Store uploaded file with tokenize file name, default to False
 
@@ -45,27 +43,67 @@
 
 ---------------------------
 Ariadne types and resolvers
 ---------------------------
 
 Integrate predefined types and resolvers to scheme.
 
-**resolvers**
+Requirements
+------------
 
-* resolve_anorganizations
-* resolve_anorganization_memberships
+* ariadne 0.16.0+
+* ariadne-relay 0.1.0a8+
+
+**schema**
+
+.. code:: python
+
+   from anorganization.graphqls import anorganization_schema
+
+
+* anarticle/graphqls/article.graphql
+* anarticle/graphqls/tag.graphql
 
 **types**
 
+.. code:: python
+
+   from anorganization.graphqls import anorganization_bindables
+
+
 * anorganization
 * anorganization_membership
 
-**graphql**
+**resolvers**
+
+Async version
+
+.. code:: python
+
+   from anorganization.graphqls import resolve_anorganization_instance, \
+           resolve_anorganization_member_connection, resolve_anorganizations
+
+   anorganization.set_instance_resolver(resolve_anorganization_instance)
+   anorganization.set_connection('members', resolve_anorganization_member_connection)
+
+   query.set_field('organizations', resolve_anorganizations)
+
+
+* resolve_anorganization_instance
+* resolve_anorganization_member_connection
+* resolve_anorganization_membership_instance
+* resolve_anorganizations
+* resolve_anorganization_memberships
+
+Sync version
 
-* anorganization/graphqls/organization.graphql
-* anorganization/graphqls/membership.graphql
+* resolve_anorganization_instance_sync
+* resolve_anorganization_member_connection_sync
+* resolve_anorganization_membership_instance_sync
+* resolve_anorganizations_sync
+* resolve_anorganization_memberships_sync
 
 -------
 License
 -------
 
 django-anarticle is released under the terms of **Apache license**. Full details in LICENSE file.
```

### Comparing `django-anorganization-0.1.0rc1/anorganization/migrations/0001_initial.py` & `django-anorganization-0.1.0rc3/anorganization/migrations/0001_initial.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,31 +23,25 @@
                 ('dn', models.CharField(blank=True, max_length=255)),
                 ('attributes', models.JSONField(blank=True)),
                 ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anorganization.utils.image_path)),
                 ('is_valid', models.BooleanField(default=True, help_text='Designates whether the membership is valid.')),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('updated_at', models.DateTimeField(auto_now=True)),
             ],
-            options={
-                'ordering': ['-updated_at'],
-            },
         ),
         migrations.CreateModel(
             name='Organization',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('name', models.CharField(max_length=255)),
                 ('dn', models.CharField(blank=True, max_length=255)),
                 ('attributes', models.JSONField(blank=True)),
                 ('image', models.ImageField(blank=True, help_text='Upload file should under size limitation, with png, jpg or jpeg file extensions.', upload_to=anorganization.utils.image_path)),
                 ('members', models.ManyToManyField(through='anorganization.Membership', to=settings.AUTH_USER_MODEL)),
             ],
-            options={
-                'ordering': ['name'],
-            },
         ),
         migrations.AddField(
             model_name='membership',
             name='organization',
             field=models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='anorganization.organization'),
         ),
         migrations.AddField(
```

### Comparing `django-anorganization-0.1.0rc1/anorganization/migrations/0002_alter_membership_attributes_and_more.py` & `django-anorganization-0.1.0rc3/anorganization/migrations/0002_alter_membership_attributes_and_more.py`

 * *Files identical despite different names*

### Comparing `django-anorganization-0.1.0rc1/anorganization/mixins.py` & `django-anorganization-0.1.0rc3/anorganization/mixins.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Copyright (c) 2014-present, aglean Inc.
 """
 
 
 class OrganizationAdminMixin():
+    ordering = ('name',)
     list_display = ('id', 'name', 'dn', 'image', 'image_url',
                     'valid_member_count', 'invalid_member_count')
     search_fields = ('name',)
 
 
 class MembershipAdminMixin():
+    ordering = ('-updated_at',)
     list_display = ('id', 'user', 'organization', 'serial_number', 'dn',
                     'is_valid', 'created_at', 'updated_at')
     list_filter = ('organization__name', 'is_valid')
     search_fields = ('user__username', 'organization__name')
     autocomplete_fields = ('user', 'organization')
```

### Comparing `django-anorganization-0.1.0rc1/anorganization/models.py` & `django-anorganization-0.1.0rc3/anorganization/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,17 +21,14 @@
         help_text=(
             'Upload file should under size limitation, '
             'with png, jpg or jpeg file extensions.'
         ),
         blank=True
     )
 
-    class Meta:
-        ordering = ['name']
-
     def __str__(self):
         return self.name
 
     @property
     def image_url(self):
         return image_url(self)
 
@@ -69,16 +66,13 @@
         default=True
     )
 
     # datetime
     created_at = models.DateTimeField(auto_now=False, auto_now_add=True)
     updated_at = models.DateTimeField(auto_now=True, auto_now_add=False)
 
-    class Meta:
-        ordering = ['-updated_at']
-
     def __str__(self):
         return self.user.username
 
     @property
     def image_url(self):
         return image_url(self)
```

### Comparing `django-anorganization-0.1.0rc1/anorganization/resolvers.py` & `django-anorganization-0.1.0rc3/anorganization/resolvers.py`

 * *Files identical despite different names*

### Comparing `django-anorganization-0.1.0rc1/anorganization/utils.py` & `django-anorganization-0.1.0rc3/anorganization/utils.py`

 * *Files identical despite different names*

### Comparing `django-anorganization-0.1.0rc1/django_anorganization.egg-info/SOURCES.txt` & `django-anorganization-0.1.0rc3/django_anorganization.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,30 @@
+.editorconfig
 .gitignore
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.py
 anorganization/apps.py
 anorganization/mixins.py
 anorganization/models.py
 anorganization/resolvers.py
 anorganization/tests.py
 anorganization/utils.py
+anorganization/graphqls/__init__.py
+anorganization/graphqls/bindables.py
+anorganization/graphqls/bindables_sync.py
 anorganization/graphqls/membership.graphql
 anorganization/graphqls/organization.graphql
+anorganization/graphqls/type_defs.py
 anorganization/migrations/0001_initial.py
 anorganization/migrations/0002_alter_membership_attributes_and_more.py
 anorganization/migrations/__init__.py
 django_anorganization.egg-info/PKG-INFO
 django_anorganization.egg-info/SOURCES.txt
 django_anorganization.egg-info/dependency_links.txt
 django_anorganization.egg-info/requires.txt
 django_anorganization.egg-info/top_level.txt
+tests/__init__.py
 tests/conftest.py
 tests/test_resolvers.py
```

### Comparing `django-anorganization-0.1.0rc1/pyproject.toml` & `django-anorganization-0.1.0rc3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 
 [build-system]
 requires = ["setuptools>=66.1.1", "setuptools_scm[toml]>=7.1.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-anorganization"
-authors = [{ name = "Chiu T.", email = "chiutung.chen@aglean.com"}]
+authors = [{ name = "Chiu", email = "chiutung.chen@aglean.com"}]
 description = "django app for organizing users through memberships"
-keywords = ["django", "ariadne", "aglean", "organization", "membership", "role"]
+keywords = ["django", "graphql", "ariadne", "aglean", "organization", "membership", "role"]
 readme = "README.rst"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
@@ -26,21 +27,23 @@
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
     "Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Content Management System"
 ]
 requires-python = ">= 3.10"
 dependencies = [
     "django >= 4.0",
-    "ariadne >= 0.16.0",
-    "ariadne-relay >= 0.1.0a8",
     "pillow >= 9.4.0",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
+graphql = [
+    "ariadne >= 0.16.0",
+    "ariadne-relay >= 0.1.0a8",
+]
 dev = [
     "python-lsp-server[rope,pyflakes,mccabe,pycodestyle,autopep8]",
     "pylsp-rope",
 ]
 test = [
     "pytest",
     "pytest-cov",
```

### Comparing `django-anorganization-0.1.0rc1/tests/test_resolvers.py` & `django-anorganization-0.1.0rc3/tests/test_resolvers.py`

 * *Files identical despite different names*

