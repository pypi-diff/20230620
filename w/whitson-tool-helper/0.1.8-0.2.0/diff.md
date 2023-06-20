# Comparing `tmp/whitson_tool_helper-0.1.8.tar.gz` & `tmp/whitson_tool_helper-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/markus/Documents/BitBucket/whitson-tool-helper/dist/.tmp-gzk2loz2/whitson_tool_helper-0.1.8.tar", last modified: Sat Jun 17 16:29:58 2023, max compression
+gzip compressed data, was "whitson_tool_helper-0.2.0.tar", last modified: Tue Jun 20 19:53:59 2023, max compression
```

## Comparing `whitson_tool_helper-0.1.8.tar` & `whitson_tool_helper-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-06-17 16:25:45.000000 whitson_tool_helper-0.1.8/pyproject.toml
--rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/setup.cfg
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/
--rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/__init__.py
--rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/logger.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/
--rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/helper.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     2729 2023-05-29 07:32:28.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/main.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3746 2023-06-12 08:05:49.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/pubsub.py
--rw-rw-r--   0 markus    (1000) markus    (1000)     3652 2023-06-17 16:24:47.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/rabbitmq.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/timeout.py
--rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper/whitson_exceptions.py
-drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/
--rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/PKG-INFO
--rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/SOURCES.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/dependency_links.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/requires.txt
--rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-06-17 16:29:58.000000 whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/top_level.txt
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      705 2023-06-20 19:53:53.000000 whitson_tool_helper-0.2.0/pyproject.toml
+-rw-rw-r--   0 markus    (1000) markus    (1000)       38 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/setup.cfg
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.635835 whitson_tool_helper-0.2.0/src/
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.635835 whitson_tool_helper-0.2.0/src/whitson_tool_helper/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      107 2023-04-26 09:25:11.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)       66 2023-04-26 13:06:47.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/logger.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.639835 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      370 2023-05-28 08:36:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/helper.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     2737 2023-06-20 19:52:57.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/main.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3746 2023-06-12 08:05:49.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/pubsub.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4201 2023-06-20 19:48:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/rabbitmq.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      574 2023-04-25 15:19:43.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/timeout.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)      704 2023-04-26 12:57:07.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper/whitson_exceptions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-06-20 19:53:59.635835 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      404 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      575 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)      116 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       20 2023-06-20 19:53:59.000000 whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/main.py` & `whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 LOGGER.error(e)
                 sys.exit()
             except Exception as e:
                 LOGGER.error("-- UNKNOWN ERROR ENCOUNTERED --")
                 LOGGER.error(e)
             finally:
                 if self._messaging_system == MessagingSystem.rabbitmq:
-                    self._consumer.connection.close()
+                    self._consumer.ack_and_close_connection()
                 LOGGER.warning("Restarting worker")
 
 
 class Publisher:
     def __init__(self, messaging_system: MessagingSystem, exchange: str = None):
         if messaging_system == MessagingSystem.pubsub:
             from whitson_tool_helper.messaging import pubsub
```

### Comparing `whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/pubsub.py` & `whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/pubsub.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.8/src/whitson_tool_helper/messaging/rabbitmq.py` & `whitson_tool_helper-0.2.0/src/whitson_tool_helper/messaging/rabbitmq.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,16 +25,36 @@
         credentials=credentials,
     )
 
 
 class RabbitMQConsumer:
     def __init__(self, process_function):
         self.process_function = process_function
-
+        self.well_id = None
+        self.model = None
+        self.delivery_tag = None
         check_environment_variables(["MESSAGING_SUBSCRIPTION"])
+
+    def _callback(self, ch, method, properties, body):
+        if not body or body.decode("utf-8") == "":
+            ch.basic_ack(delivery_tag=method.delivery_tag)
+            LOGGER.info("Recieved faulty message")
+            LOGGER.info("Listening to", method.routing_key, "...")
+            return
+
+        msg = json.loads(body.decode("utf-8"))
+        self.well_id = msg["data"].get("well_id") or "Unkown"
+        self.model = msg["data"].get("model") or "Unkown"
+        self.delivery_tag = method.delivery_tag
+        self.process_function(data=msg["data"], meta_data=msg["meta_data"])
+        LOGGER.info("  ---  SUCCESS  ---  ")
+        ch.basic_ack(delivery_tag=method.delivery_tag)
+        LOGGER.info(f"Listening to {method.routing_key} ...")
+
+    def _initialize_connection_and_channel(self):
         parameters = get_rabbitmq_params()
         self.connection = pika.BlockingConnection(parameters)
         self.channel = self.connection.channel()
         subscription = os.getenv("MESSAGING_SUBSCRIPTION")
         self.channel.queue_declare(
             queue=subscription,
             durable=True,
@@ -43,33 +63,24 @@
         exchange = "engines"
         if subscription.endswith("-calculated"):
             exchange = "clients"
 
         self.channel.queue_bind(
             queue=subscription, exchange=exchange, routing_key=subscription
         )
-
         self.channel.basic_qos(prefetch_count=1)
+        self.channel.basic_consume(queue=subscription, on_message_callback=self._callback)
 
-        def callback(ch, method, properties, body):
-            if not body or body.decode("utf-8") == "":
-                ch.basic_ack(delivery_tag=method.delivery_tag)
-                LOGGER.info("Recieved faulty message")
-                LOGGER.info("Listening to", method.routing_key, "...")
-                return
-
-            msg = json.loads(body.decode("utf-8"))
-            process_function(data=msg["data"], meta_data=msg["meta_data"])
-            LOGGER.info("  ---  SUCCESS  ---  ")
-            ch.basic_ack(delivery_tag=method.delivery_tag)
-            LOGGER.info(f"Listening to {method.routing_key} ...")
-
-        self.channel.basic_consume(queue=subscription, on_message_callback=callback)
+    def ack_and_close_connection(self):
+        LOGGER.critical(f"Destroyed calc {self.model} for well {self.well_id}")
+        self.channel.basic_ack(delivery_tag=self.delivery_tag)
+        self.channel.stop_consuming()
 
     def work(self):
+        self._initialize_connection_and_channel()
         self.channel.start_consuming()
 
 
 class RabbitMQPublisher:
     def __init__(self, exchange):
         self.parameters = get_rabbitmq_params()
         self.exchange = exchange
```

### Comparing `whitson_tool_helper-0.1.8/src/whitson_tool_helper/timeout.py` & `whitson_tool_helper-0.2.0/src/whitson_tool_helper/timeout.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.8/src/whitson_tool_helper/whitson_exceptions.py` & `whitson_tool_helper-0.2.0/src/whitson_tool_helper/whitson_exceptions.py`

 * *Files identical despite different names*

### Comparing `whitson_tool_helper-0.1.8/src/whitson_tool_helper.egg-info/SOURCES.txt` & `whitson_tool_helper-0.2.0/src/whitson_tool_helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

