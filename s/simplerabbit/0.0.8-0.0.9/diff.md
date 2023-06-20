# Comparing `tmp/simplerabbit-0.0.8.tar.gz` & `tmp/simplerabbit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplerabbit-0.0.8.tar", last modified: Thu Apr 27 11:54:34 2023, max compression
+gzip compressed data, was "simplerabbit-0.0.9.tar", last modified: Mon May  1 09:59:51 2023, max compression
```

## Comparing `simplerabbit-0.0.8.tar` & `simplerabbit-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.8/README.md
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-04-27 11:54:19.000000 simplerabbit-0.0.8/pyproject.toml
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/setup.cfg
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/src/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-25 11:00:31.000000 simplerabbit-0.0.8/src/__init__.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/src/simplerabbit/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.8/src/simplerabbit/__init__.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1993 2023-04-27 04:09:00.000000 simplerabbit-0.0.8/src/simplerabbit/rabbit_base.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2622 2023-04-27 11:53:23.000000 simplerabbit-0.0.8/src/simplerabbit/receiver.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2033 2023-04-27 11:53:00.000000 simplerabbit-0.0.8/src/simplerabbit/sender.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      325 2023-04-25 11:38:19.000000 simplerabbit-0.0.8/src/simplerabbit/test_receiver.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      473 2023-04-27 11:22:11.000000 simplerabbit-0.0.8/src/simplerabbit/test_receiver_ssl.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      243 2023-04-25 11:32:42.000000 simplerabbit-0.0.8/src/simplerabbit/test_sender.py
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      392 2023-04-27 03:27:41.000000 simplerabbit-0.0.8/src/simplerabbit/test_sender_ssl.py
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/src/simplerabbit.egg-info/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-04-27 11:54:34.000000 simplerabbit-0.0.8/src/simplerabbit.egg-info/PKG-INFO
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      471 2023-04-27 11:54:34.000000 simplerabbit-0.0.8/src/simplerabbit.egg-info/SOURCES.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-27 11:54:34.000000 simplerabbit-0.0.8/src/simplerabbit.egg-info/dependency_links.txt
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       22 2023-04-27 11:54:34.000000 simplerabbit-0.0.8/src/simplerabbit.egg-info/top_level.txt
-drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-27 11:54:34.567754 simplerabbit-0.0.8/tests/
--rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.8/tests/test.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-05-01 09:59:51.478381 simplerabbit-0.0.9/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-05-01 09:59:51.478381 simplerabbit-0.0.9/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1100 2023-04-11 11:23:43.000000 simplerabbit-0.0.9/README.md
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      638 2023-05-01 09:59:36.000000 simplerabbit-0.0.9/pyproject.toml
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       38 2023-05-01 09:59:51.478381 simplerabbit-0.0.9/setup.cfg
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-05-01 09:59:51.474381 simplerabbit-0.0.9/src/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-04-25 11:00:31.000000 simplerabbit-0.0.9/src/__init__.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-05-01 09:59:51.478381 simplerabbit-0.0.9/src/simplerabbit/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-04-11 11:39:32.000000 simplerabbit-0.0.9/src/simplerabbit/__init__.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1993 2023-05-01 09:56:44.000000 simplerabbit-0.0.9/src/simplerabbit/rabbit_base.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2622 2023-04-27 11:53:23.000000 simplerabbit-0.0.9/src/simplerabbit/receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     2033 2023-04-27 11:53:00.000000 simplerabbit-0.0.9/src/simplerabbit/sender.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      325 2023-04-25 11:38:19.000000 simplerabbit-0.0.9/src/simplerabbit/test_receiver.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      473 2023-04-27 11:22:11.000000 simplerabbit-0.0.9/src/simplerabbit/test_receiver_ssl.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      243 2023-04-27 12:06:40.000000 simplerabbit-0.0.9/src/simplerabbit/test_sender.py
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      392 2023-04-27 03:27:41.000000 simplerabbit-0.0.9/src/simplerabbit/test_sender_ssl.py
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-05-01 09:59:51.478381 simplerabbit-0.0.9/src/simplerabbit.egg-info/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)     1595 2023-05-01 09:59:51.000000 simplerabbit-0.0.9/src/simplerabbit.egg-info/PKG-INFO
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      471 2023-05-01 09:59:51.000000 simplerabbit-0.0.9/src/simplerabbit.egg-info/SOURCES.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        1 2023-05-01 09:59:51.000000 simplerabbit-0.0.9/src/simplerabbit.egg-info/dependency_links.txt
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)       22 2023-05-01 09:59:51.000000 simplerabbit-0.0.9/src/simplerabbit.egg-info/top_level.txt
+drwxrwxr-x   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)        0 2023-05-01 09:59:51.478381 simplerabbit-0.0.9/tests/
+-rw-rw-r--   0 AATSTestAdmin  (1000) AATSTestAdmin  (1000)      107 2023-04-11 12:29:32.000000 simplerabbit-0.0.9/tests/test.py
```

### Comparing `simplerabbit-0.0.8/PKG-INFO` & `simplerabbit-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `simplerabbit-0.0.8/README.md` & `simplerabbit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.8/pyproject.toml` & `simplerabbit-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "simplerabbit"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Phuong Do", email="phdo@energidanmark.dk" },
 ]
 description = "Simple RabbitMQ library"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `simplerabbit-0.0.8/src/simplerabbit/rabbit_base.py` & `simplerabbit-0.0.9/src/simplerabbit/rabbit_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 
         credentials = pika.PlainCredentials(username=self.username, password=self.password)
         parameters = pika.ConnectionParameters(
             host=self.host,
             port=self.port,
             virtual_host=self.virtual_host,
             credentials=credentials,
-            #ssl_options=pika.SSLOptions(ssl_context, 'www.test.edatom.dk'),
-            ssl_options=pika.SSLOptions(ssl_context),
+            ssl_options=pika.SSLOptions(ssl_context, 'www.test.edatom.dk'),
+            #ssl_options=pika.SSLOptions(ssl_context),
         )
         self.connection = pika.BlockingConnection(parameters)
 
     def _connect_insecured(self):
         credentials = pika.PlainCredentials(self.username,
                                             self.password) if self.username and self.password else None
         parameters = pika.ConnectionParameters(host=self.host, port=self.port, virtual_host=self.virtual_host,
```

### Comparing `simplerabbit-0.0.8/src/simplerabbit/receiver.py` & `simplerabbit-0.0.9/src/simplerabbit/receiver.py`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.8/src/simplerabbit/sender.py` & `simplerabbit-0.0.9/src/simplerabbit/sender.py`

 * *Files identical despite different names*

### Comparing `simplerabbit-0.0.8/src/simplerabbit.egg-info/PKG-INFO` & `simplerabbit-0.0.9/src/simplerabbit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplerabbit
-Version: 0.0.8
+Version: 0.0.9
 Summary: Simple RabbitMQ library
 Author-email: Phuong Do <phdo@energidanmark.dk>
 Project-URL: Homepage, https://github.com/Energidanmark/simplerabbit
 Project-URL: Bug Tracker, https://github.com/Energidanmark/simplerabbit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

