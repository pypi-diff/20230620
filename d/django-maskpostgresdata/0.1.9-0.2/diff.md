# Comparing `tmp/django-maskpostgresdata-0.1.9.tar.gz` & `tmp/django-maskpostgresdata-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-maskpostgresdata-0.1.9.tar", last modified: Fri Oct  4 08:50:20 2019, max compression
+gzip compressed data, was "django-maskpostgresdata-0.2.tar", last modified: Tue Jun 20 13:19:35 2023, max compression
```

## Comparing `django-maskpostgresdata-0.1.9.tar` & `django-maskpostgresdata-0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/
--rw-r--r--   0 ikonitas   (501) staff       (20)     2618 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/PKG-INFO
-drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/
-drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/
--rw-r--r--   0 ikonitas   (501) staff       (20)        0 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/__init__.py
-drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/
--rw-r--r--   0 ikonitas   (501) staff       (20)        0 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/__init__.py
--rw-r--r--   0 ikonitas   (501) staff       (20)     5074 2019-10-04 08:21:41.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/dump_masked_data.py
--rw-r--r--   0 ikonitas   (501) staff       (20)       92 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/maskpostgresdata/__init__.py
--rw-r--r--   0 ikonitas   (501) staff       (20)       19 2019-10-03 08:19:48.000000 django-maskpostgresdata-0.1.9/MANIFEST.in
--rw-r--r--   0 ikonitas   (501) staff       (20)     1792 2019-10-03 08:24:56.000000 django-maskpostgresdata-0.1.9/README.md
-drwxr-xr-x   0 ikonitas   (501) staff       (20)        0 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/
--rw-r--r--   0 ikonitas   (501) staff       (20)     2618 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/PKG-INFO
--rw-r--r--   0 ikonitas   (501) staff       (20)        1 2019-10-03 08:19:49.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/not-zip-safe
--rw-r--r--   0 ikonitas   (501) staff       (20)      495 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/SOURCES.txt
--rw-r--r--   0 ikonitas   (501) staff       (20)       21 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/requires.txt
--rw-r--r--   0 ikonitas   (501) staff       (20)       17 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/top_level.txt
--rw-r--r--   0 ikonitas   (501) staff       (20)        1 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/django_maskpostgresdata.egg-info/dependency_links.txt
--rw-r--r--   0 ikonitas   (501) staff       (20)      656 2019-10-04 08:44:05.000000 django-maskpostgresdata-0.1.9/setup.py
--rw-r--r--   0 ikonitas   (501) staff       (20)       79 2019-10-04 08:50:20.000000 django-maskpostgresdata-0.1.9/setup.cfg
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-20 13:19:35.941002 django-maskpostgresdata-0.2/
+-rw-r--r--   0 tomkins    (501) staff       (20)       19 2019-08-13 10:47:54.000000 django-maskpostgresdata-0.2/MANIFEST.in
+-rw-r--r--   0 tomkins    (501) staff       (20)     2137 2023-06-20 13:19:35.941074 django-maskpostgresdata-0.2/PKG-INFO
+-rw-r--r--   0 tomkins    (501) staff       (20)     1792 2019-08-28 22:56:39.000000 django-maskpostgresdata-0.2/README.md
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-20 13:19:35.939948 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/
+-rw-r--r--   0 tomkins    (501) staff       (20)     2137 2023-06-20 13:19:35.000000 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/PKG-INFO
+-rw-r--r--   0 tomkins    (501) staff       (20)      495 2023-06-20 13:19:35.000000 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/SOURCES.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)        1 2023-06-20 13:19:35.000000 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/dependency_links.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)        1 2023-06-20 13:19:35.000000 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/not-zip-safe
+-rw-r--r--   0 tomkins    (501) staff       (20)       27 2023-06-20 13:19:35.000000 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/requires.txt
+-rw-r--r--   0 tomkins    (501) staff       (20)       17 2023-06-20 13:19:35.000000 django-maskpostgresdata-0.2/django_maskpostgresdata.egg-info/top_level.txt
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-20 13:19:35.940062 django-maskpostgresdata-0.2/maskpostgresdata/
+-rw-r--r--   0 tomkins    (501) staff       (20)       92 2019-08-28 22:56:39.000000 django-maskpostgresdata-0.2/maskpostgresdata/__init__.py
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-20 13:19:35.940288 django-maskpostgresdata-0.2/maskpostgresdata/management/
+-rw-r--r--   0 tomkins    (501) staff       (20)        0 2019-08-13 10:47:54.000000 django-maskpostgresdata-0.2/maskpostgresdata/management/__init__.py
+drwxr-xr-x   0 tomkins    (501) staff       (20)        0 2023-06-20 13:19:35.940488 django-maskpostgresdata-0.2/maskpostgresdata/management/commands/
+-rw-r--r--   0 tomkins    (501) staff       (20)        0 2019-08-13 10:47:54.000000 django-maskpostgresdata-0.2/maskpostgresdata/management/commands/__init__.py
+-rw-r--r--   0 tomkins    (501) staff       (20)     7145 2023-06-20 10:38:31.000000 django-maskpostgresdata-0.2/maskpostgresdata/management/commands/dump_masked_data.py
+-rw-r--r--   0 tomkins    (501) staff       (20)       79 2023-06-20 13:19:35.941541 django-maskpostgresdata-0.2/setup.cfg
+-rw-r--r--   0 tomkins    (501) staff       (20)      683 2023-06-20 10:40:43.000000 django-maskpostgresdata-0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `django-maskpostgresdata-0.1.9/PKG-INFO` & `django-maskpostgresdata-0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,56 @@
-Metadata-Version: 2.1
-Name: django-maskpostgresdata
-Version: 0.1.9
-Summary: Creates a pg_dumpish output which masks data without saving changes to the source database.
-Home-page: https://github.com/developersociety/django-maskpostgresdata
-Author: Developer Society
-Author-email: hello@dev.ngo
-License: BSD
-Description: Django Mask Postgres Data
-        =========================
-        
-        Adds a management command to your Django project which allows you to create a (sort of) pg_dump
-        of your data with sensitive data masked.
-        
-        Installation
-        ------------
-        
-        Install with pip:
-        
-        `pip install django-maskpostgresdata`
-        
-        And add `maskpostgresdata` to your `INSTALLED_APPS`:
-        
-        ```
-        INSTALLED_APPS = [
-            ...
-            'maskpostgresdata',
-            ...
-        ]
-        ```
-        
-        Usage
-        -----
-        
-        By default, `django-maskpostgresdata` will replace the `password` column for each row in the Django `User` model with "password". Just run `manage.py dump_masked_data` and you'll get a pg_dump with the password field changed to "password" for all users.
-        
-        There are 2 ways to customise the behaviour of `django-maskpostgresdata`.
-        
-        To override individual fields of a model with a given value, add a dictionary called `MASKER_FIELDS` to your settings using the following format:
-        
-        ```
-        MASKER_FIELDS = {
-            "{ APP_NAME }": {"{ MODEL_NAME }": {"{ FIELD_NAME }": { VALUE },}},
-        }
-        ```
-        
-        Alternatively, you can define exactly how the data is updated by subclassing `BasePostgresDataMaskingCommand` in a management command of your own. For example:
-        
-        ```
-        from django.contrib.auth.hashers import make_password
-        
-        from maskpostgresdata import BasePostgresDataMaskingCommand
-        
-        
-        class Command(BasePostgresDataMaskingCommand):
-        
-            def update_auth_user(self, queryset):
-                queryset.update(password=make_password("a_different_password"))
-        
-        ```
-        
-        Just create a method called `update_{ db_table_name }` taking a `queryset` as the parameter. You can then perform `update` operations on this queryset. `{ db_table_name }` is of the format `{app_label}_{model_name}` by default, but could technically be different.
-        
-        You can then run `manage.py dump_masked_data` and it will dump your data to `stdout`.
-        
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
+Django Mask Postgres Data
+=========================
+
+Adds a management command to your Django project which allows you to create a (sort of) pg_dump
+of your data with sensitive data masked.
+
+Installation
+------------
+
+Install with pip:
+
+`pip install django-maskpostgresdata`
+
+And add `maskpostgresdata` to your `INSTALLED_APPS`:
+
+```
+INSTALLED_APPS = [
+    ...
+    'maskpostgresdata',
+    ...
+]
+```
+
+Usage
+-----
+
+By default, `django-maskpostgresdata` will replace the `password` column for each row in the Django `User` model with "password". Just run `manage.py dump_masked_data` and you'll get a pg_dump with the password field changed to "password" for all users.
+
+There are 2 ways to customise the behaviour of `django-maskpostgresdata`.
+
+To override individual fields of a model with a given value, add a dictionary called `MASKER_FIELDS` to your settings using the following format:
+
+```
+MASKER_FIELDS = {
+    "{ APP_NAME }": {"{ MODEL_NAME }": {"{ FIELD_NAME }": { VALUE },}},
+}
+```
+
+Alternatively, you can define exactly how the data is updated by subclassing `BasePostgresDataMaskingCommand` in a management command of your own. For example:
+
+```
+from django.contrib.auth.hashers import make_password
+
+from maskpostgresdata import BasePostgresDataMaskingCommand
+
+
+class Command(BasePostgresDataMaskingCommand):
+
+    def update_auth_user(self, queryset):
+        queryset.update(password=make_password("a_different_password"))
+
+```
+
+Just create a method called `update_{ db_table_name }` taking a `queryset` as the parameter. You can then perform `update` operations on this queryset. `{ db_table_name }` is of the format `{app_label}_{model_name}` by default, but could technically be different.
+
+You can then run `manage.py dump_masked_data` and it will dump your data to `stdout`.
```

