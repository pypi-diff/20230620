# Comparing `tmp/apiron-7.1.0.post2.tar.gz` & `tmp/apiron-7.1.0.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apiron-7.1.0.post2.tar", last modified: Tue Jun 20 13:50:51 2023, max compression
+gzip compressed data, was "apiron-7.1.0.post3.tar", last modified: Tue Jun 20 19:56:58 2023, max compression
```

## Comparing `apiron-7.1.0.post2.tar` & `apiron-7.1.0.post3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.259549 apiron-7.1.0.post2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-20 13:50:51.259549 apiron-7.1.0.post2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-20 13:50:51.259549 apiron-7.1.0.post2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.251549 apiron-7.1.0.post2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.255549 apiron-7.1.0.post2/src/apiron/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.255549 apiron-7.1.0.post2/src/apiron/endpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/endpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/endpoint/endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/endpoint/json.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/endpoint/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/endpoint/stub.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.259549 apiron-7.1.0.post2/src/apiron/service/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/service/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/src/apiron/service/discoverable.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.255549 apiron-7.1.0.post2/src/apiron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-20 13:50:51.000000 apiron-7.1.0.post2/src/apiron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-20 13:50:51.000000 apiron-7.1.0.post2/src/apiron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 13:50:51.000000 apiron-7.1.0.post2/src/apiron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 13:50:51.000000 apiron-7.1.0.post2/src/apiron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 13:50:51.000000 apiron-7.1.0.post2/src/apiron.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.259549 apiron-7.1.0.post2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:51.259549 apiron-7.1.0.post2/tests/service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/tests/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/tests/service/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/tests/service/test_discoverable.py
--rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-06-20 13:50:40.000000 apiron-7.1.0.post2/tests/test_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.151115 apiron-7.1.0.post3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-20 19:56:58.151115 apiron-7.1.0.post3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2473 2023-06-20 19:56:58.151115 apiron-7.1.0.post3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.147115 apiron-7.1.0.post3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.147115 apiron-7.1.0.post3/src/apiron/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.147115 apiron-7.1.0.post3/src/apiron/endpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/endpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7486 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/endpoint/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/endpoint/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/endpoint/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/endpoint/stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.147115 apiron-7.1.0.post3/src/apiron/service/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/service/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/src/apiron/service/discoverable.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.147115 apiron-7.1.0.post3/src/apiron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-06-20 19:56:58.000000 apiron-7.1.0.post3/src/apiron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-06-20 19:56:58.000000 apiron-7.1.0.post3/src/apiron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-20 19:56:58.000000 apiron-7.1.0.post3/src/apiron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-20 19:56:58.000000 apiron-7.1.0.post3/src/apiron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-20 19:56:58.000000 apiron-7.1.0.post3/src/apiron.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.151115 apiron-7.1.0.post3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:58.151115 apiron-7.1.0.post3/tests/service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/tests/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/tests/service/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/tests/service/test_discoverable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12705 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7207 2023-06-20 19:56:49.000000 apiron-7.1.0.post3/tests/test_endpoint.py
```

### Comparing `apiron-7.1.0.post2/LICENSE` & `apiron-7.1.0.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/PKG-INFO` & `apiron-7.1.0.post3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiron
-Version: 7.1.0.post2
+Version: 7.1.0.post3
 Summary: apiron helps you cook a tasty client for RESTful APIs. Just don't wash it with SOAP.
 Home-page: https://github.com/ithaka/apiron
 Author: Ithaka Harbors, Inc.
 Author-email: opensource@ithaka.org
 License: MIT
 Project-URL: Documentation, https://apiron.readthedocs.io
 Project-URL: Source, https://github.com/ithaka/apiron
```

### Comparing `apiron-7.1.0.post2/README.md` & `apiron-7.1.0.post3/README.md`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/setup.cfg` & `apiron-7.1.0.post3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = apiron
-version = 7.1.0-post.2
+version = 7.1.0-post.3
 description = apiron helps you cook a tasty client for RESTful APIs. Just don't wash it with SOAP.
 author = Ithaka Harbors, Inc.
 author_email = opensource@ithaka.org
 url = https://github.com/ithaka/apiron
 license = MIT
 license_files = LICENSE
 long_description = file: README.md
```

### Comparing `apiron-7.1.0.post2/src/apiron/__init__.py` & `apiron-7.1.0.post3/src/apiron/__init__.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/client.py` & `apiron-7.1.0.post3/src/apiron/client.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/endpoint/endpoint.py` & `apiron-7.1.0.post3/src/apiron/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/endpoint/json.py` & `apiron-7.1.0.post3/src/apiron/endpoint/json.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/endpoint/streaming.py` & `apiron-7.1.0.post3/src/apiron/endpoint/streaming.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/endpoint/stub.py` & `apiron-7.1.0.post3/src/apiron/endpoint/stub.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/exceptions.py` & `apiron-7.1.0.post3/src/apiron/exceptions.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/service/base.py` & `apiron-7.1.0.post3/src/apiron/service/base.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron/service/discoverable.py` & `apiron-7.1.0.post3/src/apiron/service/discoverable.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/src/apiron.egg-info/PKG-INFO` & `apiron-7.1.0.post3/src/apiron.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apiron
-Version: 7.1.0.post2
+Version: 7.1.0.post3
 Summary: apiron helps you cook a tasty client for RESTful APIs. Just don't wash it with SOAP.
 Home-page: https://github.com/ithaka/apiron
 Author: Ithaka Harbors, Inc.
 Author-email: opensource@ithaka.org
 License: MIT
 Project-URL: Documentation, https://apiron.readthedocs.io
 Project-URL: Source, https://github.com/ithaka/apiron
```

### Comparing `apiron-7.1.0.post2/src/apiron.egg-info/SOURCES.txt` & `apiron-7.1.0.post3/src/apiron.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/tests/service/test_base.py` & `apiron-7.1.0.post3/tests/service/test_base.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/tests/service/test_discoverable.py` & `apiron-7.1.0.post3/tests/service/test_discoverable.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/tests/test_client.py` & `apiron-7.1.0.post3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `apiron-7.1.0.post2/tests/test_endpoint.py` & `apiron-7.1.0.post3/tests/test_endpoint.py`

 * *Files identical despite different names*
