# Comparing `tmp/fastapi_websocket_pubsub-0.3.3.tar.gz` & `tmp/fastapi_websocket_pubsub-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_websocket_pubsub-0.3.3.tar", last modified: Mon Mar 27 13:48:11 2023, max compression
+gzip compressed data, was "fastapi_websocket_pubsub-0.3.4.tar", last modified: Tue Jun 20 11:54:54 2023, max compression
```

## Comparing `fastapi_websocket_pubsub-0.3.3.tar` & `fastapi_websocket_pubsub-0.3.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 13:48:11.619509 fastapi_websocket_pubsub-0.3.3/
--rw-r--r--   0 roekatz    (501) staff       (20)     1064 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/LICENSE
--rw-r--r--   0 roekatz    (501) staff       (20)       20 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/MANIFEST.in
--rw-r--r--   0 roekatz    (501) staff       (20)     7240 2023-03-27 13:48:11.619605 fastapi_websocket_pubsub-0.3.3/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)     6634 2022-08-23 19:15:45.000000 fastapi_websocket_pubsub-0.3.3/README.md
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 13:48:11.618213 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/
--rw-r--r--   0 roekatz    (501) staff       (20)      275 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/__init__.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11547 2023-03-27 12:37:52.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/event_broadcaster.py
--rw-r--r--   0 roekatz    (501) staff       (20)    11994 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/event_notifier.py
--rw-r--r--   0 roekatz    (501) staff       (20)      397 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/exceptions.py
--rwxr-xr-x   0 roekatz    (501) staff       (20)      137 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/logger.py
--rw-r--r--   0 roekatz    (501) staff       (20)    15689 2022-08-23 19:15:45.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/pub_sub_client.py
--rw-r--r--   0 roekatz    (501) staff       (20)     7397 2023-03-27 12:37:52.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/pub_sub_server.py
--rw-r--r--   0 roekatz    (501) staff       (20)     3865 2022-08-23 19:15:45.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/rpc_event_methods.py
--rw-r--r--   0 roekatz    (501) staff       (20)      100 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/websocket_rpc_event_notifier.py
-drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-03-27 13:48:11.619330 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/
--rw-r--r--   0 roekatz    (501) staff       (20)     7240 2023-03-27 13:48:11.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/PKG-INFO
--rw-r--r--   0 roekatz    (501) staff       (20)      676 2023-03-27 13:48:11.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/SOURCES.txt
--rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-03-27 13:48:11.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/dependency_links.txt
--rw-r--r--   0 roekatz    (501) staff       (20)      121 2023-03-27 13:48:11.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/requires.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       25 2023-03-27 13:48:11.000000 fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/top_level.txt
--rw-r--r--   0 roekatz    (501) staff       (20)       79 2023-03-27 13:48:11.619997 fastapi_websocket_pubsub-0.3.3/setup.cfg
--rw-r--r--   0 roekatz    (501) staff       (20)     1095 2023-03-27 13:33:29.000000 fastapi_websocket_pubsub-0.3.3/setup.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:54:54.556628 fastapi_websocket_pubsub-0.3.4/
+-rw-r--r--   0 roekatz    (501) staff       (20)     1064 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/LICENSE
+-rw-r--r--   0 roekatz    (501) staff       (20)       20 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/MANIFEST.in
+-rw-r--r--   0 roekatz    (501) staff       (20)     7240 2023-06-20 11:54:54.556745 fastapi_websocket_pubsub-0.3.4/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)     6634 2022-08-23 19:15:45.000000 fastapi_websocket_pubsub-0.3.4/README.md
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:54:54.555347 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/
+-rw-r--r--   0 roekatz    (501) staff       (20)      275 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/__init__.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11547 2023-06-20 11:37:18.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/event_broadcaster.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    11994 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/event_notifier.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      397 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/exceptions.py
+-rwxr-xr-x   0 roekatz    (501) staff       (20)      137 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/logger.py
+-rw-r--r--   0 roekatz    (501) staff       (20)    15689 2022-08-23 19:15:45.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/pub_sub_client.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     7397 2023-06-20 11:37:18.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/pub_sub_server.py
+-rw-r--r--   0 roekatz    (501) staff       (20)     3865 2022-08-23 19:15:45.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/rpc_event_methods.py
+-rw-r--r--   0 roekatz    (501) staff       (20)      100 2022-05-30 14:27:21.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/websocket_rpc_event_notifier.py
+drwxr-xr-x   0 roekatz    (501) staff       (20)        0 2023-06-20 11:54:54.556215 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/
+-rw-r--r--   0 roekatz    (501) staff       (20)     7240 2023-06-20 11:54:54.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/PKG-INFO
+-rw-r--r--   0 roekatz    (501) staff       (20)      676 2023-06-20 11:54:54.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/SOURCES.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)        1 2023-06-20 11:54:54.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/dependency_links.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)      121 2023-06-20 11:54:54.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/requires.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       25 2023-06-20 11:54:54.000000 fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/top_level.txt
+-rw-r--r--   0 roekatz    (501) staff       (20)       79 2023-06-20 11:54:54.557012 fastapi_websocket_pubsub-0.3.4/setup.cfg
+-rw-r--r--   0 roekatz    (501) staff       (20)     1098 2023-06-20 11:45:45.000000 fastapi_websocket_pubsub-0.3.4/setup.py
```

### Comparing `fastapi_websocket_pubsub-0.3.3/LICENSE` & `fastapi_websocket_pubsub-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/PKG-INFO` & `fastapi_websocket_pubsub-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fastapi_websocket_pubsub
-Version: 0.3.3
+Version: 0.3.4
 Summary: A fast and durable PubSub channel over Websockets (using fastapi-websockets-rpc).
 Home-page: https://github.com/permitio/fastapi_websocket_pubsub
 Author: Or Weis
 Author-email: or@permit.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="https://i.ibb.co/NV6wmy8/pubsub.png" width="55%" alt="pubsub" border="0">
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: fastapi_websocket_pubsub Version: 0.3.3 Summary: A
+Metadata-Version: 2.1 Name: fastapi_websocket_pubsub Version: 0.3.4 Summary: A
 fast and durable PubSub channel over Websockets (using fastapi-websockets-rpc).
 Home-page: https://github.com/permitio/fastapi_websocket_pubsub Author: Or Weis
 Author-email: or@permit.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.7
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                                    [pubsub]
 # # â¡ðï¸ FastAPI Websocket Pub/Sub [Tests] [Package] [Downloads] A fast
 and durable Pub/Sub channel over Websockets. The easiest way to create a live
 publish / subscribe multi-cast over the web. Supports and tested on Python >=
 3.7 As seen at PyCon_IL_2021 and EuroPython_2021 ## Installation ð ï¸ ```
 pip install fastapi_websocket_pubsub ``` ## Intro The classic pub/sub pattern
```

