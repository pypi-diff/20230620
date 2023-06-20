# Comparing `tmp/cmem_plugin_kafka-1.3.0.tar.gz` & `tmp/cmem_plugin_kafka-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_plugin_kafka-1.3.0.tar", max compression
+gzip compressed data, was "cmem_plugin_kafka-1.3.0rc1.tar", max compression
```

## Comparing `cmem_plugin_kafka-1.3.0.tar` & `cmem_plugin_kafka-1.3.0rc1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    11334 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/LICENSE
--rw-r--r--   0        0        0     3733 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/README-public.md
--rw-r--r--   0        0        0        0 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/__init__.py
--rw-r--r--   0        0        0     4432 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/constants.py
--rw-r--r--   0        0        0    14682 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/kafka_handlers.py
--rw-r--r--   0        0        0    11743 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/utils.py
--rw-r--r--   0        0        0        0 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/__init__.py
--rw-r--r--   0        0        0    11640 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/consumer.py
--rw-r--r--   0        0        0     9739 2023-06-12 09:29:48.249799 cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/producer.py
--rw-r--r--   0        0        0     2203 2023-06-12 09:30:15.957696 cmem_plugin_kafka-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     4789 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11334 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/LICENSE
+-rw-r--r--   0        0        0     3733 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/README-public.md
+-rw-r--r--   0        0        0        0 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/__init__.py
+-rw-r--r--   0        0        0     4331 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/constants.py
+-rw-r--r--   0        0        0    14787 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/kafka_handlers.py
+-rw-r--r--   0        0        0    12053 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/utils.py
+-rw-r--r--   0        0        0        0 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/__init__.py
+-rw-r--r--   0        0        0    11646 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/consumer.py
+-rw-r--r--   0        0        0     9739 2023-06-20 07:14:18.923375 cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/producer.py
+-rw-r--r--   0        0        0     2206 2023-06-20 07:14:46.663061 cmem_plugin_kafka-1.3.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4792 1970-01-01 00:00:00.000000 cmem_plugin_kafka-1.3.0rc1/PKG-INFO
```

### Comparing `cmem_plugin_kafka-1.3.0/LICENSE` & `cmem_plugin_kafka-1.3.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0/README-public.md` & `cmem_plugin_kafka-1.3.0rc1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/constants.py` & `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -97,19 +97,16 @@
 """
 
 MESSAGE_LIMIT_DESCRIPTION = """
 The maximum number of messages to fetch and process in each run.
 If 0 or less, all messages will be fetched.
 """
 
-ENABLE_AUTO_COMMIT_DESCRIPTION = """
-Automatically and periodically commit offsets in the background.
-
-Note: setting this to false does not prevent the consumer from fetching
-previously committed start offsets.
+DISABLE_COMMIT_DESCRIPTION = """
+Setting this to false will allow the consumer to commit the offset to kafka.
 """
 
 XML_SAMPLE = """
 ```xml
     <?xml version="1.0" encoding="utf-8"?>
     <KafkaMessages>
         <Message>
```

### Comparing `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/kafka_handlers.py` & `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/kafka_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,16 @@
 class KafkaDatasetHandler(KafkaDataHandler, ABC):
     """A Base class for producing messages from Dataset to a Kafka topic."""
 
     def __enter__(self):
         return self.consume_messages()
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        if not exc_val:
+            self._kafka_consumer.commit()
         self._kafka_consumer.close()
 
 
 class KafkaJSONDataHandler(KafkaDatasetHandler):
     """
     A class for producing messages from JSON Dataset to a Kafka topic.
 
@@ -394,14 +396,16 @@
         """Generate the entities from kafka messages"""
         if self._kafka_consumer.get_first_message():
             yield self._get_entity(self._kafka_consumer.get_first_message())
 
         for message in self._kafka_consumer.poll():
             yield self._get_entity(message)
 
+        self._kafka_consumer.commit()
+
     def _get_entity(self, message: KafkaMessage):
         try:
             json_payload = json.loads(message.value)
         except json.decoder.JSONDecodeError as exc:
             raise ValueError("Kafka message in not in valid JSON format") from exc
 
         entity_uri = json_payload["entity"]["uri"]
```

### Comparing `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/utils.py` & `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,30 +98,42 @@
         """Return count of the successful messages"""
         return self._no_of_success_messages
 
 
 class KafkaConsumer:
     """Kafka consumer wrapper over confluent consumer"""
 
+    # pylint: disable=too-many-instance-attributes
     def __init__(
-        self, config: dict, topic: str, log: PluginLogger, context: ExecutionContext
+            self,
+            config: dict,
+            commit_offset: bool,
+            topic: str,
+            log: PluginLogger,
+            context: ExecutionContext
     ):
         """Create consumer instance"""
         self._consumer = Consumer(config)
+        self._commit_offset = commit_offset
         self._context = context
         self._topic = topic
         self._log = log
         self._no_of_success_messages = 0
         self._first_message: Optional[KafkaMessage] = None
         self.fetch_limit = -1
 
     def get_success_messages_count(self) -> int:
         """Return count of the successful messages"""
         return self._no_of_success_messages
 
+    def commit(self):
+        """Commit the latest offset"""
+        if self._commit_offset:
+            self._consumer.commit()
+
     def subscribe(self):
         """Subscribes to a topic to consume messages"""
         self._consumer.subscribe(topics=[self._topic])
 
     def get_first_message(self):
         """Get the first message from kafka subscribed topic"""
         if self._first_message:
```

### Comparing `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/consumer.py` & `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/consumer.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     BOOTSTRAP_SERVERS_DESCRIPTION,
     SECURITY_PROTOCOL_DESCRIPTION,
     SASL_ACCOUNT_DESCRIPTION,
     SASL_PASSWORD_DESCRIPTION,
     CLIENT_ID_DESCRIPTION,
     LOCAL_CONSUMER_QUEUE_MAX_SIZE_DESCRIPTION,
     XML_SAMPLE,
