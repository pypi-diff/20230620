# Comparing `tmp/draper-utils-1.0.tar.gz` & `tmp/draper-utils-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "draper-utils-1.0.tar", last modified: Mon Jun 12 21:49:34 2023, max compression
+gzip compressed data, was "draper-utils-1.1.tar", last modified: Tue Jun 20 01:31:09 2023, max compression
```

## Comparing `draper-utils-1.0.tar` & `draper-utils-1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.450743 draper-utils-1.0/
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 draper-utils-1.0/LICENCE.txt
--rw-rw-rw-   0        0        0      355 2023-06-12 21:49:34.450743 draper-utils-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 draper-utils-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.372744 draper-utils-1.0/draper_utils/
--rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/__init__.py
--rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/admin.py
--rw-rw-rw-   0        0        0      161 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/apps.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.392744 draper-utils-1.0/draper_utils/management/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 draper-utils-1.0/draper_utils/management/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.407744 draper-utils-1.0/draper_utils/management/commands/
--rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 draper-utils-1.0/draper_utils/management/commands/__init__.py
--rw-rw-rw-   0        0        0    14141 2023-06-12 12:15:19.000000 draper-utils-1.0/draper_utils/management/commands/import_projects.py
--rw-rw-rw-   0        0        0     3326 2023-06-05 11:39:22.000000 draper-utils-1.0/draper_utils/management/commands/setup_project_center.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.409742 draper-utils-1.0/draper_utils/migrations/
--rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/migrations/__init__.py
--rw-rw-rw-   0        0        0       60 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/models.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.449743 draper-utils-1.0/draper_utils/sql/
--rw-rw-rw-   0        0        0       79 2023-01-04 12:10:24.000000 draper-utils-1.0/draper_utils/sql/list_project_activities.sql
--rw-rw-rw-   0        0        0      279 2023-02-09 18:41:35.000000 draper-utils-1.0/draper_utils/sql/list_project_assigned_users.sql
--rw-rw-rw-   0        0        0      228 2023-02-16 02:03:32.000000 draper-utils-1.0/draper_utils/sql/list_project_categories.sql
--rw-rw-rw-   0        0        0      172 2023-01-02 16:39:10.000000 draper-utils-1.0/draper_utils/sql/list_project_stages.sql
--rw-rw-rw-   0        0        0      178 2023-01-02 16:22:17.000000 draper-utils-1.0/draper_utils/sql/list_project_statuses.sql
--rw-rw-rw-   0        0        0      609 2023-02-05 20:55:33.000000 draper-utils-1.0/draper_utils/sql/list_project_users.sql
--rw-rw-rw-   0        0        0      399 2023-01-14 16:07:20.000000 draper-utils-1.0/draper_utils/sql/list_projects.sql
--rw-rw-rw-   0        0        0       63 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/tests.py
--rw-rw-rw-   0        0        0     7345 2023-01-29 13:45:21.000000 draper-utils-1.0/draper_utils/utils.py
--rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-1.0/draper_utils/views.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:49:34.391744 draper-utils-1.0/draper_utils.egg-info/
--rw-rw-rw-   0        0        0      355 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      925 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-31 20:41:35.000000 draper-utils-1.0/draper_utils.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-12 21:49:34.000000 draper-utils-1.0/draper_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 21:49:34.450743 draper-utils-1.0/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-06-12 21:49:22.000000 draper-utils-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.888841 draper-utils-1.1/
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:35.000000 draper-utils-1.1/LICENCE.txt
+-rw-rw-rw-   0        0        0      355 2023-06-20 01:31:09.887840 draper-utils-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-01-28 18:46:11.000000 draper-utils-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.844840 draper-utils-1.1/draper_utils/
+-rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/__init__.py
+-rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/admin.py
+-rw-rw-rw-   0        0        0      161 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/apps.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.861842 draper-utils-1.1/draper_utils/management/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:29.000000 draper-utils-1.1/draper_utils/management/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.875840 draper-utils-1.1/draper_utils/management/commands/
+-rw-rw-rw-   0        0        0        0 2022-12-23 17:39:49.000000 draper-utils-1.1/draper_utils/management/commands/__init__.py
+-rw-rw-rw-   0        0        0    14241 2023-06-19 20:09:39.000000 draper-utils-1.1/draper_utils/management/commands/import_projects.py
+-rw-rw-rw-   0        0        0     3326 2023-06-05 11:39:22.000000 draper-utils-1.1/draper_utils/management/commands/setup_project_center.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.876840 draper-utils-1.1/draper_utils/migrations/
+-rw-rw-rw-   0        0        0        0 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/migrations/__init__.py
+-rw-rw-rw-   0        0        0       60 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/models.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.886841 draper-utils-1.1/draper_utils/sql/
+-rw-rw-rw-   0        0        0       79 2023-01-04 12:10:24.000000 draper-utils-1.1/draper_utils/sql/list_project_activities.sql
+-rw-rw-rw-   0        0        0      279 2023-02-09 18:41:35.000000 draper-utils-1.1/draper_utils/sql/list_project_assigned_users.sql
+-rw-rw-rw-   0        0        0      228 2023-02-16 02:03:32.000000 draper-utils-1.1/draper_utils/sql/list_project_categories.sql
+-rw-rw-rw-   0        0        0      172 2023-01-02 16:39:10.000000 draper-utils-1.1/draper_utils/sql/list_project_stages.sql
+-rw-rw-rw-   0        0        0      178 2023-01-02 16:22:17.000000 draper-utils-1.1/draper_utils/sql/list_project_statuses.sql
+-rw-rw-rw-   0        0        0      609 2023-02-05 20:55:33.000000 draper-utils-1.1/draper_utils/sql/list_project_users.sql
+-rw-rw-rw-   0        0        0      399 2023-01-14 16:07:20.000000 draper-utils-1.1/draper_utils/sql/list_projects.sql
+-rw-rw-rw-   0        0        0       63 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/tests.py
+-rw-rw-rw-   0        0        0     7345 2023-01-29 13:45:21.000000 draper-utils-1.1/draper_utils/utils.py
+-rw-rw-rw-   0        0        0       66 2023-01-28 21:06:51.000000 draper-utils-1.1/draper_utils/views.py
+drwxrwxrwx   0        0        0        0 2023-06-20 01:31:09.860840 draper-utils-1.1/draper_utils.egg-info/
+-rw-rw-rw-   0        0        0      355 2023-06-20 01:31:09.000000 draper-utils-1.1/draper_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      925 2023-06-20 01:31:09.000000 draper-utils-1.1/draper_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 01:31:09.000000 draper-utils-1.1/draper_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-31 20:41:35.000000 draper-utils-1.1/draper_utils.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2023-06-20 01:31:09.000000 draper-utils-1.1/draper_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-20 01:31:09.000000 draper-utils-1.1/draper_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-20 01:31:09.888841 draper-utils-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-06-20 01:30:06.000000 draper-utils-1.1/setup.py
```

### Comparing `draper-utils-1.0/draper_utils/management/commands/import_projects.py` & `draper-utils-1.1/draper_utils/management/commands/import_projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,14 +254,16 @@
                         'name':row.activity_name,
                         'project':project,
                         'date':activity_date,
                         'user':User.objects.get(import_id=row.creator_id),
                         'notes':row.notes,
                     })
                     activity._change_reason = activity.name
