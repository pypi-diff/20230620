# Comparing `tmp/rstream-0.8.1.tar.gz` & `tmp/rstream-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rstream-0.8.1.tar", max compression
+gzip compressed data, was "rstream-0.9.0.tar", max compression
```

## Comparing `rstream-0.8.1.tar` & `rstream-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1074 2023-06-16 14:04:37.011220 rstream-0.8.1/LICENSE
--rw-r--r--   0        0        0     9792 2023-06-16 14:04:37.011220 rstream-0.8.1/README.md
--rw-r--r--   0        0        0      734 2023-06-16 14:04:37.011220 rstream-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     1077 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/__init__.py
--rw-r--r--   0        0        0      651 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/amqp.py
--rw-r--r--   0        0        0    18240 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/client.py
--rw-r--r--   0        0        0     4883 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/compression.py
--rw-r--r--   0        0        0     2117 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/connection.py
--rw-r--r--   0        0        0      928 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/constants.py
--rw-r--r--   0        0        0     8590 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/consumer.py
--rw-r--r--   0        0        0     5638 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/encoding.py
--rw-r--r--   0        0        0     1364 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/exceptions.py
--rw-r--r--   0        0        0    15804 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/producer.py
--rw-r--r--   0        0        0    16111 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/schema.py
--rw-r--r--   0        0        0     2434 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/superstream.py
--rw-r--r--   0        0        0     5637 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/superstream_consumer.py
--rw-r--r--   0        0        0     4372 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/superstream_producer.py
--rw-r--r--   0        0        0      950 2023-06-16 14:04:37.011220 rstream-0.8.1/rstream/utils.py
--rw-r--r--   0        0        0    10502 1970-01-01 00:00:00.000000 rstream-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-20 13:41:50.047564 rstream-0.9.0/LICENSE
+-rw-r--r--   0        0        0    12325 2023-06-20 13:41:50.047564 rstream-0.9.0/README.md
+-rw-r--r--   0        0        0      734 2023-06-20 13:41:50.051564 rstream-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1304 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/__init__.py
+-rw-r--r--   0        0        0      651 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/amqp.py
+-rw-r--r--   0        0        0    18240 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/client.py
+-rw-r--r--   0        0        0     4883 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/compression.py
+-rw-r--r--   0        0        0     2117 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/connection.py
+-rw-r--r--   0        0        0      928 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/constants.py
+-rw-r--r--   0        0        0     8746 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/consumer.py
+-rw-r--r--   0        0        0     5638 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/encoding.py
+-rw-r--r--   0        0        0     1364 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/exceptions.py
+-rw-r--r--   0        0        0    15804 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/producer.py
+-rw-r--r--   0        0        0    16111 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/schema.py
+-rw-r--r--   0        0        0     2611 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/superstream.py
+-rw-r--r--   0        0        0     5637 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/superstream_consumer.py
+-rw-r--r--   0        0        0     4372 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/superstream_producer.py
+-rw-r--r--   0        0        0      950 2023-06-20 13:41:50.051564 rstream-0.9.0/rstream/utils.py
+-rw-r--r--   0        0        0    13035 1970-01-01 00:00:00.000000 rstream-0.9.0/PKG-INFO
```

### Comparing `rstream-0.8.1/LICENSE` & `rstream-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/README.md` & `rstream-0.9.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -170,23 +170,103 @@
         password='guest',
     )
 
     loop = asyncio.get_event_loop()
     loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
 
     def on_message(msg: AMQPMessage, message_context: MessageContext):
