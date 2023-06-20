# Comparing `tmp/whiffle_client-0.1.1.tar.gz` & `tmp/whiffle_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/app/dist/.tmp-pbrda6_o/whiffle_client-0.1.1.tar", last modified: Tue Jun 20 09:50:51 2023, max compression
+gzip compressed data, was "/app/dist/.tmp-h4b32k12/whiffle_client-0.1.2.tar", last modified: Tue Jun 20 10:17:12 2023, max compression
```

## Comparing `whiffle_client-0.1.1.tar` & `whiffle_client-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/
--rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/LICENCE.txt
--rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      784 2023-06-20 07:37:38.000000 whiffle_client-0.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      749 2023-06-20 07:58:24.000000 whiffle_client-0.1.1/USER_README.md
--rw-rw-r--   0 root         (0) root         (0)      681 2023-06-20 09:50:30.000000 whiffle_client-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/tests/
--rw-rw-r--   0 root         (0) root         (0)     3259 2023-06-16 12:41:36.000000 whiffle_client-0.1.1/tests/test_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client/
--rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/client.py
--rw-rw-r--   0 root         (0) root         (0)     1855 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/entrypoints.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client/resources/
--rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/resources/example_generic_params.json
--rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.1/whiffle_client/resources/whiffle_config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1088 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      494 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 09:50:51.000000 whiffle_client-0.1.1/whiffle_client.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/
+-rw-rw-r--   0 root         (0) root         (0)     1069 2023-06-20 10:03:07.000000 whiffle_client-0.1.2/LICENCE.txt
+-rw-rw-r--   0 root         (0) root         (0)      121 2023-06-16 16:28:25.000000 whiffle_client-0.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      780 2023-06-20 10:06:11.000000 whiffle_client-0.1.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      740 2023-06-20 10:16:02.000000 whiffle_client-0.1.2/USER_README.md
+-rw-rw-r--   0 root         (0) root         (0)      681 2023-06-20 10:16:07.000000 whiffle_client-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/tests/
+-rw-rw-r--   0 root         (0) root         (0)     3259 2023-06-16 12:41:36.000000 whiffle_client-0.1.2/tests/test_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client/
+-rw-rw-r--   0 root         (0) root         (0)      120 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7145 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/client.py
+-rw-rw-r--   0 root         (0) root         (0)     1855 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/entrypoints.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client/resources/
+-rw-rw-r--   0 root         (0) root         (0)     2624 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/resources/example_generic_params.json
+-rw-rw-r--   0 root         (0) root         (0)       60 2023-06-19 14:25:24.000000 whiffle_client-0.1.2/whiffle_client/resources/whiffle_config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1079 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       63 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-06-20 10:17:12.000000 whiffle_client-0.1.2/whiffle_client.egg-info/top_level.txt
```

### Comparing `whiffle_client-0.1.1/LICENCE.txt` & `whiffle_client-0.1.2/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.1/PKG-INFO` & `whiffle_client-0.1.2/whiffle_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: whiffle_client
-Version: 0.1.1
+Name: whiffle-client
+Version: 0.1.2
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Whiffle client
 
-This client allows running wind resource assessment (WRA) with Whiffle's GPU-resident, high-fidelity LES model <https://whiffle.nl/>. 
+This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
 `whiffle config-edit user.token <your_token>`
 
 You can create a new task by executing,
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
```

### Comparing `whiffle_client-0.1.1/README.md` & `whiffle_client-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,9 +30,9 @@
 `docker build --rm . -t whiffle-client && docker run --rm -it whiffle-client bash`
 
 ## Deploying
 
 `bash
 docker build --rm . -t whiffle-client && docker run --rm -it whiffle-client bash
 python -m build
-python3 -m twine upload --repository testpypi dist/*
+python3 -m twine upload --repository pypi dist/*
 `
```

### Comparing `whiffle_client-0.1.1/USER_README.md` & `whiffle_client-0.1.2/USER_README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Whiffle client
 
-This client allows running wind resource assessment (WRA) with Whiffle's GPU-resident, high-fidelity LES model <https://whiffle.nl/>. 
+This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
 `whiffle config-edit user.token <your_token>`
 
 You can create a new task by executing,
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
```

### Comparing `whiffle_client-0.1.1/pyproject.toml` & `whiffle_client-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "whiffle_client"
-version = "0.1.1"
+version = "0.1.2"
 description = "Python based web client to interact with Whiffle services"
 readme = "USER_README.md"
 
 license = {file = "LICENSE.txt"}
 
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `whiffle_client-0.1.1/tests/test_client.py` & `whiffle_client-0.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.1/whiffle_client/client.py` & `whiffle_client-0.1.2/whiffle_client/client.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.1/whiffle_client/entrypoints.py` & `whiffle_client-0.1.2/whiffle_client/entrypoints.py`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.1/whiffle_client/resources/example_generic_params.json` & `whiffle_client-0.1.2/whiffle_client/resources/example_generic_params.json`

 * *Files identical despite different names*

### Comparing `whiffle_client-0.1.1/whiffle_client.egg-info/PKG-INFO` & `whiffle_client-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
-Name: whiffle-client
-Version: 0.1.1
+Name: whiffle_client
+Version: 0.1.2
 Summary: Python based web client to interact with Whiffle services
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENCE.txt
 
 # Whiffle client
 
-This client allows running wind resource assessment (WRA) with Whiffle's GPU-resident, high-fidelity LES model <https://whiffle.nl/>. 
+This client allows running atmospheric large-eddy simulations (LES) with Whiffle's GPU-resident model <https://whiffle.nl/>. 
 The client requires an access token, which you can configure with the command line interface by executing,
 
 `whiffle config-edit user.token <your_token>`
 
 You can create a new task by executing,
 
 `whiffle run <path_to_the_task_specification.[json|yaml]>`
```

