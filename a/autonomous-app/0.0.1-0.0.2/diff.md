# Comparing `tmp/autonomous-app-0.0.1.tar.gz` & `tmp/autonomous-app-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomous-app-0.0.1.tar", last modified: Tue Jun 20 21:05:49 2023, max compression
+gzip compressed data, was "autonomous-app-0.0.2.tar", last modified: Tue Jun 20 21:26:10 2023, max compression
```

## Comparing `autonomous-app-0.0.1.tar` & `autonomous-app-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2161 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.687827 autonomous-app-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.687827 autonomous-app-0.0.1/src/autonomous/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.687827 autonomous-app-0.0.1/src/autonomous/apis/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/src/autonomous/apis/version_control/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/version_control/GHCallbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/version_control/GHOrganization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/version_control/GHRepo.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/version_control/GHVersionControl.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/apis/version_control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/assets.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/src/autonomous/db/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/db/autodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/db/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/db/table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/src/autonomous/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/model/automodel.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/model/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/src/autonomous/storage/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/storage/basestorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/storage/cloudinarystorage.py
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/storage/localstorage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 21:05:38.000000 autonomous-app-0.0.1/src/autonomous/storage/s3storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:05:49.691827 autonomous-app-0.0.1/src/autonomous_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-06-20 21:05:49.000000 autonomous-app-0.0.1/src/autonomous_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-20 21:05:49.000000 autonomous-app-0.0.1/src/autonomous_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:05:49.000000 autonomous-app-0.0.1/src/autonomous_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 21:05:49.000000 autonomous-app-0.0.1/src/autonomous_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 21:05:49.000000 autonomous-app-0.0.1/src/autonomous_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 21:05:49.000000 autonomous-app-0.0.1/src/autonomous_app.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.570176 autonomous-app-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.570176 autonomous-app-0.0.2/src/autonomous/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.570176 autonomous-app-0.0.2/src/autonomous/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.570176 autonomous-app-0.0.2/src/autonomous/apis/version_control/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/version_control/GHCallbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/version_control/GHOrganization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/version_control/GHRepo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/version_control/GHVersionControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/apis/version_control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/src/autonomous/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/db/autodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/db/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/db/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/src/autonomous/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/model/automodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/model/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/src/autonomous/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/storage/basestorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/storage/cloudinarystorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/storage/localstorage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-20 21:25:51.000000 autonomous-app-0.0.2/src/autonomous/storage/s3storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 21:26:10.574176 autonomous-app-0.0.2/src/autonomous_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-20 21:26:10.000000 autonomous-app-0.0.2/src/autonomous_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-20 21:26:10.000000 autonomous-app-0.0.2/src/autonomous_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 21:26:10.000000 autonomous-app-0.0.2/src/autonomous_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-20 21:26:10.000000 autonomous-app-0.0.2/src/autonomous_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-20 21:26:10.000000 autonomous-app-0.0.2/src/autonomous_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-20 21:26:10.000000 autonomous-app-0.0.2/src/autonomous_app.egg-info/top_level.txt
```

### Comparing `autonomous-app-0.0.1/LICENSE` & `autonomous-app-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/PKG-INFO` & `autonomous-app-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.0.1
+Version: 0.0.2
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,40 +30,32 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autonomous
 
-:warning::warning::warning: WiP :warning::warning::warning:
+:warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
 A local, containerized, service based application library built on top of Flask. 
 The goal is to make it easy to create self-contained Python applications with minimal dependencies and built in libraries for many different kinds of tasks.
 