-        print('Got message: {}'.format(msg) + "from stream " + message_context.stream+ "offset: " + str(message_context.offset))
+        consumer = message_context.consumer
+        stream = await message_context.consumer.stream(message_context.subscriber_name)
+        offset = message_context.offset
+    
+    print('Got message: {}'.format(msg) + "from stream " + stream+ "offset: " + str(offset))
 
     await consumer.start()
     await consumer.subscribe('mystream', on_message, decoder=amqp_decoder)
     await consumer.run()
 
 asyncio.run(consume())
 ```
 
+### Server-side offset tracking
+
+RabbitMQ Streams provides server-side offset tracking for consumers. This features allows a consuming application to restart consuming where it left off in a previous run.
+You can use the store_offset (to store an offset in the server) and query_offset (to query it) methods of the consumer class like in this example:
+
+```python
+cont = 0
+lock = asyncio.Lock()
+
+async def on_message(msg: AMQPMessage, message_context: MessageContext):
+
+    global cont
+    global lock
+
+    consumer = message_context.consumer
+    stream = await message_context.consumer.stream(message_context.subscriber_name)
+    offset = message_context.offset
+    
+    print('Got message: {}'.format(msg) + "from stream " + stream+ "offset: " + str(offset))
+
+    # store the offset every 1000 messages received
+    async with lock:
+        cont = cont+1
+        # store the offset every 1000 messages received
+        if (cont % 1000 == 0):
+            await consumer.store_offset(stream=stream, offset=offset, subscriber_name=message_context.subscriber_name)
+
+async def consume():
+
+    consumer = Consumer  (
+    host='localhost',
+    port=5552,
+        vhost='/',
+        username='guest',
+        password='guest',
+    )
+
+    loop = asyncio.get_event_loop()
+    loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
+
+    await consumer.start()
+    # Take back the server stored offset
+    try: 
+        my_offset = await consumer.query_offset(stream="mixing", subscriber_name="subscriber_1")
+    # catch exceptions if stream or offset for the subscriber name doesn't exist
+    except OffsetNotFound as offset_exception:
+        print(f"ValueError: {offset_exception}")
+        exit(1)
+    
+    except StreamDoesNotExist as stream_exception:
+        print(f"ValueError: {stream_exception}")
+        exit(1)
+         
+    except ServerError as e:
+        print(f"ValueError: {e}")
+        exit(1)
+   
+    await consumer.subscribe(stream='mixing', subscriber_name='subscriber-1', callback=on_message, decoder=amqp_decoder, offset_type=OffsetType.OFFSET, offset=my_offset)
+    await consumer.run()
+
+# main coroutine
+async def main():
+    # schedule the task
+    task = asyncio.create_task(consume())
+
+    # wait a moment
+    await asyncio.sleep(5)
+    # cancel the task
+    was_cancelled = task.cancel()
+ 
+# run the asyncio program
+asyncio.run(main())
+```
+
+
+
 ### Superstreams
 
 The client is also supporting superstream: https://blog.rabbitmq.com/posts/2022/07/rabbitmq-3-11-feature-preview-super-streams/
 A super stream is a logical stream made of individual, regular streams. It is a way to scale out publishing and consuming with RabbitMQ Streams: a large logical stream is divided into partition streams, splitting up the storage and the traffic on several cluster nodes.
 
 You can use superstream_producer and superstream_consumer classes which internally uses producers and consumers to operate on the componsing streams.
```

