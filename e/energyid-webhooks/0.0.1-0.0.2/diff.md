# Comparing `tmp/energyid-webhooks-0.0.1.tar.gz` & `tmp/energyid-webhooks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energyid-webhooks-0.0.1.tar", last modified: Fri Jun 16 13:25:10 2023, max compression
+gzip compressed data, was "energyid-webhooks-0.0.2.tar", last modified: Tue Jun 20 11:49:10 2023, max compression
```

## Comparing `energyid-webhooks-0.0.1.tar` & `energyid-webhooks-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-16 13:25:10.719078 energyid-webhooks-0.0.1/
--rw-r--r--   0 Jan        (504) staff       (20)     1074 2023-06-16 12:54:48.000000 energyid-webhooks-0.0.1/LICENSE
--rw-r--r--   0 Jan        (504) staff       (20)     2127 2023-06-16 13:25:10.719196 energyid-webhooks-0.0.1/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)     1570 2023-06-16 13:24:11.000000 energyid-webhooks-0.0.1/README.md
--rw-r--r--   0 Jan        (504) staff       (20)      103 2023-06-16 12:57:53.000000 energyid-webhooks-0.0.1/pyproject.toml
--rw-r--r--   0 Jan        (504) staff       (20)      720 2023-06-16 13:25:10.719632 energyid-webhooks-0.0.1/setup.cfg
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-16 13:25:10.716475 energyid-webhooks-0.0.1/src/
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-16 13:25:10.717950 energyid-webhooks-0.0.1/src/energyid_webhooks/
--rw-r--r--   0 Jan        (504) staff       (20)       75 2023-06-16 13:07:18.000000 energyid-webhooks-0.0.1/src/energyid_webhooks/__init__.py
--rw-r--r--   0 Jan        (504) staff       (20)     1214 2023-06-16 13:02:11.000000 energyid-webhooks-0.0.1/src/energyid_webhooks/client.py
-drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-16 13:25:10.718957 energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/
--rw-r--r--   0 Jan        (504) staff       (20)     2127 2023-06-16 13:25:10.000000 energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/PKG-INFO
--rw-r--r--   0 Jan        (504) staff       (20)      332 2023-06-16 13:25:10.000000 energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/SOURCES.txt
--rw-r--r--   0 Jan        (504) staff       (20)        1 2023-06-16 13:25:10.000000 energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/dependency_links.txt
--rw-r--r--   0 Jan        (504) staff       (20)       17 2023-06-16 13:25:10.000000 energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/requires.txt
--rw-r--r--   0 Jan        (504) staff       (20)       18 2023-06-16 13:25:10.000000 energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/top_level.txt
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-20 11:49:10.370178 energyid-webhooks-0.0.2/
+-rw-r--r--   0 Jan        (504) staff       (20)     1074 2023-06-16 12:54:48.000000 energyid-webhooks-0.0.2/LICENSE
+-rw-r--r--   0 Jan        (504) staff       (20)     2131 2023-06-20 11:49:10.370308 energyid-webhooks-0.0.2/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)     1574 2023-06-16 13:26:52.000000 energyid-webhooks-0.0.2/README.md
+-rw-r--r--   0 Jan        (504) staff       (20)      103 2023-06-16 12:57:53.000000 energyid-webhooks-0.0.2/pyproject.toml
+-rw-r--r--   0 Jan        (504) staff       (20)      720 2023-06-20 11:49:10.370734 energyid-webhooks-0.0.2/setup.cfg
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-20 11:49:10.367106 energyid-webhooks-0.0.2/src/
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-20 11:49:10.368895 energyid-webhooks-0.0.2/src/energyid_webhooks/
+-rw-r--r--   0 Jan        (504) staff       (20)       75 2023-06-16 13:07:18.000000 energyid-webhooks-0.0.2/src/energyid_webhooks/__init__.py
+-rw-r--r--   0 Jan        (504) staff       (20)     2193 2023-06-20 11:45:56.000000 energyid-webhooks-0.0.2/src/energyid_webhooks/client.py
+-rw-r--r--   0 Jan        (504) staff       (20)      807 2023-06-20 11:45:07.000000 energyid-webhooks-0.0.2/src/energyid_webhooks/metercatalog.py
+drwxr-xr-x   0 Jan        (504) staff       (20)        0 2023-06-20 11:49:10.369936 energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/
+-rw-r--r--   0 Jan        (504) staff       (20)     2131 2023-06-20 11:49:10.000000 energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/PKG-INFO
+-rw-r--r--   0 Jan        (504) staff       (20)      370 2023-06-20 11:49:10.000000 energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/SOURCES.txt
+-rw-r--r--   0 Jan        (504) staff       (20)        1 2023-06-20 11:49:10.000000 energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/dependency_links.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       17 2023-06-20 11:49:10.000000 energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/requires.txt
+-rw-r--r--   0 Jan        (504) staff       (20)       18 2023-06-20 11:49:10.000000 energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/top_level.txt
```

### Comparing `energyid-webhooks-0.0.1/LICENSE` & `energyid-webhooks-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `energyid-webhooks-0.0.1/PKG-INFO` & `energyid-webhooks-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyid-webhooks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Light weight python package to interface with EnergyID webhooks
 Home-page: https://api.energyid.eu/docs.html#webhook
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
 Project-URL: Bug Tracker, https://github.com/EnergieID/energyid-webhooks-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -81,15 +81,15 @@
     await client.post(data)
 
 asyncio.run(main())
 ```
 
 ## Demo Notebook
 
-See [demo.ipynb](demo.ipynb) for a demo notebook.
+See [demo.ipynb](src/demo.ipynb) for a demo notebook.
 
 ## Development
 
 ### Setup
 
 ```bash
 python3 -m venv venv
```

### Comparing `energyid-webhooks-0.0.1/README.md` & `energyid-webhooks-0.0.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
     await client.post(data)
 
 asyncio.run(main())
 ```
 
 ## Demo Notebook
 
-See [demo.ipynb](demo.ipynb) for a demo notebook.
+See [demo.ipynb](src/demo.ipynb) for a demo notebook.
 
 ## Development
 
 ### Setup
 
 ```bash
 python3 -m venv venv
```

### Comparing `energyid-webhooks-0.0.1/setup.cfg` & `energyid-webhooks-0.0.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = energyid-webhooks
-version = 0.0.1
+version = 0.0.2
 author = Jan Pecinovsky
 author_email = jan@energieid.be
 description = Light weight python package to interface with EnergyID webhooks
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://api.energyid.eu/docs.html#webhook
 project_urls =
```

### Comparing `energyid-webhooks-0.0.1/src/energyid_webhooks.egg-info/PKG-INFO` & `energyid-webhooks-0.0.2/src/energyid_webhooks.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: energyid-webhooks
-Version: 0.0.1
+Version: 0.0.2
 Summary: Light weight python package to interface with EnergyID webhooks
 Home-page: https://api.energyid.eu/docs.html#webhook
 Author: Jan Pecinovsky
 Author-email: jan@energieid.be
 Project-URL: Bug Tracker, https://github.com/EnergieID/energyid-webhooks-py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -81,15 +81,15 @@
     await client.post(data)
 
 asyncio.run(main())
 ```
 
 ## Demo Notebook
 
-See [demo.ipynb](demo.ipynb) for a demo notebook.
+See [demo.ipynb](src/demo.ipynb) for a demo notebook.
 
 ## Development
 
 ### Setup
 
 ```bash
 python3 -m venv venv
```

