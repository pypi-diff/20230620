# Comparing `tmp/elefantolib_events-0.4.0.tar.gz` & `tmp/elefantolib_events-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elefantolib_events-0.4.0.tar", max compression
+gzip compressed data, was "elefantolib_events-0.5.0.tar", max compression
```

## Comparing `elefantolib_events-0.4.0.tar` & `elefantolib_events-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-06-19 15:45:11.051061 elefantolib_events-0.4.0/LICENSE
--rw-r--r--   0        0        0        0 2023-06-19 15:45:11.051061 elefantolib_events-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-06-19 15:45:11.051061 elefantolib_events-0.4.0/elefantolib_events/__init__.py
--rw-r--r--   0        0        0      733 2023-06-19 15:45:11.051061 elefantolib_events-0.4.0/elefantolib_events/emitter.py
--rw-r--r--   0        0        0      938 2023-06-19 15:45:11.051061 elefantolib_events-0.4.0/elefantolib_events/listener.py
--rw-r--r--   0        0        0      336 2023-06-19 15:45:22.911455 elefantolib_events-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 elefantolib_events-0.4.0/setup.py
--rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 elefantolib_events-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/LICENSE
+-rw-r--r--   0        0        0        0 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/elefantolib_events/__init__.py
+-rw-r--r--   0        0        0      765 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/elefantolib_events/emitter.py
+-rw-r--r--   0        0        0     1071 2023-06-20 14:37:53.655186 elefantolib_events-0.5.0/elefantolib_events/listener.py
+-rw-r--r--   0        0        0      336 2023-06-20 14:38:04.671449 elefantolib_events-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      605 1970-01-01 00:00:00.000000 elefantolib_events-0.5.0/setup.py
+-rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 elefantolib_events-0.5.0/PKG-INFO
```

### Comparing `elefantolib_events-0.4.0/LICENSE` & `elefantolib_events-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elefantolib_events-0.4.0/elefantolib_events/emitter.py` & `elefantolib_events-0.5.0/elefantolib_events/emitter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import json
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 
 import aio_pika
-from aio_pika.abc import AbstractRobustConnection
+from aio_pika.abc import DeliveryMode, ExchangeType
 
 
 @dataclass(slots=True)
 class Emitter:
     rabbitmq_url: str
-    connection: AbstractRobustConnection = field(init=False, default=None)
-
-    async def run(self):
-        self.connection = await aio_pika.connect_robust(self.rabbitmq_url)
 
     async def emit(self, event_name: str, payload: dict) -> None:
-        if not self.connection:
-            await self.run()
-
-        channel = await self.connection.channel()
+        connection = await aio_pika.connect(self.rabbitmq_url)
 
-        body = json.dumps(payload, default=str)
-        await channel.default_exchange.publish(
-            aio_pika.Message(body=str.encode(body)),
-            routing_key=event_name,
-        )
+        async with connection:
+            channel = await connection.channel()
+            await channel.declare_queue(event_name)
+
+            exchange = await channel.declare_exchange(event_name, ExchangeType.TOPIC)
+            body = json.dumps(payload, default=str)
+            await exchange.publish(
+                aio_pika.Message(body=str.encode(body), delivery_mode=DeliveryMode.PERSISTENT),
+                routing_key=event_name,
+            )
```

### Comparing `elefantolib_events-0.4.0/elefantolib_events/listener.py` & `elefantolib_events-0.5.0/elefantolib_events/listener.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 import asyncio
 import json
 
 import aio_pika
+from aio_pika import ExchangeType
 
 
-class ConnectionPool:
+class Listener:
     def __init__(self, url, pool_size=10):
         self.rabbitmq_url = url
         self.pool_size = pool_size
         self._connections = asyncio.Queue()
 
     async def initialize(self):
         for _ in range(self.pool_size):
             connection = await aio_pika.connect_robust(self.rabbitmq_url)
             await self._connections.put(connection)
 
-    async def listen(self, queue_name, fn):
-        new_connection = await self._connections.get()
+    async def listen(self, event_name, fn):
+        connection = await self._connections.get()
 
-        async with new_connection as connection:
+        async with connection:
             channel = await connection.channel()
-            queue = await channel.declare_queue(queue_name)
+            queue = await channel.declare_queue(event_name)
+            exchange = await channel.declare_exchange(event_name, ExchangeType.TOPIC)
+
+            await queue.bind(exchange)
+
             async with queue.iterator() as queue_iter:
                 async for message in queue_iter:
                     async with message.process():
                         data = json.loads(message.body.decode())
                         await fn(data)
```

### Comparing `elefantolib_events-0.4.0/setup.py` & `elefantolib_events-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aio-pika>=9.1.2,<10.0.0']
 
 setup_kwargs = {
     'name': 'elefantolib-events',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
     'long_description': '',
     'author': 'Aibar',
     'author_email': 'bekaybar@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

