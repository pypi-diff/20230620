# Comparing `tmp/oxalis-0.6.3.tar.gz` & `tmp/oxalis-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxalis-0.6.3.tar", max compression
+gzip compressed data, was "oxalis-0.6.4.tar", max compression
```

## Comparing `oxalis-0.6.3.tar` & `oxalis-0.6.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.3/LICENSE
--rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.3/README.md
--rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.3/oxalis/__init__.py
--rw-r--r--   0        0        0    11619 2023-06-15 05:50:52.211402 oxalis-0.6.3/oxalis/amqp.py
--rw-r--r--   0        0        0     7314 2023-06-15 05:41:22.005127 oxalis-0.6.3/oxalis/base.py
--rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.6.3/oxalis/beater.py
--rw-r--r--   0        0        0     5917 2023-06-14 07:44:58.843783 oxalis-0.6.3/oxalis/kafka.py
--rw-r--r--   0        0        0     3542 2023-06-15 05:41:58.004260 oxalis-0.6.3/oxalis/pool.py
--rw-r--r--   0        0        0     7448 2023-05-12 06:41:48.719578 oxalis-0.6.3/oxalis/redis.py
--rw-r--r--   0        0        0      884 2023-06-15 05:50:57.851266 oxalis-0.6.3/pyproject.toml
--rw-r--r--   0        0        0     7653 1970-01-01 00:00:00.000000 oxalis-0.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-06-07 12:05:40.532331 oxalis-0.6.4/LICENSE
+-rw-r--r--   0        0        0     6896 2023-04-20 05:15:02.504528 oxalis-0.6.4/README.md
+-rw-r--r--   0        0        0       22 2022-06-03 10:29:06.678568 oxalis-0.6.4/oxalis/__init__.py
+-rw-r--r--   0        0        0    11619 2023-06-15 05:51:44.478143 oxalis-0.6.4/oxalis/amqp.py
+-rw-r--r--   0        0        0     7314 2023-06-15 05:41:22.005127 oxalis-0.6.4/oxalis/base.py
+-rw-r--r--   0        0        0     1978 2023-04-28 02:27:00.905636 oxalis-0.6.4/oxalis/beater.py
+-rw-r--r--   0        0        0     7717 2023-06-20 07:00:16.938574 oxalis-0.6.4/oxalis/kafka.py
+-rw-r--r--   0        0        0     3542 2023-06-15 05:41:58.004260 oxalis-0.6.4/oxalis/pool.py
+-rw-r--r--   0        0        0     7448 2023-05-12 06:41:48.719578 oxalis-0.6.4/oxalis/redis.py
+-rw-r--r--   0        0        0      884 2023-06-20 06:58:30.369161 oxalis-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0     7653 1970-01-01 00:00:00.000000 oxalis-0.6.4/PKG-INFO
```

### Comparing `oxalis-0.6.3/LICENSE` & `oxalis-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/README.md` & `oxalis-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/oxalis/amqp.py` & `oxalis-0.6.4/oxalis/amqp.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/oxalis/base.py` & `oxalis-0.6.4/oxalis/base.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/oxalis/beater.py` & `oxalis-0.6.4/oxalis/beater.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/oxalis/kafka.py` & `oxalis-0.6.4/oxalis/kafka.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
 import asyncio
-import contextlib
 import typing as tp
 
 import aiokafka
 
 from .base import PARAM, RT
 from .base import Oxalis as _Oxalis
 from .base import Task as _Task
@@ -18,18 +17,20 @@
 class Topic:
     def __init__(
         self,
         name: str,
         consumer_count: int = 3,
         pause: bool = False,
         enable_auto_commit: bool = True,
+        batch_count: int = 1,
         **consumer_kwargs: tp.Any,
     ) -> None:
         self.name = name
         self.consumer_count = consumer_count
+        self.batch_count = batch_count
         self.pause = pause
         self.enable_auto_commit = enable_auto_commit
         self.consumer_kwargs = consumer_kwargs
 
     def __hash__(self) -> int:
         return hash(self.name)
 
@@ -141,48 +142,96 @@
             )
             self.register_task(task)
             self.topics.add(topic)
             return task
 
         return wrapped
 
