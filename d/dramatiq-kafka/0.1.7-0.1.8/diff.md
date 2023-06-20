# Comparing `tmp/dramatiq_kafka-0.1.7.tar.gz` & `tmp/dramatiq_kafka-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_kafka-0.1.7.tar", max compression
+gzip compressed data, was "dramatiq_kafka-0.1.8.tar", max compression
```

## Comparing `dramatiq_kafka-0.1.7.tar` & `dramatiq_kafka-0.1.8.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1228 2023-06-16 08:12:06.848140 dramatiq_kafka-0.1.7/README.md
--rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.7/dramatiq_kafka/__init__.py
--rw-r--r--   0        0        0     4318 2023-06-20 03:31:24.214817 dramatiq_kafka-0.1.7/dramatiq_kafka/broker.py
--rw-r--r--   0        0        0      351 2023-06-20 03:33:31.868025 dramatiq_kafka-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1201 2023-06-20 03:42:55.693621 dramatiq_kafka-0.1.8/README.md
+-rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.8/dramatiq_kafka/__init__.py
+-rw-r--r--   0        0        0     4318 2023-06-20 03:31:24.214817 dramatiq_kafka-0.1.8/dramatiq_kafka/broker.py
+-rw-r--r--   0        0        0      350 2023-06-20 04:19:01.618992 dramatiq_kafka-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1679 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.8/PKG-INFO
```

### Comparing `dramatiq_kafka-0.1.7/README.md` & `dramatiq_kafka-0.1.8/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -19,22 +19,23 @@
         Pipelines(),
         Retries(min_backoff=1000, max_backoff=900000, max_retries=96),
     ],
 )
 dramatiq.set_broker(broker)
 ```
 
-Use dramatiq to send a message to a Kafka topic with the following format:
+Use dramatiq to send a message to a Kafka topic (`queue_name`) as usual:
 
 ```python
-{
-    "queue_name": "testdramatiq_topic",
-    "actor_name": "email_customer",
-    "args": ["testing@gmail.com"],
-    "kwargs": {},
-    "options": {},
-    "message_id": "e566b8d8-4e3d-437d-989f-939dd4f8ee04",
-    "message_timestamp": 1686877955147
-}
+    message = Message(
+        queue_name="rita",
+        actor_name="email_customer",
+        args=("testing@gmail.com",),
+        kwargs={},
+        options={},
+    )
+
+    broker = get_broker()
+    broker.enqueue(message)
 ```
 
 Write tasks as described in django_dramatiq's documentation (i.e. create dramatiq actors in the task.py files) and modify settings as shown in `django_example` to get started. To send messages, view the views.py file for an example
```

### Comparing `dramatiq_kafka-0.1.7/dramatiq_kafka/broker.py` & `dramatiq_kafka-0.1.8/dramatiq_kafka/broker.py`

 * *Files identical despite different names*

### Comparing `dramatiq_kafka-0.1.7/PKG-INFO` & `dramatiq_kafka-0.1.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 Metadata-Version: 2.1
 Name: dramatiq-kafka
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Kafka broker for Dramatiq.
 Author: Viktor Babchanik
 Author-email: vbabchanik@ucdavis.edu
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 Uses kafka-python package to write a Kafka broker for dramatiq.
 
 ```python
 
@@ -30,23 +33,24 @@
         Pipelines(),
         Retries(min_backoff=1000, max_backoff=900000, max_retries=96),
     ],
 )
 dramatiq.set_broker(broker)
 ```
 
-Use dramatiq to send a message to a Kafka topic with the following format:
+Use dramatiq to send a message to a Kafka topic (`queue_name`) as usual:
 
 ```python
-{
-    "queue_name": "testdramatiq_topic",
-    "actor_name": "email_customer",
-    "args": ["testing@gmail.com"],
-    "kwargs": {},
-    "options": {},
-    "message_id": "e566b8d8-4e3d-437d-989f-939dd4f8ee04",
-    "message_timestamp": 1686877955147
-}
+    message = Message(
+        queue_name="rita",
+        actor_name="email_customer",
+        args=("testing@gmail.com",),
+        kwargs={},
+        options={},
+    )
+
+    broker = get_broker()
+    broker.enqueue(message)
 ```
 
 Write tasks as described in django_dramatiq's documentation (i.e. create dramatiq actors in the task.py files) and modify settings as shown in `django_example` to get started. To send messages, view the views.py file for an example
```

