# Comparing `tmp/dramatiq_kafka-0.1.5.tar.gz` & `tmp/dramatiq_kafka-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramatiq_kafka-0.1.5.tar", max compression
+gzip compressed data, was "dramatiq_kafka-0.1.6.tar", max compression
```

## Comparing `dramatiq_kafka-0.1.5.tar` & `dramatiq_kafka-0.1.6.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1228 2023-06-16 08:12:06.848140 dramatiq_kafka-0.1.5/README.md
--rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.5/dramatiq_kafka/__init__.py
--rw-r--r--   0        0        0     4359 2023-06-20 03:07:58.795638 dramatiq_kafka-0.1.5/dramatiq_kafka/broker.py
--rw-r--r--   0        0        0      351 2023-06-20 03:14:55.481316 dramatiq_kafka-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1228 2023-06-16 08:12:06.848140 dramatiq_kafka-0.1.6/README.md
+-rw-r--r--   0        0        0       32 2023-06-16 03:12:34.377444 dramatiq_kafka-0.1.6/dramatiq_kafka/__init__.py
+-rw-r--r--   0        0        0     4355 2023-06-20 03:25:10.060656 dramatiq_kafka-0.1.6/dramatiq_kafka/broker.py
+-rw-r--r--   0        0        0      351 2023-06-20 03:27:13.379096 dramatiq_kafka-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 dramatiq_kafka-0.1.6/PKG-INFO
```

### Comparing `dramatiq_kafka-0.1.5/README.md` & `dramatiq_kafka-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dramatiq_kafka-0.1.5/dramatiq_kafka/broker.py` & `dramatiq_kafka-0.1.6/dramatiq_kafka/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,16 +54,17 @@
         *,
         delay: Optional[int] = None,
         topic: Optional[str] = None,
     ) -> Message:
         if delay:
             sleep(delay)
 
-        t = topic if topic else self.topic
-        self.producer.send(t, json.dumps(message.asdict()).encode("utf-8"))
+        self.producer.send(
+            message.queue_name, json.dumps(message.asdict()).encode("utf-8")
+        )
         self.producer.flush()
         return message
 
     def consume(
         self, queue_name: str, prefetch: int = 1, timeout: int = 30000
     ) -> Consumer:
         return _KafkaConsumer(
```

### Comparing `dramatiq_kafka-0.1.5/PKG-INFO` & `dramatiq_kafka-0.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramatiq-kafka
-Version: 0.1.5
+Version: 0.1.6
 Summary: A Kafka broker for Dramatiq.
 Author: Viktor Babchanik
 Author-email: vbabchanik@ucdavis.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