-- **pypi**: https://test.pypi.org/project/autonomous
-- **github**: https://github.com/Sallenmoore/autonomous
+- **[pypi](https://test.pypi.org/project/autonomous)**
+- **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
 - All services are localized to a virtual intranet
 - Built-in Local NoSQL database and Model API
 - Cloud file storage with Cloudinary or S3
 - Auto-Generated Documentation Pages (Coming Soon!!!)
 
-### Container Apps
-
-Autonomous App has minimally 1 container components:
-
-- **app**
-  - access documentation on port:TBD
-  - App
-
 ## Dependencies
 
 - **Languages**
   - [Python 3.10](/Dev/language/python)
 - **Frameworks**
   - [Flask](https://flask.palletsprojects.com/en/2.1.x/)
 - **Containers**
@@ -83,16 +75,14 @@
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
   - [highlight.js](https://highlightjs.org/)
 
 ---
 
 ## Developer Notes
 
-## {.tabset}
-
 ### TODO
 
 - Auto generate API documentation
 - Setup/fix template app generator
 - Add type hints
 - Switch to less verbose html preprocessor
 - Add more database options
@@ -113,10 +103,8 @@
 ```sh
 make tests
 ```
 
 ### package
 
 1. Update version in `/src/autonomous/__init__.py`
-2. ```sh
-   make package
-   ```
+2. `make package`
```

### Comparing `autonomous-app-0.0.1/README.md` & `autonomous-app-0.0.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,27 @@
 # Autonomous
 
-:warning::warning::warning: WiP :warning::warning::warning:
+:warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
 A local, containerized, service based application library built on top of Flask. 
 The goal is to make it easy to create self-contained Python applications with minimal dependencies and built in libraries for many different kinds of tasks.
 
-- **pypi**: https://test.pypi.org/project/autonomous
-- **github**: https://github.com/Sallenmoore/autonomous
+- **[pypi](https://test.pypi.org/project/autonomous)**
+- **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
 - All services are localized to a virtual intranet
 - Built-in Local NoSQL database and Model API
 - Cloud file storage with Cloudinary or S3
 - Auto-Generated Documentation Pages (Coming Soon!!!)
 
-### Container Apps
-
-Autonomous App has minimally 1 container components:
-
-- **app**
-  - access documentation on port:TBD
-  - App
-
 ## Dependencies
 
 - **Languages**
   - [Python 3.10](/Dev/language/python)
 - **Frameworks**
   - [Flask](https://flask.palletsprojects.com/en/2.1.x/)
 - **Containers**
@@ -49,16 +41,14 @@
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
   - [highlight.js](https://highlightjs.org/)
 
 ---
 
 ## Developer Notes
 
-## {.tabset}
-
 ### TODO
 
 - Auto generate API documentation
 - Setup/fix template app generator
 - Add type hints
 - Switch to less verbose html preprocessor
 - Add more database options
@@ -79,10 +69,8 @@
 ```sh
 make tests
 ```
 
 ### package
 
 1. Update version in `/src/autonomous/__init__.py`
-2. ```sh
-   make package
-   ```
+2. `make package`
```

### Comparing `autonomous-app-0.0.1/pyproject.toml` & `autonomous-app-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/apis/openai.py` & `autonomous-app-0.0.2/src/autonomous/apis/openai.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/apis/version_control/GHCallbacks.py` & `autonomous-app-0.0.2/src/autonomous/apis/version_control/GHCallbacks.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/apis/version_control/GHOrganization.py` & `autonomous-app-0.0.2/src/autonomous/apis/version_control/GHOrganization.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/apis/version_control/GHRepo.py` & `autonomous-app-0.0.2/src/autonomous/apis/version_control/GHRepo.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/assets.py` & `autonomous-app-0.0.2/src/autonomous/assets.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/db/autodb.py` & `autonomous-app-0.0.2/src/autonomous/db/autodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,18 @@
 
 class Database:
     def __init__(self, path="."):
         """
         create an interface for your database
         """
         if not path.startswith("/"):
-            path = "/" + path
+            path = f"{pathlib.Path().resolve()}{path}"
         if not path.endswith("/"):
             path = path + "/"
-        self.db_path = (
-            f'{pathlib.Path().resolve()}{path}{os.environ.get("DB_NAME", "tables")}'
-        )
+        self.db_path = f'{path}{os.environ.get("DB_NAME", "tables")}'
         # log(self.db_path)
         os.path.isdir(self.db_path) or os.makedirs(self.db_path)
         self.tables = {}
 
     def get_table(self, table="default"):
         """
         opens the table from the file, which clears any changed data
```

### Comparing `autonomous-app-0.0.1/src/autonomous/db/storage.py` & `autonomous-app-0.0.2/src/autonomous/db/storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/db/table.py` & `autonomous-app-0.0.2/src/autonomous/db/table.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/logger.py` & `autonomous-app-0.0.2/src/autonomous/logger.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/model/automodel.py` & `autonomous-app-0.0.2/src/autonomous/model/automodel.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/model/orm.py` & `autonomous-app-0.0.2/src/autonomous/model/orm.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/storage/cloudinarystorage.py` & `autonomous-app-0.0.2/src/autonomous/storage/cloudinarystorage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous/storage/s3storage.py` & `autonomous-app-0.0.2/src/autonomous/storage/s3storage.py`

 * *Files identical despite different names*

### Comparing `autonomous-app-0.0.1/src/autonomous_app.egg-info/PKG-INFO` & `autonomous-app-0.0.2/src/autonomous_app.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonomous-app
-Version: 0.0.1
+Version: 0.0.2
 Summary: Containerized application framework built on Flask with additional libraries and tools for rapid development of web applications.
 Author-email: Steven A Moore <samoore@binghamton.edu>
 License: MIT License
         
         Copyright (c) [2022] Steven Allen Moore
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,40 +30,32 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Autonomous
 
-:warning::warning::warning: WiP :warning::warning::warning:
+:warning: :warning: :warning: WiP :warning: :warning: :warning:
 
 ![Tests](https://github.com/Sallenmoore/autonomous/actions/workflows/tests.yml/badge.svg)
 
 A local, containerized, service based application library built on top of Flask. 
 The goal is to make it easy to create self-contained Python applications with minimal dependencies and built in libraries for many different kinds of tasks.
 
-- **pypi**: https://test.pypi.org/project/autonomous
-- **github**: https://github.com/Sallenmoore/autonomous
+- **[pypi](https://test.pypi.org/project/autonomous)**
+- **[github](https://github.com/Sallenmoore/autonomous)**
 
 ## Features
 
 - Fully containerized, service based Python application framework
 - All services are localized to a virtual intranet
 - Built-in Local NoSQL database and Model API
 - Cloud file storage with Cloudinary or S3
 - Auto-Generated Documentation Pages (Coming Soon!!!)
 
-### Container Apps
-
-Autonomous App has minimally 1 container components:
-
-- **app**
-  - access documentation on port:TBD
-  - App
-
 ## Dependencies
 
 - **Languages**
   - [Python 3.10](/Dev/language/python)
 - **Frameworks**
   - [Flask](https://flask.palletsprojects.com/en/2.1.x/)
 - **Containers**
@@ -83,16 +75,14 @@
   - [pdoc](https://pdoc.dev/docs/pdoc/doc.html)
   - [highlight.js](https://highlightjs.org/)
 
 ---
 
 ## Developer Notes
 
-## {.tabset}
-
 ### TODO
 
 - Auto generate API documentation
 - Setup/fix template app generator
 - Add type hints
 - Switch to less verbose html preprocessor
 - Add more database options
@@ -113,10 +103,8 @@
 ```sh
 make tests
 ```
 
 ### package
 
 1. Update version in `/src/autonomous/__init__.py`
-2. ```sh
-   make package
-   ```
+2. `make package`
```

### Comparing `autonomous-app-0.0.1/src/autonomous_app.egg-info/SOURCES.txt` & `autonomous-app-0.0.2/src/autonomous_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

