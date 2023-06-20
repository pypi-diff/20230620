# Comparing `tmp/dramatiq_kafka-0.1.6.tar.gz` & `tmp/dramatiq_kafka-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_kafka-0.1.6.tar", max compression
+gzip compressed data, was "dramatiq_kafka-0.1.7.tar", max compression
```

## Comparing `dramatiq_kafka-0.1.6.tar` & `dramatiq_kafka-0.1.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1228 2023-06-16 08:12:06.848140 dramatiq_kafka-0.1.6/README.md
--rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.6/dramatiq_kafka/__init__.py
--rw-r--r--   0        0        0     4355 2023-06-20 03:25:10.060656 dramatiq_kafka-0.1.6/dramatiq_kafka/broker.py
--rw-r--r--   0        0        0      351 2023-06-20 03:27:13.379096 dramatiq_kafka-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1228 2023-06-16 08:12:06.848140 dramatiq_kafka-0.1.7/README.md
+-rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.7/dramatiq_kafka/__init__.py
+-rw-r--r--   0        0        0     4318 2023-06-20 03:31:24.214817 dramatiq_kafka-0.1.7/dramatiq_kafka/broker.py
+-rw-r--r--   0        0        0      351 2023-06-20 03:33:31.868025 dramatiq_kafka-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.7/PKG-INFO
```

### Comparing `dramatiq_kafka-0.1.6/README.md` & `dramatiq_kafka-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_kafka-0.1.6/dramatiq_kafka/broker.py` & `dramatiq_kafka-0.1.7/dramatiq_kafka/broker.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
         self.queues.append(queue_name)
 
     def enqueue(
         self,
         message: Message,
         *,
         delay: Optional[int] = None,
-        topic: Optional[str] = None,
     ) -> Message:
         if delay:
             sleep(delay)
 
         self.producer.send(
             message.queue_name, json.dumps(message.asdict()).encode("utf-8")
         )
```

### Comparing `dramatiq_kafka-0.1.6/PKG-INFO` & `dramatiq_kafka-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq-kafka
-Version: 0.1.6
+Version: 0.1.7
 Summary: A Kafka broker for Dramatiq.
 Author: Viktor Babchanik
 Author-email: vbabchanik@ucdavis.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

