# Comparing `tmp/cq23-2.0.1.tar.gz` & `tmp/cq23-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cq23-2.0.1.tar", last modified: Mon Jun 19 03:33:54 2023, max compression
+gzip compressed data, was "cq23-2.1.0.tar", last modified: Tue Jun 20 12:04:40 2023, max compression
```

## Comparing `cq23-2.0.1.tar` & `cq23-2.1.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 03:33:54.200623 cq23-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-19 03:33:46.000000 cq23-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-19 03:33:46.000000 cq23-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-19 03:33:54.200623 cq23-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.196623 cq23-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.196623 cq23-2.0.1/src/cq23/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/admin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/admin/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/admin/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/admin/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/build_image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/build_image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/build_image/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/build_image/docker_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/check/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/check/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/cleanup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/cleanup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/cleanup/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/main/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/main/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/main/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/main/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/new_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/new_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/new_client/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/replay/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/replay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/replay/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/run_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/run_game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/run_game/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/run_game/docker_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/run_game/gcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/web_server/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/web_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/web_server/files/
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/web_server/files/loading_screen.html
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/web_server/flask_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23/zip/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/zip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-19 03:33:46.000000 cq23-2.0.1/src/cq23/zip/command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 03:33:54.200623 cq23-2.0.1/src/cq23.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-19 03:33:54.000000 cq23-2.0.1/src/cq23.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-19 03:33:54.000000 cq23-2.0.1/src/cq23.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 03:33:54.000000 cq23-2.0.1/src/cq23.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-19 03:33:54.000000 cq23-2.0.1/src/cq23.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-19 03:33:54.000000 cq23-2.0.1/src/cq23.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-19 03:33:54.000000 cq23-2.0.1/src/cq23.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.051012 cq23-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-20 12:04:40.051012 cq23-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-20 12:04:32.000000 cq23-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-20 12:04:32.000000 cq23-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-20 12:04:40.051012 cq23-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.039012 cq23-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.039012 cq23-2.1.0/src/cq23/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/admin/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23/build_image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/build_image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/build_image/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/build_image/docker_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23/check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/check/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/cleanup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/cleanup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/cleanup/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/main/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/main/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/main/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/main/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/new_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/new_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/new_client/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/replay/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/replay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/replay/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/run_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/docker_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/run_game/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/web_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/web_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.047012 cq23-2.1.0/src/cq23/web_server/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/web_server/files/loading_screen.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/web_server/flask_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.051012 cq23-2.1.0/src/cq23/zip/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/zip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-20 12:04:32.000000 cq23-2.1.0/src/cq23/zip/command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 12:04:40.043012 cq23-2.1.0/src/cq23.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-20 12:04:40.000000 cq23-2.1.0/src/cq23.egg-info/top_level.txt
```

### Comparing `cq23-2.0.1/PKG-INFO` & `cq23-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.0.1
+Version: 2.1.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.0.1/setup.cfg` & `cq23-2.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cq23
-version = 2.0.1
+version = 2.1.0
 author = CodeQuest
 author_email = info@codequest.club
 description = CLI Tools for CodeQuest 23
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CALED-Team/cq23-cli-utilities
 project_urls =
```

### Comparing `cq23-2.0.1/src/cq23/admin/aws.py` & `cq23-2.1.0/src/cq23/admin/aws.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/admin/builder.py` & `cq23-2.1.0/src/cq23/admin/builder.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/admin/worker.py` & `cq23-2.1.0/src/cq23/admin/worker.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/build_image/command.py` & `cq23-2.1.0/src/cq23/build_image/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/build_image/docker_tools.py` & `cq23-2.1.0/src/cq23/build_image/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/check/command.py` & `cq23-2.1.0/src/cq23/check/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/cleanup/command.py` & `cq23-2.1.0/src/cq23/cleanup/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/main/command.py` & `cq23-2.1.0/src/cq23/main/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/main/utils.py` & `cq23-2.1.0/src/cq23/main/utils.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/new_client/command.py` & `cq23-2.1.0/src/cq23/new_client/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         return
 
     language_map = {
         "raw": "https://github.com/CALED-Team/codequest23-raw-submission.git",
         "python": "https://github.com/CALED-Team/codequest23-python-submission.git",
         "cpp": "https://github.com/CALED-Team/codequest23-cpp-submission.git",
         "java": "https://github.com/CALED-Team/codequest23-java-submission.git",
+        "go": "https://github.com/CALED-Team/codequest23-go-submission.git",
     }
     language = args[0]
 
     if language not in language_map.keys():
         return print(
             "Invalid language selected for the new bot. Language should be one of:",
             "[" + " - ".join(language_map.keys()) + "]",
```

### Comparing `cq23-2.0.1/src/cq23/replay/command.py` & `cq23-2.1.0/src/cq23/replay/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/run_game/command.py` & `cq23-2.1.0/src/cq23/run_game/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/run_game/docker_tools.py` & `cq23-2.1.0/src/cq23/run_game/docker_tools.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/run_game/gcs.py` & `cq23-2.1.0/src/cq23/run_game/gcs.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/web_server/files/loading_screen.html` & `cq23-2.1.0/src/cq23/web_server/files/loading_screen.html`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/web_server/flask_api.py` & `cq23-2.1.0/src/cq23/web_server/flask_api.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23/zip/command.py` & `cq23-2.1.0/src/cq23/zip/command.py`

 * *Files identical despite different names*

### Comparing `cq23-2.0.1/src/cq23.egg-info/PKG-INFO` & `cq23-2.1.0/src/cq23.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cq23
-Version: 2.0.1
+Version: 2.1.0
 Summary: CLI Tools for CodeQuest 23
 Home-page: https://github.com/CALED-Team/cq23-cli-utilities
 Author: CodeQuest
 Author-email: info@codequest.club
 Project-URL: Bug Tracker, https://github.com/CALED-Team/cq23-cli-utilities/-/issues
 Project-URL: repository, https://github.com/CALED-Team/cq23-cli-utilities
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cq23-2.0.1/src/cq23.egg-info/SOURCES.txt` & `cq23-2.1.0/src/cq23.egg-info/SOURCES.txt`

 * *Files identical despite different names*

