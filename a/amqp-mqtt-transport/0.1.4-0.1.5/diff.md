# Comparing `tmp/amqp-mqtt-transport-0.1.4.tar.gz` & `tmp/amqp_mqtt_transport-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp-mqtt-transport-0.1.4.tar", last modified: Tue Jun 20 19:24:13 2023, max compression
+gzip compressed data, was "amqp_mqtt_transport-0.1.5.tar", last modified: Tue Jun 20 19:29:10 2023, max compression
```

## Comparing `amqp-mqtt-transport-0.1.4.tar` & `amqp_mqtt_transport-0.1.5.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:24:13.798041 amqp-mqtt-transport-0.1.4/
--rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp-mqtt-transport-0.1.4/.gitattributes
--rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp-mqtt-transport-0.1.4/.gitignore
--rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp-mqtt-transport-0.1.4/LICENSE
--rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp-mqtt-transport-0.1.4/Makefile
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 19:24:13.798041 amqp-mqtt-transport-0.1.4/PKG-INFO
--rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp-mqtt-transport-0.1.4/README.md
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:24:13.798041 amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 19:24:13.000000 amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)      290 2023-06-20 19:24:13.000000 amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 19:24:13.000000 amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       65 2023-06-20 19:24:13.000000 amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/requires.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 19:24:13.000000 amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/top_level.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)      758 2023-06-20 19:23:30.000000 amqp-mqtt-transport-0.1.4/pyproject.toml
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-20 19:24:13.798041 amqp-mqtt-transport-0.1.4/setup.cfg
--rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp-mqtt-transport-0.1.4/setup.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/
+-rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp_mqtt_transport-0.1.5/.gitattributes
+-rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp_mqtt_transport-0.1.5/.gitignore
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp_mqtt_transport-0.1.5/LICENSE
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp_mqtt_transport-0.1.5/Makefile
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/PKG-INFO
+-rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp_mqtt_transport-0.1.5/README.md
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.461011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/
+-rw-rw-r--   0 igor      (1001) igor      (1001)      146 2023-06-19 12:15:25.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      956 2023-06-19 12:15:26.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/abc.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1728 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/consumer.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     5533 2023-06-19 12:15:29.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1521 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2102 2023-06-19 12:15:26.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/message_scheduler.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     3115 2023-06-19 12:15:31.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      807 2023-06-19 12:15:32.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2430 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/scheduled_publisher.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.461011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)      698 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/SOURCES.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/dependency_links.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       65 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/requires.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       20 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/top_level.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)      758 2023-06-20 19:27:50.000000 amqp_mqtt_transport-0.1.5/pyproject.toml
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/setup.cfg
+-rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp_mqtt_transport-0.1.5/setup.py
```

### Comparing `amqp-mqtt-transport-0.1.4/LICENSE` & `amqp_mqtt_transport-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.4/Makefile` & `amqp_mqtt_transport-0.1.5/Makefile`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.4/PKG-INFO` & `amqp_mqtt_transport-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: amqp-mqtt-transport
-Version: 0.1.4
+Name: amqp_mqtt_transport
+Version: 0.1.5
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp-mqtt-transport-0.1.4/README.md` & `amqp_mqtt_transport-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `amqp-mqtt-transport-0.1.4/amqp_mqtt_transport.egg-info/PKG-INFO` & `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.4
+Version: 0.1.5
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp-mqtt-transport-0.1.4/pyproject.toml` & `amqp_mqtt_transport-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
-name = "amqp-mqtt-transport"
-version = "0.1.4"
+name = "amqp_mqtt_transport"
+version = "0.1.5"
 authors = [
   { name="Igor Toropov", email="it.cups.54@gmail.com" },
 ]
 description = "Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

