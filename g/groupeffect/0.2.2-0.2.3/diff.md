# Comparing `tmp/groupeffect-0.2.2.tar.gz` & `tmp/groupeffect-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groupeffect-0.2.2.tar", last modified: Tue Jun 20 20:39:01 2023, max compression
+gzip compressed data, was "groupeffect-0.2.3.tar", last modified: Tue Jun 20 20:46:55 2023, max compression
```

## Comparing `groupeffect-0.2.2.tar` & `groupeffect-0.2.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/
--rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.2/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3508 2023-06-20 20:39:01.078676 groupeffect-0.2.2/PKG-INFO
--rwxrwxr-x   0 root         (0) root         (0)     2775 2023-06-20 20:37:48.000000 groupeffect-0.2.2/README.md
--rw-rw-r--   0 root         (0) root         (0)      190 2023-06-20 20:39:00.000000 groupeffect-0.2.2/VERSION.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.2/groupeffect/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/apps.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/management/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.2/groupeffect/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.2/groupeffect/management/commands/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5529 2023-06-20 20:33:30.000000 groupeffect-0.2.2/groupeffect/management/commands/effect.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/management/configuration/
--rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/management/configuration/default.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/management/tasks/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/management/tasks/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/management/tasks/default.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect/templates/groupeffect/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/
--rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/database.txt
--rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/serializers.txt
--rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/tests.txt
--rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/urls.txt
--rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/default/views.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.078676 groupeffect-0.2.2/groupeffect/templates/groupeffect/web/
--rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.2/groupeffect/templates/groupeffect/web/api.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:39:01.074676 groupeffect-0.2.2/groupeffect.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3508 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      846 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 20:39:01.000000 groupeffect-0.2.2/groupeffect.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)      821 2023-06-20 20:39:01.078676 groupeffect-0.2.2/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      417 2023-06-20 20:23:01.000000 groupeffect-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/
+-rwxrwxr-x   0 root         (0) root         (0)     1068 2023-06-20 17:39:47.000000 groupeffect-0.2.3/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      141 2023-06-20 20:21:23.000000 groupeffect-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-06-20 20:46:55.229185 groupeffect-0.2.3/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)     2870 2023-06-20 20:45:33.000000 groupeffect-0.2.3/README.md
+-rw-rw-r--   0 root         (0) root         (0)      190 2023-06-20 20:46:54.000000 groupeffect-0.2.3/VERSION.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:11:47.000000 groupeffect-0.2.3/groupeffect/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      146 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/apps.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.3/groupeffect/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 18:13:00.000000 groupeffect-0.2.3/groupeffect/management/commands/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5529 2023-06-20 20:33:30.000000 groupeffect-0.2.3/groupeffect/management/commands/effect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/configuration/
+-rw-rw-r--   0 root         (0) root         (0)      205 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/management/configuration/default.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/management/tasks/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/management/tasks/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5510 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/management/tasks/default.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.225185 groupeffect-0.2.3/groupeffect/templates/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.225185 groupeffect-0.2.3/groupeffect/templates/groupeffect/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/
+-rw-rw-r--   0 root         (0) root         (0)      240 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/database.txt
+-rw-rw-r--   0 root         (0) root         (0)      260 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/serializers.txt
+-rw-rw-r--   0 root         (0) root         (0)       72 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/tests.txt
+-rw-rw-r--   0 root         (0) root         (0)      280 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/urls.txt
+-rw-rw-r--   0 root         (0) root         (0)      429 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/default/views.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect/templates/groupeffect/web/
+-rw-rw-r--   0 root         (0) root         (0)     2056 2023-06-20 20:21:23.000000 groupeffect-0.2.3/groupeffect/templates/groupeffect/web/api.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 20:46:55.229185 groupeffect-0.2.3/groupeffect.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3603 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      846 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-06-20 20:46:55.000000 groupeffect-0.2.3/groupeffect.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)      821 2023-06-20 20:46:55.233185 groupeffect-0.2.3/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      417 2023-06-20 20:23:01.000000 groupeffect-0.2.3/setup.py
```

### Comparing `groupeffect-0.2.2/LICENSE` & `groupeffect-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.2/PKG-INFO` & `groupeffect-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupeffect
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Django app for fast api development.
 Home-page: https://github.com/Groupeffect/groupeffect-pypi
 Author: Amir Yousefi
 Author-email: groupeffect.public@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -40,19 +40,14 @@
 
     INSTALLED_APPS = [ 
         ... 
         groupeffect,
         ...
     ]
 
-`python manage.py makemigrations` -> add Namespace model 
-
-`python manage.py migrate` -> migrates Namespace model 
-
-
 ## Requirements
 
 - https://github.com/django/django
 
 - https://www.django-rest-framework.org/
 
 ## Params in settings.py
@@ -70,35 +65,39 @@
 `python manage.py effect -d`
 
 - help and usage
 
 `python manage.py effect -h`
 
 - create config file
+
+    - in BASE_DIR folder  
+    
+        `python manage.py effect -c create -t config`
     
-    - in app folder, provide app name  
+    - in app folder 'api', provide app name with -n flag  
     
-    `python manage.py effect -c create -t config -n api`
+        `python manage.py effect -c create -t config -n api`
     
     - at certain path, provide path
     