-    JSON_SAMPLE, MESSAGE_LIMIT_DESCRIPTION, ENABLE_AUTO_COMMIT_DESCRIPTION,
+    JSON_SAMPLE, MESSAGE_LIMIT_DESCRIPTION, DISABLE_COMMIT_DESCRIPTION,
 )
 from cmem_plugin_kafka.utils import (
     KafkaConsumer,
     validate_kafka_config,
     get_kafka_statistics,
     get_default_client_id,
     DatasetParameterType,
@@ -170,20 +170,20 @@
             advanced=True,
             param_type=IntParameterType(),
             default_value=100000,
             description=MESSAGE_LIMIT_DESCRIPTION,
         ),
 
         PluginParameter(
-            name="enable_auto_commit",
-            label="Enable Auto Commit",
+            name="disable_commit",
+            label="Disable Commit",
             advanced=True,
             param_type=BoolParameterType(),
-            default_value=True,
-            description=ENABLE_AUTO_COMMIT_DESCRIPTION,
+            default_value=False,
+            description=DISABLE_COMMIT_DESCRIPTION,
         ),
     ],
 )
 class KafkaConsumerPlugin(WorkflowPlugin):
     """Kafka Consumer Plugin"""
 
     # pylint: disable=too-many-instance-attributes
@@ -197,15 +197,15 @@
         sasl_password: str,
         kafka_topic: str,
         auto_offset_reset: str,
         group_id: str = "",
         client_id: str = "",
         local_consumer_queue_size: int = 5000,
         message_limit: int = 100000,
-        enable_auto_commit: bool = True
+        disable_commit: bool = False
     ) -> None:
         if not isinstance(bootstrap_servers, str):
             raise ValueError("Specified server id is invalid")
         self.message_dataset = message_dataset
         self.bootstrap_servers = bootstrap_servers
         self.security_protocol = security_protocol
         self.sasl_mechanisms = sasl_mechanisms
@@ -213,15 +213,15 @@
         self.sasl_password = sasl_password
         self.kafka_topic = kafka_topic
         self.group_id = group_id
         self.auto_offset_reset = auto_offset_reset
         self.client_id = client_id
         self.local_consumer_queue_size = local_consumer_queue_size
         self.message_limit = int(message_limit)
-        self.enable_auto_commit = bool(enable_auto_commit)
+        self.disable_commit = bool(disable_commit)
         self._kafka_stats: dict = {}
 
     def metrics_callback(self, json: str):
         """sends producer metrics to server"""
         self._kafka_stats = get_kafka_statistics(json_data=json)
         for key, value in self._kafka_stats.items():
             self.log.info(f"kafka-stats: {key:10} - {value:10}")
@@ -236,15 +236,15 @@
         """construct and return kafka connection configuration"""
         default_client_id = get_default_client_id(
             project_id=project_id, task_id=task_id
         )
         config = {
             "bootstrap.servers": self.bootstrap_servers,
             "security.protocol": self.security_protocol,
-            "enable.auto.commit": self.enable_auto_commit,
+            "enable.auto.commit": False,
             "auto.offset.reset": self.auto_offset_reset,
             "group.id": self.group_id if self.group_id else default_client_id,
             "client.id": self.client_id if self.client_id else default_client_id,
             "statistics.interval.ms": "1000",
             "queued.max.messages.kbytes": self.local_consumer_queue_size,
             # "stats_cb": self.metrics_callback,
             "error_cb": self.error_callback,
@@ -269,14 +269,15 @@
         self.log.info("Kafka Consumer Started")
         self.validate()
 
         kafka_consumer = KafkaConsumer(
             config=self.get_config(
                 project_id=context.task.project_id(), task_id=context.task.task_id()
             ),
+            commit_offset=not self.disable_commit,
             topic=self.kafka_topic,
             log=self.log,
             context=context,
         )
         kafka_consumer.fetch_limit = self.message_limit
         kafka_consumer.subscribe()
         if not self.message_dataset:
@@ -298,15 +299,14 @@
         # Prefix project id to dataset name
         self.message_dataset = f"{context.task.project_id()}:{self.message_dataset}"
         write_to_dataset(
             dataset_id=self.message_dataset,
             file_resource=handler,
             context=context.user,
         )
-
         context.report.update(
             ExecutionReport(
                 entity_count=kafka_consumer.get_success_messages_count(),
                 operation="read",
                 operation_desc="messages received",
                 summary=list(self._kafka_stats.items()),
             )
```

### Comparing `cmem_plugin_kafka-1.3.0/cmem_plugin_kafka/workflow/producer.py` & `cmem_plugin_kafka-1.3.0rc1/cmem_plugin_kafka/workflow/producer.py`

 * *Files identical despite different names*

### Comparing `cmem_plugin_kafka-1.3.0/pyproject.toml` & `cmem_plugin_kafka-1.3.0rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cmem-plugin-kafka"
-version = "1.3.0"
+version = "1.3.0rc1"
 license = "Apache-2.0"
 description = "Send and receive messages from Apache Kafka."
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Plugins",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `cmem_plugin_kafka-1.3.0/PKG-INFO` & `cmem_plugin_kafka-1.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmem-plugin-kafka
-Version: 1.3.0
+Version: 1.3.0rc1
 Summary: Send and receive messages from Apache Kafka.
 Home-page: https://github.com/eccenca/cmem-plugin-kafka
 License: Apache-2.0
 Keywords: eccenca Corporate Memory,plugin,kafka,kafka-producer,kafka-consumer
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Requires-Python: >=3.9,<4.0
```

