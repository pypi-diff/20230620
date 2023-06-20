# Comparing `tmp/whiffle_client-0.1.0.tar.gz` & `tmp/whiffle_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whiffle_client-0.1.0.tar", last modified: Tue Jun 20 09:35:52 2023, max compression
+gzip compressed data, was "/app/dist/.tmp-pbrda6_o/whiffle_client-0.1.1.tar", last modified: Tue Jun 20 09:50:51 2023, max compression
```

## Comparing `whiffle_client-0.1.0.tar` & `whiffle_client-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:35:52.983578 whiffle_client-0.1.0/
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-19 14:25:24.000000 whiffle_client-0.1.0/LICENCE.txt
--rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-20 09:35:52.983578 whiffle_client-0.1.0/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      784 2023-06-20 07:37:38.000000 whiffle_client-0.1.0/README.md
--rw-rw-r--   0 root         (0) root         (0)      749 2023-06-20 07:58:24.000000 whiffle_client-0.1.0/USER_README.md
--rw-rw-r--   0 root         (0) root         (0)      681 2023-06-20 07:37:14.000000 whiffle_client-0.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 09:35:52.983578 whiffle_client-0.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:35:52.979578 whiffle_client-0.1.0/tests/
--rw-rw-r--   0 root         (0) root         (0)     3259 2023-06-16 12:41:36.000000 whiffle_client-0.1.0/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:35:52.983578 whiffle_client-0.1.0/whiffle_client/
--rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.0/whiffle_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.0/whiffle_client/client.py
--rw-rw-r--   0 root         (0) root         (0)     1855 2023-06-19 14:25:24.000000 whiffle_client-0.1.0/whiffle_client/entrypoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:35:52.983578 whiffle_client-0.1.0/whiffle_client/resources/
--rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.0/whiffle_client/resources/example_generic_params.json
--rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.0/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:35:52.983578 whiffle_client-0.1.0/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-20 09:35:52.000000 whiffle_client-0.1.0/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-20 09:35:52.000000 whiffle_client-0.1.0/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:35:52.000000 whiffle_client-0.1.0/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 09:35:52.000000 whiffle_client-0.1.0/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 09:35:52.000000 whiffle_client-0.1.0/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 09:35:52.000000 whiffle_client-0.1.0/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/LICENCE.txt
+-rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      784 2023-06-20 07:37:38.000000 whiffle_client-0.1.1/README.md
+-rw-rw-r--   0 root         (0) root         (0)      749 2023-06-20 07:58:24.000000 whiffle_client-0.1.1/USER_README.md
+-rw-rw-r--   0 root         (0) root         (0)      681 2023-06-20 09:50:30.000000 whiffle_client-0.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/tests/
+-rw-rw-r--   0 root         (0) root         (0)     3259 2023-06-16 12:41:36.000000 whiffle_client-0.1.1/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client/
+-rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1855 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/entrypoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client/resources/
+-rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/resources/example_generic_params.json
+-rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `whiffle_client-0.1.0/LICENCE.txt` & `whiffle_client-0.1.1/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/PKG-INFO` & `whiffle_client-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle_client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

### Comparing `whiffle_client-0.1.0/README.md` & `whiffle_client-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/USER_README.md` & `whiffle_client-0.1.1/USER_README.md`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/pyproject.toml` & `whiffle_client-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "whiffle_client"
-version = "0.1.0"
+version = "0.1.1"
 description = "Python based web client to interact with Whiffle services"
 readme = "USER_README.md"
 
 license = {file = "LICENSE.txt"}
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 dependencies = [
-    "click~=8.1.3",
+    "click~=8.0.4",
     "PyYAML~=6.0",
-    "requests~=2.31.0",
+    "requests~=2.27.1",
 ]
 # dynamic = ["version"]
 [tool.setuptools]
 packages = ["whiffle_client"]
 
 [project.scripts]
 whiffle = "whiffle_client.entrypoints:whiffle"
```

### Comparing `whiffle_client-0.1.0/tests/test_client.py` & `whiffle_client-0.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/whiffle_client/client.py` & `whiffle_client-0.1.1/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/whiffle_client/entrypoints.py` & `whiffle_client-0.1.1/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.1.1/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.0/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.1.1/whiffle_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whiffle-client
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
```