-    `python manage.py effect -c create -t config -p /app/package/tests/testapp/api`
+        `python manage.py effect -c create -t config -p /app/package/tests/testapp/api`
 
 - startapp with nested folders
 
     - from config file
 
     `GROUPEFFECT_CONFIG_JSON_FILE_PATH`
 
     `python manage.py effect -c app -t start`
 
 
 **Tasks** 
 
-You can add task classes to the array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs.
+You can add task classes to the GROUPEFFECT_MANAGEMENT_TASKS array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs. You have to set the command and tasks functions in your `TaskClass`.
 
 Example: 
 
     settings.py:
 
     `GROUPEFFECT_MANAGEMENT_TASKS = ['app.module.script.class_name_1', app.module.script.task_class_2]`
```

### Comparing `groupeffect-0.2.2/README.md` & `groupeffect-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,19 +19,14 @@
 
     INSTALLED_APPS = [ 
         ... 
         groupeffect,
         ...
     ]
 
-`python manage.py makemigrations` -> add Namespace model 
-
-`python manage.py migrate` -> migrates Namespace model 
-
-
 ## Requirements
 
 - https://github.com/django/django
 
 - https://www.django-rest-framework.org/
 
 ## Params in settings.py
@@ -49,35 +44,39 @@
 `python manage.py effect -d`
 
 - help and usage
 
 `python manage.py effect -h`
 
 - create config file
+
+    - in BASE_DIR folder  
+    
+        `python manage.py effect -c create -t config`
     
-    - in app folder, provide app name  
+    - in app folder 'api', provide app name with -n flag  
     
-    `python manage.py effect -c create -t config -n api`
+        `python manage.py effect -c create -t config -n api`
     
     - at certain path, provide path
     
-    `python manage.py effect -c create -t config -p /app/package/tests/testapp/api`
+        `python manage.py effect -c create -t config -p /app/package/tests/testapp/api`
 
 - startapp with nested folders
 
     - from config file
 
     `GROUPEFFECT_CONFIG_JSON_FILE_PATH`
 
     `python manage.py effect -c app -t start`
 
 
 **Tasks** 
 
-You can add task classes to the array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs.
+You can add task classes to the GROUPEFFECT_MANAGEMENT_TASKS array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs. You have to set the command and tasks functions in your `TaskClass`.
 
 Example: 
 
     settings.py:
 
     `GROUPEFFECT_MANAGEMENT_TASKS = ['app.module.script.class_name_1', app.module.script.task_class_2]`
```

### Comparing `groupeffect-0.2.2/groupeffect/management/commands/effect.py` & `groupeffect-0.2.3/groupeffect/management/commands/effect.py`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.2/groupeffect/management/tasks/default.py` & `groupeffect-0.2.3/groupeffect/management/tasks/default.py`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.2/groupeffect/templates/groupeffect/web/api.html` & `groupeffect-0.2.3/groupeffect/templates/groupeffect/web/api.html`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.2/groupeffect.egg-info/PKG-INFO` & `groupeffect-0.2.3/groupeffect.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: groupeffect
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Django app for fast api development.
 Home-page: https://github.com/Groupeffect/groupeffect-pypi
 Author: Amir Yousefi
 Author-email: groupeffect.public@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -40,19 +40,14 @@
 
     INSTALLED_APPS = [ 
         ... 
         groupeffect,
         ...
     ]
 
-`python manage.py makemigrations` -> add Namespace model 
-
-`python manage.py migrate` -> migrates Namespace model 
-
-
 ## Requirements
 
 - https://github.com/django/django
 
 - https://www.django-rest-framework.org/
 
 ## Params in settings.py
@@ -70,35 +65,39 @@
 `python manage.py effect -d`
 
 - help and usage
 
 `python manage.py effect -h`
 
 - create config file
+
+    - in BASE_DIR folder  
+    
+        `python manage.py effect -c create -t config`
     
-    - in app folder, provide app name  
+    - in app folder 'api', provide app name with -n flag  
     
-    `python manage.py effect -c create -t config -n api`
+        `python manage.py effect -c create -t config -n api`
     
     - at certain path, provide path
     
-    `python manage.py effect -c create -t config -p /app/package/tests/testapp/api`
+        `python manage.py effect -c create -t config -p /app/package/tests/testapp/api`
 
 - startapp with nested folders
 
     - from config file
 
     `GROUPEFFECT_CONFIG_JSON_FILE_PATH`
 
     `python manage.py effect -c app -t start`
 
 
 **Tasks** 
 
-You can add task classes to the array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs.
+You can add task classes to the GROUPEFFECT_MANAGEMENT_TASKS array. They will be called by the `effect` command and the `configuration` and `options` will be passed to the `__init__` function as `**context`. You can also find `Configurator` and `Command` classes in the `management.commands.effect` module. They will handle cli inputs, json file upload and task classes. Feel free to fit them to your needs. You have to set the command and tasks functions in your `TaskClass`.
 
 Example: 
 
     settings.py:
 
     `GROUPEFFECT_MANAGEMENT_TASKS = ['app.module.script.class_name_1', app.module.script.task_class_2]`
```

### Comparing `groupeffect-0.2.2/groupeffect.egg-info/SOURCES.txt` & `groupeffect-0.2.3/groupeffect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `groupeffect-0.2.2/setup.cfg` & `groupeffect-0.2.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = groupeffect
-version = 0.2.2
+version = 0.2.3
 description = A Django app for fast api development.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Groupeffect/groupeffect-pypi
 author = Amir Yousefi
 author_email = groupeffect.public@gmail.com
 license = MIT
```

