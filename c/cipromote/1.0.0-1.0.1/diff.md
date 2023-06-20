# Comparing `tmp/cipromote-1.0.0.tar.gz` & `tmp/cipromote-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cipromote-1.0.0.tar", max compression
+gzip compressed data, was "cipromote-1.0.1.tar", max compression
```

## Comparing `cipromote-1.0.0.tar` & `cipromote-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       65 2023-03-02 21:37:34.089109 cipromote-1.0.0/README.md
--rw-r--r--   0        0        0      506 2023-03-02 21:38:51.457776 cipromote-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.0.0/src/cipromote/__init__.py
--rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.0.0/src/cipromote/ci-cli.py
--rw-r--r--   0        0        0     7416 2023-03-02 21:27:10.506729 cipromote-1.0.0/src/cipromote/cli.py
--rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.0.0/src/cipromote/constants.py
--rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.0.0/src/cipromote/instances.py
--rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.0.0/src/cipromote/label_versions.py
--rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.0.0/src/cipromote/labels.py
--rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.0.0/src/cipromote/login.py
--rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.0.0/src/cipromote/loginInput.py
--rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.0.0/src/cipromote/projects.py
--rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.0.0/src/cipromote/queries.py
--rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.0.0/src/cipromote/versioned_items.py
--rw-r--r--   0        0        0      695 1970-01-01 00:00:00.000000 cipromote-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       68 2023-03-13 15:43:49.230739 cipromote-1.0.1/README.md
+-rw-r--r--   0        0        0      548 2023-06-20 21:26:30.105404 cipromote-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-01 21:23:03.887994 cipromote-1.0.1/src/cipromote/__init__.py
+-rw-r--r--   0        0        0    25204 2023-03-01 22:01:52.712793 cipromote-1.0.1/src/cipromote/ci-cli.py
+-rw-r--r--   0        0        0     7585 2023-06-20 20:25:28.071576 cipromote-1.0.1/src/cipromote/cli.py
+-rw-r--r--   0        0        0      114 2023-03-01 22:01:52.717793 cipromote-1.0.1/src/cipromote/constants.py
+-rw-r--r--   0        0        0     1680 2023-03-02 20:06:52.453096 cipromote-1.0.1/src/cipromote/instances.py
+-rw-r--r--   0        0        0     5708 2023-03-02 21:27:59.317150 cipromote-1.0.1/src/cipromote/label_versions.py
+-rw-r--r--   0        0        0     3889 2023-03-02 20:55:55.574572 cipromote-1.0.1/src/cipromote/labels.py
+-rw-r--r--   0        0        0      387 2023-03-02 15:58:17.336622 cipromote-1.0.1/src/cipromote/login.py
+-rw-r--r--   0        0        0     3510 2023-03-02 15:12:46.158566 cipromote-1.0.1/src/cipromote/loginInput.py
+-rw-r--r--   0        0        0     2981 2023-03-02 19:49:52.016215 cipromote-1.0.1/src/cipromote/projects.py
+-rw-r--r--   0        0        0    11691 2023-03-01 22:01:52.726793 cipromote-1.0.1/src/cipromote/queries.py
+-rw-r--r--   0        0        0     2158 2023-03-01 22:01:52.728793 cipromote-1.0.1/src/cipromote/versioned_items.py
+-rw-r--r--   0        0        0      698 1970-01-01 00:00:00.000000 cipromote-1.0.1/PKG-INFO
```

### Comparing `cipromote-1.0.0/src/cipromote/ci-cli.py` & `cipromote-1.0.1/src/cipromote/ci-cli.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/cli.py` & `cipromote-1.0.1/src/cipromote/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,16 +57,19 @@
 
 @main.command("get-instances", short_help="Get a list of instances")
 def get_instances():
     """Gets a list of instances"""
     server_url = os.getenv("MOTIOCI_SERVERURL")
     constants.CI_URL = server_url
     constants.GRAPH_URL = constants.CI_URL + constants.GRAPH_URL
+    print('Sending query to the following url')
+    print(constants.GRAPH_URL)
     instance_object = instances.get_instances_default()
     pprint(instance_object)
+    #print(f"Instance 0 has these namespaces {instance_object[0]['node']['namespaces']}")
     return instance_object
 
 
 @main.command("get-labels", short_help="Get a list of available labels")
 def get_labels():
     """Gets a lit of available labels"""
     server_url = os.getenv("MOTIOCI_SERVERURL")
```

### Comparing `cipromote-1.0.0/src/cipromote/instances.py` & `cipromote-1.0.1/src/cipromote/instances.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/label_versions.py` & `cipromote-1.0.1/src/cipromote/label_versions.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/labels.py` & `cipromote-1.0.1/src/cipromote/labels.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/loginInput.py` & `cipromote-1.0.1/src/cipromote/loginInput.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/projects.py` & `cipromote-1.0.1/src/cipromote/projects.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/queries.py` & `cipromote-1.0.1/src/cipromote/queries.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/src/cipromote/versioned_items.py` & `cipromote-1.0.1/src/cipromote/versioned_items.py`

 * *Files identical despite different names*

### Comparing `cipromote-1.0.0/PKG-INFO` & `cipromote-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cipromote
-Version: 1.0.0
+Version: 1.0.1
 Summary: Promote MotionCI Labels
 Author: Michael MacKenna
 Author-email: mmackenna@ufginsurance.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -14,10 +14,11 @@
 Requires-Dist: gql (>=3.4.0,<4.0.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: termcolor (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # CI Promote
 
-CIPromote is a CLI for promoting MotionCI labels.
+## CIPromote is a CLI for promoting MotioCI labels.
+
```

