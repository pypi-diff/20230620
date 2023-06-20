# Comparing `tmp/groupeffect-0.1.1.tar.gz` & `tmp/groupeffect-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupeffect-0.1.1.tar", last modified: Sat Jun 17 14:15:07 2023, max compression
+gzip compressed data, was "groupeffect-0.1.10.tar", last modified: Tue Jun 20 20:26:04 2023, max compression
```

## Comparing `groupeffect-0.1.1.tar` & `groupeffect-0.1.10.tar`

### file list

```diff
@@ -1,42 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/
--rwxrwxrwx   0 root         (0) root         (0)     1068 2023-04-01 18:23:21.000000 groupeffect-0.1.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       75 2023-06-17 11:59:17.000000 groupeffect-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-17 14:15:07.321877 groupeffect-0.1.1/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     1128 2023-06-17 14:14:46.000000 groupeffect-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      160 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/admin.py
--rw-rw-r--   0 root         (0) root         (0)      154 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/database/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/database/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      273 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/database/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/management/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/management/commands/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/management/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       52 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/management/commands/effect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/migrations/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/migrations/__init__.py
--rw-rw-r--   0 root         (0) root         (0)       59 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/serializers/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/serializers/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      252 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/serializers/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.317877 groupeffect-0.1.1/groupeffect/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/templates/rest_framework/
--rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/templates/rest_framework/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/tests/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/urls/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/urls/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      253 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/urls/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect/views/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/views/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      423 2023-06-17 11:59:17.000000 groupeffect-0.1.1/groupeffect/views/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-17 14:15:07.321877 groupeffect-0.1.1/groupeffect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1854 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      781 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-17 14:15:07.000000 groupeffect-0.1.1/groupeffect.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      814 2023-06-17 14:15:07.321877 groupeffect-0.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)       38 2023-06-17 11:59:17.000000 groupeffect-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/
+-rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.1.10/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.1.10/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-06-20 20:26:04.850183 groupeffect-0.1.10/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     2675 2023-06-20 20:21:23.000000 groupeffect-0.1.10/README.md
+-rw-rw-r--   0 root         (0) root         (0)      191 2023-06-20 20:26:04.000000 groupeffect-0.1.10/VERSION.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.1.10/groupeffect/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.1.10/groupeffect/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.1.10/groupeffect/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5529 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/management/commands/effect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/management/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/management/configuration/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/management/tasks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/management/tasks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/management/tasks/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/templates/groupeffect/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/templates/groupeffect/default/
+-rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/templates/groupeffect/default/database.txt
+-rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/templates/groupeffect/default/serializers.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/templates/groupeffect/default/tests.txt
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/templates/groupeffect/default/urls.txt
+-rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/templates/groupeffect/default/views.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect/templates/groupeffect/web/
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.1.10/groupeffect/templates/groupeffect/web/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:26:04.846183 groupeffect-0.1.10/groupeffect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-06-20 20:26:04.000000 groupeffect-0.1.10/groupeffect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      846 2023-06-20 20:26:04.000000 groupeffect-0.1.10/groupeffect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:26:04.000000 groupeffect-0.1.10/groupeffect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 20:26:04.000000 groupeffect-0.1.10/groupeffect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 20:26:04.000000 groupeffect-0.1.10/groupeffect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      822 2023-06-20 20:26:04.850183 groupeffect-0.1.10/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      417 2023-06-20 20:23:01.000000 groupeffect-0.1.10/setup.py
```

### Comparing `groupeffect-0.1.1/LICENSE` & `groupeffect-0.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `groupeffect-0.1.1/groupeffect/templates/rest_framework/api.html` & `groupeffect-0.1.10/groupeffect/templates/groupeffect/web/api.html`

 * *Files identical despite different names*

### Comparing `groupeffect-0.1.1/setup.cfg` & `groupeffect-0.1.10/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = groupeffect
-version = 0.1.1
-description = A Django app to load dev stuff.
+version = 0.1.10
+description = A Django app for fast api development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Groupeffect/groupeffect-pypi
 author = Amir Yousefi
 author_email = groupeffect.public@gmail.com
 license = MIT
 classifiers =
```

