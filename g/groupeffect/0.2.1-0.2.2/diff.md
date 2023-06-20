# Comparing `tmp/groupeffect-0.2.1.tar.gz` & `tmp/groupeffect-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupeffect-0.2.1.tar", last modified: Tue Jun 20 20:29:41 2023, max compression
+gzip compressed data, was "groupeffect-0.2.2.tar", last modified: Tue Jun 20 20:39:01 2023, max compression
```

## Comparing `groupeffect-0.2.1.tar` & `groupeffect-0.2.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/
--rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3408 2023-06-20 20:29:41.188534 groupeffect-0.2.1/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     2675 2023-06-20 20:21:23.000000 groupeffect-0.2.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      190 2023-06-20 20:29:40.000000 groupeffect-0.2.1/VERSION.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.1/groupeffect/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.1/groupeffect/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.1/groupeffect/management/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5529 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/management/commands/effect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/management/configuration/
--rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/management/configuration/default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/management/tasks/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/management/tasks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/management/tasks/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.184534 groupeffect-0.2.1/groupeffect/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.184534 groupeffect-0.2.1/groupeffect/templates/groupeffect/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/templates/groupeffect/default/
--rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/templates/groupeffect/default/database.txt
--rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/templates/groupeffect/default/serializers.txt
--rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/templates/groupeffect/default/tests.txt
--rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/templates/groupeffect/default/urls.txt
--rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/templates/groupeffect/default/views.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect/templates/groupeffect/web/
--rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.1/groupeffect/templates/groupeffect/web/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:29:41.188534 groupeffect-0.2.1/groupeffect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3408 2023-06-20 20:29:41.000000 groupeffect-0.2.1/groupeffect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      846 2023-06-20 20:29:41.000000 groupeffect-0.2.1/groupeffect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:29:41.000000 groupeffect-0.2.1/groupeffect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 20:29:41.000000 groupeffect-0.2.1/groupeffect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 20:29:41.000000 groupeffect-0.2.1/groupeffect.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      821 2023-06-20 20:29:41.188534 groupeffect-0.2.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      417 2023-06-20 20:23:01.000000 groupeffect-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/
+-rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.2/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-06-20 20:39:01.078676 groupeffect-0.2.2/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     2775 2023-06-20 20:37:48.000000 groupeffect-0.2.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      190 2023-06-20 20:39:00.000000 groupeffect-0.2.2/VERSION.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.2/groupeffect/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.2/groupeffect/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.2/groupeffect/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5529 2023-06-20 20:33:30.000000 groupeffect-0.2.2/groupeffect/management/commands/effect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/management/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/management/configuration/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/management/tasks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/management/tasks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/management/tasks/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/templates/groupeffect/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/
+-rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/database.txt
+-rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/serializers.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/tests.txt
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/urls.txt
+-rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/views.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/templates/groupeffect/web/
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/web/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3508 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      846 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      821 2023-06-20 20:39:01.078676 groupeffect-0.2.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      417 2023-06-20 20:23:01.000000 groupeffect-0.2.2/setup.py
```

### Comparing `groupeffect-0.2.1/LICENSE` & `groupeffect-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.1/PKG-INFO` & `groupeffect-0.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupeffect
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django app for fast api development.
 Home-page: https://github.com/Groupeffect/groupeffect-pypi
 Author: Amir Yousefi
 Author-email: groupeffect.public@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,18 +19,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GROUPEFFECT-PYPI
 
 Django app with rest framework integration for fast development.
 Write task classes instead of management commands for faster cli integrations.
-Run enhanced `startapp` command to generate boilerplate `ModeViewSets` from a configuration file.
+Run enhanced `startapp` command to generate boilerplate `ModelViewSets` from a configuration file.
+
+**Package code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi/tree/main/framework/pypi/app/package
 
+**Development code on Github**
+
+https://github.com/Groupeffect/groupeffect-pypi
+
 
 # Quick start
 
 1. Add "groupeffect" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [ 
         ... 
@@ -79,15 +85,15 @@
 
 - startapp with nested folders
 
     - from config file
 
     `GROUPEFFECT_CONFIG_JSON_FILE_PATH`
 
-    `python manage.py effect -c app -t start -t config`
+    `python manage.py effect -c app -t start`
 
 
 **Tasks** 
 
 You can add task classes to the array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs.
 
 Example:
```

### Comparing `groupeffect-0.2.1/README.md` & `groupeffect-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # GROUPEFFECT-PYPI
 
 Django app with rest framework integration for fast development.
 Write task classes instead of management commands for faster cli integrations.
-Run enhanced `startapp` command to generate boilerplate `ModeViewSets` from a configuration file.
+Run enhanced `startapp` command to generate boilerplate `ModelViewSets` from a configuration file.
+
+**Package code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi/tree/main/framework/pypi/app/package
 
+**Development code on Github**
+
+https://github.com/Groupeffect/groupeffect-pypi
+
 
 # Quick start
 
 1. Add "groupeffect" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [ 
         ... 
@@ -58,15 +64,15 @@
 
 - startapp with nested folders
 
     - from config file
 
     `GROUPEFFECT_CONFIG_JSON_FILE_PATH`
 
-    `python manage.py effect -c app -t start -t config`
+    `python manage.py effect -c app -t start`
 
 
 **Tasks** 
 
 You can add task classes to the array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs.
 
 Example:
```

### Comparing `groupeffect-0.2.1/groupeffect/management/commands/effect.py` & `groupeffect-0.2.2/groupeffect/management/commands/effect.py`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.1/groupeffect/management/tasks/default.py` & `groupeffect-0.2.2/groupeffect/management/tasks/default.py`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.1/groupeffect/templates/groupeffect/web/api.html` & `groupeffect-0.2.2/groupeffect/templates/groupeffect/web/api.html`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.1/groupeffect.egg-info/PKG-INFO` & `groupeffect-0.2.2/groupeffect.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupeffect
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Django app for fast api development.
 Home-page: https://github.com/Groupeffect/groupeffect-pypi
 Author: Amir Yousefi
 Author-email: groupeffect.public@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -19,18 +19,24 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GROUPEFFECT-PYPI
 
 Django app with rest framework integration for fast development.
 Write task classes instead of management commands for faster cli integrations.
-Run enhanced `startapp` command to generate boilerplate `ModeViewSets` from a configuration file.
+Run enhanced `startapp` command to generate boilerplate `ModelViewSets` from a configuration file.
+
+**Package code on Github**
 
 https://github.com/Groupeffect/groupeffect-pypi/tree/main/framework/pypi/app/package
 
+**Development code on Github**
+
+https://github.com/Groupeffect/groupeffect-pypi
+
 
 # Quick start
 
 1. Add "groupeffect" to your INSTALLED_APPS setting like this::
 
     INSTALLED_APPS = [ 
         ... 
@@ -79,15 +85,15 @@
 
 - startapp with nested folders
 
     - from config file
 
     `GROUPEFFECT_CONFIG_JSON_FILE_PATH`
 
-    `python manage.py effect -c app -t start -t config`
+    `python manage.py effect -c app -t start`
 
 
 **Tasks** 
 
 You can add task classes to the array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs.
 
 Example:
```

### Comparing `groupeffect-0.2.1/groupeffect.egg-info/SOURCES.txt` & `groupeffect-0.2.2/groupeffect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.1/setup.cfg` & `groupeffect-0.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = groupeffect
-version = 0.2.1
+version = 0.2.2
 description = A Django app for fast api development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Groupeffect/groupeffect-pypi
 author = Amir Yousefi
 author_email = groupeffect.public@gmail.com
 license = MIT
```