### Comparing `django-maskpostgresdata-0.1.9/maskpostgresdata/management/commands/dump_masked_data.py` & `django-maskpostgresdata-0.2/maskpostgresdata/management/commands/dump_masked_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,28 @@
 import os
 import subprocess
+import sys
 
 from django.apps import apps
 from django.conf import settings
 from django.contrib.auth.hashers import make_password
 from django.core.management.base import BaseCommand
 from django.db import DEFAULT_DB_ALIAS, connections, transaction
 
-from psycopg2.extensions import ISOLATION_LEVEL_SERIALIZABLE
+from psycopg import IsolationLevel
 
 
 class Command(BaseCommand):
-    help = ("Prints a (sort of) pg_dump of the db with sensitive data masked.")
+    help = "Prints a (sort of) pg_dump of the db with sensitive data masked."
 
-    requires_system_checks = False
+    requires_system_checks = []
 
     def add_arguments(self, parser):
         parser.add_argument(
-            "--database",
-            action="store",
-            dest="database",
-            default=DEFAULT_DB_ALIAS,
+            "--database", action="store", dest="database", default=DEFAULT_DB_ALIAS,
         )
 
     def update_auth_user(self, queryset):
         queryset.update(password=make_password("password"))
 
     def reset_sequences(self, cursor):
         """
@@ -34,31 +32,46 @@
         cursor.execute("SELECT sequence_name FROM information_schema.sequences;")
         rows = cursor.fetchall()
         for row in rows:
             sequence_name = row[0]
 
             # Get the last value for the sequence
             cursor.execute(
-                "SELECT last_value FROM {sequence_name}".format(sequence_name=sequence_name)
+                "SELECT last_value FROM {sequence_name}".format(
+                    sequence_name=sequence_name
+                )
             )
             last_value = cursor.fetchone()[0]
 
-            print("SELECT pg_catalog.setval('public.{sequence_name}', {last_value});".format(
-                sequence_name=sequence_name, last_value=last_value
-            ), flush=True)
+            self.stdout.write(
+                "SELECT pg_catalog.setval('public.{sequence_name}', {last_value});".format(
+                    sequence_name=sequence_name, last_value=last_value
+                ),
+            )
 
     def handle(self, **options):
-        connection = connections[options["database"]]
+        try:
+            self.process_data(**options)
+        except KeyboardInterrupt:
+            self.stdout.write("\n")
+            self.stdout.write("-- Keyboard interaction detected")
+            sys.exit(0)
+        except BrokenPipeError:
+            # Usually the result of a connection drop during the command - there's no point in
+            # printing any response, as that's the cause of the problem!
+            sys.exit(0)
 
+    def process_data(self, **options):
+        connection = connections[options["database"]]
         args = ["pg_dump"]
 
         conn_params = connection.get_connection_params()
         host = conn_params.get("host", "")
         port = conn_params.get("port", "")
-        dbname = conn_params.get("database", "")
+        dbname = conn_params.get("dbname", "")
         user = conn_params.get("user", "")
         passwd = conn_params.get("password", "")
 
         if user:
             args += ["-U", user]
         if host:
             args += ["-h", host]
@@ -66,69 +79,109 @@
             args += ["-p", str(port)]
         args += [dbname]
 
         subprocess_env = os.environ.copy()
         if passwd:
             subprocess_env["PGPASSWORD"] = str(passwd)
 
-        masker_args = getattr(settings, "MASKER_ARGS", ["--no-owner", "--no-privileges"])
+        masker_args = getattr(
+            settings, "MASKER_ARGS", ["--no-owner", "--no-privileges"]
+        )
         if masker_args:
             args += masker_args
 
         connection.ensure_connection()
         connection.set_autocommit(False)
 
-        if connection.isolation_level != ISOLATION_LEVEL_SERIALIZABLE:
-            connection.connection.set_session(isolation_level=ISOLATION_LEVEL_SERIALIZABLE)
-            connection.isolation_level = ISOLATION_LEVEL_SERIALIZABLE
-            connection.connection.isolation_level = ISOLATION_LEVEL_SERIALIZABLE
+        if connection.isolation_level != IsolationLevel.SERIALIZABLE:
+            connection.isolation_level = IsolationLevel.SERIALIZABLE
+            connection.connection.isolation_level = IsolationLevel.SERIALIZABLE
 
         cursor = connection.cursor()
         cursor.execute("SELECT pg_export_snapshot();")
         snapshot_id = cursor.fetchone()[0]
 
         args += ["--snapshot={}".format(snapshot_id)]
 
         header_dump = args + ["--section=pre-data"]
-        subprocess.run(header_dump, stdout=self.stdout._out, env=subprocess_env)
+        subprocess.run(header_dump, env=subprocess_env)
 
         fields_to_mask = getattr(settings, "MASKER_FIELDS", None)
         altered_tables = []
 
         for app in apps.get_app_configs():
             for model in app.get_models():
                 table_name = model._default_manager.model._meta.db_table
-                if hasattr(self, 'update_{}'.format(table_name)):
-                    getattr(self, 'update_{}'.format(table_name))(model._default_manager.all())
+                if hasattr(self, "update_{}".format(table_name)):
+                    getattr(self, "update_{}".format(table_name))(
+                        model._default_manager.all()
+                    )
 
         if fields_to_mask:
             for app in fields_to_mask.keys():
                 for model, fields in fields_to_mask[app].items():
                     model_class = apps.get_model(app.lower(), model_name=model.lower())
                     model_class._default_manager.update(**fields)
                     table_name = model_class._default_manager.model._meta.db_table
 
                     altered_tables.append(table_name)
-                    print("COPY public.{} FROM stdin;".format(table_name), flush=True)
-                    cursor.copy_to(self.stdout._out, table_name)
-                    print("\\.\n", file=self.stdout._out, flush=True)
+                    self.stdout.write("COPY public.{} FROM stdin;".format(table_name))
+                    self.stdout.flush()
+                    with cursor.copy("COPY public.{} TO STDOUT".format(table_name)) as copy:
+                        while data := copy.read():
+                            sys.stdout.buffer.write(data)
+                    self.stdout.write("\\.\n")
 
+        copied_tables = []
         for app in apps.get_app_configs():
+            # GeoDjango tables are automatically created by postgis, and we can't use COPY on them
+            if app.name == "django.contrib.gis":
+                continue
+
             for model in app.get_models():
+                if model._meta.proxy:
+                    # Proxy models have another underlying model/table - so skip
+                    continue
+
                 table_name = model._default_manager.model._meta.db_table
 
-                if table_name not in altered_tables:
-                    print("COPY public.{} FROM stdin;".format(table_name), flush=True)
-                    cursor.copy_to(self.stdout._out, table_name)
-                    print("\\.\n", file=self.stdout._out, flush=True)
-
-        print("COPY public.django_migrations FROM stdin;".format(table_name), flush=True)
-        cursor.copy_to(self.stdout._out, 'django_migrations')
-        print("\\.\n", file=self.stdout._out, flush=True)
+                if table_name not in altered_tables and table_name not in copied_tables:
+                    self.stdout.write("COPY public.{} FROM stdin;".format(table_name))
+                    self.stdout.flush()
+                    with cursor.copy("COPY public.{} TO STDOUT".format(table_name)) as copy:
+                        while data := copy.read():
+                            sys.stdout.buffer.write(data)
+                    self.stdout.write("\\.\n")
+
+                    copied_tables.append(table_name)
+
+                for field in model._meta.local_many_to_many:
+                    m2m_table_name = field.m2m_db_table()
+
+                    if (
+                        m2m_table_name not in altered_tables
+                        and m2m_table_name not in copied_tables # noqa
+                    ):
+                        self.stdout.write("COPY public.{} FROM stdin;".format(m2m_table_name))
+                        self.stdout.flush()
+                        with cursor.copy("COPY public.{} TO STDOUT".format(m2m_table_name)) as copy:
+                            while data := copy.read():
+                                sys.stdout.buffer.write(data)
+                        self.stdout.write("\\.\n")
+
+                        copied_tables.append(m2m_table_name)
+
+        self.stdout.write("COPY public.django_migrations FROM stdin;".format(table_name))
+        self.stdout.flush()
+        with cursor.copy("COPY public.django_migrations TO STDOUT") as copy:
+            while data := copy.read():
+                sys.stdout.buffer.write(data)
+        self.stdout.write("\\.\n")
 
         # Sets a new values for sequences.
         self.reset_sequences(cursor)
 
         post_data_dump = args + ["--section=post-data"]
-        subprocess.run(post_data_dump, stdout=self.stdout._out, env=subprocess_env)
+        self.stdout.flush()
+        subprocess.run(post_data_dump, env=subprocess_env)
 
         transaction.rollback()
```

### Comparing `django-maskpostgresdata-0.1.9/setup.py` & `django-maskpostgresdata-0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(
     name='django-maskpostgresdata',
     packages=find_packages(),
-    version='0.1.9',
+    version='0.2',
     description=(
         'Creates a pg_dumpish output which masks data without saving changes to the source '
         'database.'
     ),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/developersociety/django-maskpostgresdata',
     author='Developer Society',
     author_email='hello@dev.ngo',
     license='BSD',
     zip_safe=False,
-    install_requires=['django>=1.8', 'psycopg2']
+    install_requires=[
+        'django>=4.2',
+        'psycopg>=3.1.8',
+    ]
 )
```