+    async def _consume(self, message: aiokafka.ConsumerRecord):
+        await self.on_message_receive(message.value)
+        return message
+
+    async def _batch_consume(
+        self,
+        topic: Topic,
+        consumer: aiokafka.AIOKafkaConsumer,
+        messages: tp.List[aiokafka.ConsumerRecord],
+    ):
+        offsets = sorted([msg.offset for msg in messages])
+        assert offsets
+        consumed_offsets = set()
+        committed_offsets: tp.Set[int] = set()
+        offset_index = 0
+        for cor in asyncio.as_completed(
+            [self._consume(message) for message in messages]
+        ):
+            msg: aiokafka.ConsumerRecord = await cor
+            consumed_offsets.add(msg.offset)
+            # commit minimum consumed message offset
+            if not topic.enable_auto_commit:
+                while (
+                    offset_index < len(offsets)
+                    and offsets[offset_index] in consumed_offsets
+                ):
+                    offset_index += 1
+                offset_index = offset_index - 1
+                if offset_index < 0:
+                    continue
+
+                offset = offsets[offset_index]
+                if offset in committed_offsets:
+                    continue
+                try:
+                    await consumer.commit(
+                        {aiokafka.TopicPartition(msg.topic, msg.partition): offset + 1}
+                    )
+                    committed_offsets.add(offset)
+                except Exception as e:
+                    logger.warning(
+                        f"Topic<{msg.topic}> commit offset<{offset}> failed: {e}"
+                    )
+
     async def _start_consumer(self, topic: Topic):
         self.consuming_count += 1
         consumer = aiokafka.AIOKafkaConsumer(
             topic.name,
             bootstrap_servers=self.kafka_url,
             group_id=self.group,
             enable_auto_commit=topic.enable_auto_commit,
             **topic.consumer_kwargs,
         )
+        pool = Pool(concurrency=-1, timeout=None)
         self.consumers.append(consumer)
+        self.pools.append(pool)
         consumer_started = False
         try:
             await consumer.start()
             consumer_started = True
             await asyncio.sleep(
                 self.timeout
             )  # wait for rebalancing when boost same topic's consumer in same time
             while self.running:
-                with contextlib.suppress(asyncio.TimeoutError):
-                    msg = await asyncio.wait_for(
-                        consumer.getone(), timeout=self.timeout
-                    )
+                data = await consumer.getmany(
+                    max_records=topic.batch_count, timeout_ms=self.timeout * 100
+                )
+                if not data:
+                    if pool.done and topic.pause:
+                        consumer.resume(*consumer.assignment())
+                else:
+                    cors = [
+                        self._batch_consume(topic, consumer, msgs)
+                        for _, msgs in data.items()
+                    ]
                     if topic.pause:
+                        assert pool.done  # in case
                         consumer.pause(*consumer.assignment())
-                    await self.on_message_receive(msg.value)
-                    if topic.pause:
-                        consumer.resume(*consumer.assignment())
-                    if not topic.enable_auto_commit:
-                        try:
-                            await consumer.commit()
-                        except Exception as e:
-                            logger.warning(
-                                f"Topic<{topic}> Commit <{consumer.assignment()}> failed: {e}"
-                            )
+                        for cor in cors:
+                            pool.spawn(cor)
+                    else:
+                        await asyncio.wait([asyncio.ensure_future(cor) for cor in cors])
         except Exception as e:
             self.health = False
             raise e from None
         finally:
             if consumer_started:
                 await asyncio.sleep(self.timeout)  # wait for committing
                 await consumer.stop()
```

### Comparing `oxalis-0.6.3/oxalis/pool.py` & `oxalis-0.6.4/oxalis/pool.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/oxalis/redis.py` & `oxalis-0.6.4/oxalis/redis.py`

 * *Files identical despite different names*

### Comparing `oxalis-0.6.3/pyproject.toml` & `oxalis-0.6.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxalis"
-version = "0.6.3"
+version = "0.6.4"
 description = "Distributed async task/job queue"
 authors = ["strongbugman <strongbugman@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     "Environment :: Console",
     "Programming Language :: Python :: 3.10",
```

### Comparing `oxalis-0.6.3/PKG-INFO` & `oxalis-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxalis
-Version: 0.6.3
+Version: 0.6.4
 Summary: Distributed async task/job queue
 License: MIT
 Author: strongbugman
 Author-email: strongbugman@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
```

