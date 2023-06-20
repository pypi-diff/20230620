# Comparing `tmp/kafka_connect_watcher-0.3.1.tar.gz` & `tmp/kafka_connect_watcher-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kafka_connect_watcher-0.3.1.tar", max compression
+gzip compressed data, was "kafka_connect_watcher-0.3.2.tar", max compression
```

## Comparing `kafka_connect_watcher-0.3.1.tar` & `kafka_connect_watcher-0.3.2.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      944 2023-02-28 14:05:27.479088 kafka_connect_watcher-0.3.1/README.rst
--rw-r--r--   0        0        0      189 2023-04-17 15:35:02.457313 kafka_connect_watcher-0.3.1/kafka_connect_watcher/__init__.py
--rw-r--r--   0        0        0     4038 2023-03-15 14:40:57.739243 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_emf.py
--rw-r--r--   0        0        0     5383 2023-04-17 15:31:09.335440 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/__init__.py
--rw-r--r--   0        0        0      107 2023-03-20 14:52:32.551851 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/default.j2
--rw-r--r--   0        0        0      140 2023-03-20 14:10:44.078719 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/email.j2
--rw-r--r--   0        0        0       80 2023-03-20 14:45:41.271914 kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/sms.j2
--rw-r--r--   0        0        0      616 2023-02-28 16:04:00.414003 kafka_connect_watcher-0.3.1/kafka_connect_watcher/cli.py
--rw-r--r--   0        0        0     3466 2023-03-20 15:50:03.131477 kafka_connect_watcher-0.3.1/kafka_connect_watcher/cluster.py
--rw-r--r--   0        0        0     5075 2023-03-22 20:06:47.639263 kafka_connect_watcher-0.3.1/kafka_connect_watcher/config.py
--rw-r--r--   0        0        0     2571 2023-03-22 21:01:49.767003 kafka_connect_watcher-0.3.1/kafka_connect_watcher/connectors_eval.py
--rw-r--r--   0        0        0     8064 2023-03-22 20:17:29.774964 kafka_connect_watcher-0.3.1/kafka_connect_watcher/error_rules.py
--rw-r--r--   0        0        0     1928 2023-04-17 15:32:30.604442 kafka_connect_watcher-0.3.1/kafka_connect_watcher/logger.py
--rw-r--r--   0        0        0      918 2023-03-22 21:01:49.737002 kafka_connect_watcher-0.3.1/kafka_connect_watcher/notifications.py
--rw-r--r--   0        0        0      254 2023-01-23 17:30:58.219507 kafka_connect_watcher-0.3.1/kafka_connect_watcher/threads_settings.py
--rw-r--r--   0        0        0      492 2023-01-23 08:58:32.729607 kafka_connect_watcher-0.3.1/kafka_connect_watcher/tools.py
--rw-r--r--   0        0        0     8149 2023-03-23 13:26:18.128320 kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher-config.spec.json
--rw-r--r--   0        0        0     4674 2023-04-17 15:24:05.452215 kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher.py
--rw-r--r--   0        0        0     2489 2023-04-17 15:35:02.457313 kafka_connect_watcher-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2163 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.1/setup.py
--rw-r--r--   0        0        0     2480 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      944 2023-02-28 14:05:27.479088 kafka_connect_watcher-0.3.2/README.rst
+-rw-r--r--   0        0        0      189 2023-06-20 08:19:49.549786 kafka_connect_watcher-0.3.2/kafka_connect_watcher/__init__.py
+-rw-r--r--   0        0        0     4038 2023-04-17 17:49:03.339977 kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_emf.py
+-rw-r--r--   0        0        0     5383 2023-04-17 15:31:09.335440 kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_sns/__init__.py
+-rw-r--r--   0        0        0      107 2023-03-20 14:52:32.551851 kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_sns/default.j2
+-rw-r--r--   0        0        0      140 2023-03-20 14:10:44.078719 kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_sns/email.j2
+-rw-r--r--   0        0        0       80 2023-03-20 14:45:41.271914 kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_sns/sms.j2
+-rw-r--r--   0        0        0      616 2023-02-28 16:04:00.414003 kafka_connect_watcher-0.3.2/kafka_connect_watcher/cli.py
+-rw-r--r--   0        0        0     3466 2023-04-17 21:56:47.586979 kafka_connect_watcher-0.3.2/kafka_connect_watcher/cluster.py
+-rw-r--r--   0        0        0     5075 2023-06-20 08:13:09.789116 kafka_connect_watcher-0.3.2/kafka_connect_watcher/config.py
+-rw-r--r--   0        0        0     2571 2023-06-20 08:13:09.790116 kafka_connect_watcher-0.3.2/kafka_connect_watcher/connectors_eval.py
+-rw-r--r--   0        0        0     8064 2023-06-20 08:13:09.790116 kafka_connect_watcher-0.3.2/kafka_connect_watcher/error_rules.py
+-rw-r--r--   0        0        0     1928 2023-04-17 15:32:30.604442 kafka_connect_watcher-0.3.2/kafka_connect_watcher/logger.py
+-rw-r--r--   0        0        0      918 2023-03-22 21:01:49.737002 kafka_connect_watcher-0.3.2/kafka_connect_watcher/notifications.py
+-rw-r--r--   0        0        0      254 2023-01-23 17:30:58.219507 kafka_connect_watcher-0.3.2/kafka_connect_watcher/threads_settings.py
+-rw-r--r--   0        0        0      492 2023-01-23 08:58:32.729607 kafka_connect_watcher-0.3.2/kafka_connect_watcher/tools.py
+-rw-r--r--   0        0        0     8149 2023-06-20 08:13:09.791116 kafka_connect_watcher-0.3.2/kafka_connect_watcher/watcher-config.spec.json
+-rw-r--r--   0        0        0     4674 2023-06-20 08:13:09.791116 kafka_connect_watcher-0.3.2/kafka_connect_watcher/watcher.py
+-rw-r--r--   0        0        0     2489 2023-06-20 08:19:49.549786 kafka_connect_watcher-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2281 1970-01-01 00:00:00.000000 kafka_connect_watcher-0.3.2/PKG-INFO
```

### Comparing `kafka_connect_watcher-0.3.1/README.rst` & `kafka_connect_watcher-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_emf.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_emf.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/aws_sns/__init__.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/aws_sns/__init__.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/cli.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/cli.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/cluster.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/cluster.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/config.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/config.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/connectors_eval.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/connectors_eval.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/error_rules.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/error_rules.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/logger.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/logger.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/notifications.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/notifications.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher-config.spec.json` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/watcher-config.spec.json`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/kafka_connect_watcher/watcher.py` & `kafka_connect_watcher-0.3.2/kafka_connect_watcher/watcher.py`

 * *Files identical despite different names*

### Comparing `kafka_connect_watcher-0.3.1/pyproject.toml` & `kafka_connect_watcher-0.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kafka-connect-watcher"
-version = "0.3.1"
+version = "0.3.2"
 description = "Kafka Connect active watcher"
 authors = ["John \"Preston\" Mille <john@ews-network.net>"]
 readme = "README.rst"
 license = "MPL-2.0"
 keywords = ["kafka", "connect", "monitoring", "observability"]
 classifiers = [
   "Development Status :: 4 - Beta",
@@ -83,15 +83,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/johnpreston/kafka-connect-watcher"
 
 [tool.tbump.version]
-current = "0.3.1"
+current = "0.3.2"
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
   (?:(?P<rc>[\S]+))?
```

### Comparing `kafka_connect_watcher-0.3.1/PKG-INFO` & `kafka_connect_watcher-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kafka-connect-watcher
-Version: 0.3.1
+Version: 0.3.2
 Summary: Kafka Connect active watcher
 License: MPL-2.0
 Keywords: kafka,connect,monitoring,observability
 Author: John "Preston" Mille
 Author-email: john@ews-network.net
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -15,18 +15,14 @@
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aws-embedded-metrics (>=3.0.0,<4.0.0)
 Requires-Dist: compose-x-common (>=1.2,<2.0)
 Requires-Dist: importlib-resources (>=5.10,<6.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: kafka-connect-api (>=0.5.3,<0.6.0)
 Requires-Dist: prometheus-client (>=0.16,<0.17)
```