### Comparing `fastapi_websocket_pubsub-0.3.3/README.md` & `fastapi_websocket_pubsub-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/event_broadcaster.py` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/event_broadcaster.py`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/event_notifier.py` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/event_notifier.py`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/pub_sub_client.py` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/pub_sub_client.py`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/pub_sub_server.py` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/pub_sub_server.py`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub/rpc_event_methods.py` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub/rpc_event_methods.py`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/PKG-INFO` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: fastapi-websocket-pubsub
-Version: 0.3.3
+Version: 0.3.4
 Summary: A fast and durable PubSub channel over Websockets (using fastapi-websockets-rpc).
 Home-page: https://github.com/permitio/fastapi_websocket_pubsub
 Author: Or Weis
 Author-email: or@permit.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
 <img src="https://i.ibb.co/NV6wmy8/pubsub.png" width="55%" alt="pubsub" border="0">
 </p>
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
-Metadata-Version: 2.1 Name: fastapi-websocket-pubsub Version: 0.3.3 Summary: A
+Metadata-Version: 2.1 Name: fastapi-websocket-pubsub Version: 0.3.4 Summary: A
 fast and durable PubSub channel over Websockets (using fastapi-websockets-rpc).
 Home-page: https://github.com/permitio/fastapi_websocket_pubsub Author: Or Weis
 Author-email: or@permit.io Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.7
+Classifier: Topic :: Internet :: WWW/HTTP :: WSGI Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
                                    [pubsub]
 # # â¡ðï¸ FastAPI Websocket Pub/Sub [Tests] [Package] [Downloads] A fast
 and durable Pub/Sub channel over Websockets. The easiest way to create a live
 publish / subscribe multi-cast over the web. Supports and tested on Python >=
 3.7 As seen at PyCon_IL_2021 and EuroPython_2021 ## Installation ð ï¸ ```
 pip install fastapi_websocket_pubsub ``` ## Intro The classic pub/sub pattern
```

### Comparing `fastapi_websocket_pubsub-0.3.3/fastapi_websocket_pubsub.egg-info/SOURCES.txt` & `fastapi_websocket_pubsub-0.3.4/fastapi_websocket_pubsub.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_websocket_pubsub-0.3.3/setup.py` & `fastapi_websocket_pubsub-0.3.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 from setuptools import setup, find_packages
 
+
 def get_requirements(env=""):
     if env:
         env = "-{}".format(env)
     with open("requirements{}.txt".format(env)) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
 
+
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
-    name='fastapi_websocket_pubsub',
-    version='0.3.3',
-    author='Or Weis',
+    name="fastapi_websocket_pubsub",
+    version="0.3.4",
+    author="Or Weis",
     author_email="or@permit.io",
     description="A fast and durable PubSub channel over Websockets (using fastapi-websockets-rpc).",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://github.com/permitio/fastapi_websocket_pubsub",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
-        "Topic :: Internet :: WWW/HTTP :: WSGI"
+        "Topic :: Internet :: WWW/HTTP :: WSGI",
     ],
-    python_requires='>=3.7',
+    python_requires=">=3.8",
     install_requires=get_requirements(),
 )
```