+                    if row.is_final_locked_file == 1:
+                        activity.pin = True
                     activity.save()
                     if url:
                         r = requests.get(url)
                         if r.status_code == 200:
                             data = r.content
                             filename = url.split('/')[-1]
                             activity.file.save(filename, ContentFile(data))
```

### Comparing `draper-utils-1.0/draper_utils/management/commands/setup_project_center.py` & `draper-utils-1.1/draper_utils/management/commands/setup_project_center.py`

 * *Files identical despite different names*

### Comparing `draper-utils-1.0/draper_utils/sql/list_project_users.sql` & `draper-utils-1.1/draper_utils/sql/list_project_users.sql`

 * *Files identical despite different names*

### Comparing `draper-utils-1.0/draper_utils/utils.py` & `draper-utils-1.1/draper_utils/utils.py`

 * *Files identical despite different names*

### Comparing `draper-utils-1.0/draper_utils.egg-info/SOURCES.txt` & `draper-utils-1.1/draper_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draper-utils-1.0/setup.py` & `draper-utils-1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 
 # https://pypi.python.org/pypi?%3Aaction=list_classifiers
 CLASSIFIERS = []
 
 setup(
     name='draper-utils',
-    version='1.0',
+    version='1.1',
     description='Project Management Module for Django - Utils',
     author='siteshell.net',
     author_email='pdbethke@siteshell.net',
     url='https://github.com/pdbethke/draper-utils',
     packages=find_packages(exclude=('tests', 'docs')),
     package_dir={'draper_utils': 'draper_utils'},
     package_data={'draper_utils': ['sql/*', 'management/*', 'migrations/*']},
```