### Comparing `rstream-0.8.1/pyproject.toml` & `rstream-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rstream"
-version = "0.8.1"
+version = "0.9.0"
 description = "A python client for RabbitMQ Streams"
 authors = ["George Fortunatov <qweeeze@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/qweeze/rstream"
 repository = "https://github.com/qweeze/rstream"
 license = "MIT"
```

### Comparing `rstream-0.8.1/rstream/amqp.py` & `rstream-0.9.0/rstream/amqp.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/client.py` & `rstream-0.9.0/rstream/client.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/compression.py` & `rstream-0.9.0/rstream/compression.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/connection.py` & `rstream-0.9.0/rstream/connection.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/constants.py` & `rstream-0.9.0/rstream/constants.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/consumer.py` & `rstream-0.9.0/rstream/consumer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,16 @@
 
 MT = TypeVar("MT")
 CB = Annotated[Callable[[MT, Any], Union[None, Awaitable[None]]], "Message callback type"]
 
 
 @dataclass
 class MessageContext:
-    stream: str
+    consumer: Consumer
+    subscriber_name: str
     offset: int
     timestamp: int
 
 
 @dataclass
 class _Subscriber:
     stream: str
@@ -97,15 +98,15 @@
         self._stop_event.set()
 
     async def close(self) -> None:
         self.stop()
 
         for subscriber in list(self._subscribers.values()):
             await self.unsubscribe(subscriber.reference)
-            await self.store_offset(subscriber.stream, subscriber.reference, subscriber.offset)
+            # await self.store_offset(subscriber.stream, subscriber.reference, subscriber.offset)
 
         self._subscribers.clear()
 
         await self._pool.close()
         self._clients.clear()
         self._default_client = None
 
@@ -229,17 +230,19 @@
 
     async def _on_deliver(self, frame: schema.Deliver, subscriber: _Subscriber) -> None:
         if frame.subscription_id != subscriber.subscription_id:
             return
 
         await subscriber.client.credit(subscriber.subscription_id, 1)
         offset = frame.chunk_first_offset
+
         for index, message in enumerate(self._filter_messages(frame, subscriber)):
             offset = offset + index
-            message_context = MessageContext(subscriber.stream, offset, frame.timestamp)
+            message_context = MessageContext(self, subscriber.reference, offset, frame.timestamp)
+
             maybe_coro = subscriber.callback(subscriber.decoder(message), message_context)
             if maybe_coro is not None:
                 await maybe_coro
 
     async def create_stream(
         self,
         stream: str,
@@ -261,7 +264,11 @@
             await self.default_client.delete_stream(stream)
         except exceptions.StreamDoesNotExist:
             if not missing_ok:
                 raise
 
     async def stream_exists(self, stream: str) -> bool:
         return await self.default_client.stream_exists(stream)
+
+    async def stream(self, subscriber_name) -> str:
+
+        return self._subscribers[subscriber_name].stream
```

### Comparing `rstream-0.8.1/rstream/encoding.py` & `rstream-0.9.0/rstream/encoding.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/exceptions.py` & `rstream-0.9.0/rstream/exceptions.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/producer.py` & `rstream-0.9.0/rstream/producer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/schema.py` & `rstream-0.9.0/rstream/schema.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/superstream.py` & `rstream-0.9.0/rstream/superstream.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,26 +29,31 @@
         pass
 
 
 class DefaultSuperstreamMetadata(Metadata):
     def __init__(self, super_stream: str, client: Client):
         self.super_stream = super_stream
         self.client = client
+        self._partitions: list[str] = []
+        self._routes: list[str] = []
 
     async def partitions(self) -> list[str]:
-        self._partitions = await self.client.partitions(self.super_stream)
-        if len(self._partitions) <= 0:
-            raise ValueError(
-                "the number of partitions of the stream is less or equal to 0, the superstream doesn't probably exist"
-            )
+        if len(self._partitions) == 0:
+            self._partitions = await self.client.partitions(self.super_stream)
+            if len(self._partitions) <= 0:
+                raise ValueError(
+                    "the number of partitions of the stream is <= to 0, the superstream doesn't probably exist"
+                )
+
         return self._partitions
 
     async def routes(self, routing_key: str) -> list[str]:
-        self.route = await self.client.route(routing_key, self.super_stream)
-        return self.route
+        if len(self._routes) == 0:
+            self._routes = await self.client.route(routing_key, self.super_stream)
+        return self._routes
 
 
 class RoutingStrategy(abc.ABC):
     async def route(self, message: MessageT, metadata: Metadata) -> list[str]:
         pass
 
 
@@ -62,19 +67,20 @@
 
 
 class HashRoutingMurmurStrategy(RoutingStrategy):
     def __init__(self, routingKeyExtractor: CB[Any]):
         self.routingKeyExtractor: CB[Any] = routingKeyExtractor
 
     async def route(self, message: MessageT, metadata: Metadata) -> list[str]:
+
         streams = []
         key = await self.routingKeyExtractor(message)
         key_bytes = bytes(key, "UTF-16")
         hash = mmh3.hash_bytes(key_bytes, 104729)
-        partitions = len(await metadata.partitions())
+        number_of_partitions = len(await metadata.partitions())
 
-        route = int.from_bytes(hash, "little", signed=False) % partitions
-        stream_partitions = await metadata.partitions()
-        stream = stream_partitions[route]
+        route = int.from_bytes(hash, "little", signed=False) % number_of_partitions
+        partitions = await metadata.partitions()
+        stream = partitions[route]
         streams.append(stream)
 
         return streams
```

### Comparing `rstream-0.8.1/rstream/superstream_consumer.py` & `rstream-0.9.0/rstream/superstream_consumer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/superstream_producer.py` & `rstream-0.9.0/rstream/superstream_producer.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/rstream/utils.py` & `rstream-0.9.0/rstream/utils.py`

 * *Files identical despite different names*

### Comparing `rstream-0.8.1/PKG-INFO` & `rstream-0.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rstream
-Version: 0.8.1
+Version: 0.9.0
 Summary: A python client for RabbitMQ Streams
 Home-page: https://github.com/qweeze/rstream
 License: MIT
 Author: George Fortunatov
 Author-email: qweeeze@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -190,23 +190,103 @@
         password='guest',
     )
 
     loop = asyncio.get_event_loop()
     loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
 
     def on_message(msg: AMQPMessage, message_context: MessageContext):
-        print('Got message: {}'.format(msg) + "from stream " + message_context.stream+ "offset: " + str(message_context.offset))
+        consumer = message_context.consumer
+        stream = await message_context.consumer.stream(message_context.subscriber_name)
+        offset = message_context.offset
+    
+    print('Got message: {}'.format(msg) + "from stream " + stream+ "offset: " + str(offset))
 
     await consumer.start()
     await consumer.subscribe('mystream', on_message, decoder=amqp_decoder)
     await consumer.run()
 
 asyncio.run(consume())
 ```
 
+### Server-side offset tracking
+
+RabbitMQ Streams provides server-side offset tracking for consumers. This features allows a consuming application to restart consuming where it left off in a previous run.
+You can use the store_offset (to store an offset in the server) and query_offset (to query it) methods of the consumer class like in this example:
+
+```python
+cont = 0
+lock = asyncio.Lock()
+
+async def on_message(msg: AMQPMessage, message_context: MessageContext):
+
+    global cont
+    global lock
+
+    consumer = message_context.consumer
+    stream = await message_context.consumer.stream(message_context.subscriber_name)
+    offset = message_context.offset
+    
+    print('Got message: {}'.format(msg) + "from stream " + stream+ "offset: " + str(offset))
+
+    # store the offset every 1000 messages received
+    async with lock:
+        cont = cont+1
+        # store the offset every 1000 messages received
+        if (cont % 1000 == 0):
+            await consumer.store_offset(stream=stream, offset=offset, subscriber_name=message_context.subscriber_name)
+
+async def consume():
+
+    consumer = Consumer  (
+    host='localhost',
+    port=5552,
+        vhost='/',
+        username='guest',
+        password='guest',
+    )
+
+    loop = asyncio.get_event_loop()
+    loop.add_signal_handler(signal.SIGINT, lambda: asyncio.create_task(consumer.close()))
+
+    await consumer.start()
+    # Take back the server stored offset
+    try: 
+        my_offset = await consumer.query_offset(stream="mixing", subscriber_name="subscriber_1")
+    # catch exceptions if stream or offset for the subscriber name doesn't exist
+    except OffsetNotFound as offset_exception:
+        print(f"ValueError: {offset_exception}")
+        exit(1)
+    
+    except StreamDoesNotExist as stream_exception:
+        print(f"ValueError: {stream_exception}")
+        exit(1)
+         
+    except ServerError as e:
+        print(f"ValueError: {e}")
+        exit(1)
+   
+    await consumer.subscribe(stream='mixing', subscriber_name='subscriber-1', callback=on_message, decoder=amqp_decoder, offset_type=OffsetType.OFFSET, offset=my_offset)
+    await consumer.run()
+
+# main coroutine
+async def main():
+    # schedule the task
+    task = asyncio.create_task(consume())
+
+    # wait a moment
+    await asyncio.sleep(5)
+    # cancel the task
+    was_cancelled = task.cancel()
+ 
+# run the asyncio program
+asyncio.run(main())
+```
+
+
+
 ### Superstreams
 
 The client is also supporting superstream: https://blog.rabbitmq.com/posts/2022/07/rabbitmq-3-11-feature-preview-super-streams/
 A super stream is a logical stream made of individual, regular streams. It is a way to scale out publishing and consuming with RabbitMQ Streams: a large logical stream is divided into partition streams, splitting up the storage and the traffic on several cluster nodes.
 
 You can use superstream_producer and superstream_consumer classes which internally uses producers and consumers to operate on the componsing streams.
```

