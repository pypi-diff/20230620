# Comparing `tmp/amqp_mqtt_transport-0.1.5.tar.gz` & `tmp/amqp_mqtt_transport-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amqp_mqtt_transport-0.1.5.tar", last modified: Tue Jun 20 19:29:10 2023, max compression
+gzip compressed data, was "amqp_mqtt_transport-0.1.6.tar", last modified: Tue Jun 20 20:54:33 2023, max compression
```

## Comparing `amqp_mqtt_transport-0.1.5.tar` & `amqp_mqtt_transport-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/
--rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp_mqtt_transport-0.1.5/.gitattributes
--rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp_mqtt_transport-0.1.5/.gitignore
--rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp_mqtt_transport-0.1.5/LICENSE
--rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp_mqtt_transport-0.1.5/Makefile
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/PKG-INFO
--rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp_mqtt_transport-0.1.5/README.md
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.461011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/
--rw-rw-r--   0 igor      (1001) igor      (1001)      146 2023-06-19 12:15:25.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      956 2023-06-19 12:15:26.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/abc.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/
--rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1728 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/consumer.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     5533 2023-06-19 12:15:29.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     1521 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2102 2023-06-19 12:15:26.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/message_scheduler.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/
--rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/__init__.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     3115 2023-06-19 12:15:31.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/controller.py
--rw-rw-r--   0 igor      (1001) igor      (1001)      807 2023-06-19 12:15:32.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/publisher.py
--rw-rw-r--   0 igor      (1001) igor      (1001)     2430 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/scheduled_publisher.py
-drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 19:29:10.461011 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/
--rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/PKG-INFO
--rw-rw-r--   0 igor      (1001) igor      (1001)      698 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/SOURCES.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/dependency_links.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       65 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/requires.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)       20 2023-06-20 19:29:10.000000 amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/top_level.txt
--rw-rw-r--   0 igor      (1001) igor      (1001)      758 2023-06-20 19:27:50.000000 amqp_mqtt_transport-0.1.5/pyproject.toml
--rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-20 19:29:10.465011 amqp_mqtt_transport-0.1.5/setup.cfg
--rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp_mqtt_transport-0.1.5/setup.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 20:54:33.803720 amqp_mqtt_transport-0.1.6/
+-rw-r--r--   0 igor      (1001) igor      (1001)       87 2023-06-19 12:04:53.000000 amqp_mqtt_transport-0.1.6/.gitattributes
+-rw-r--r--   0 igor      (1001) igor      (1001)      483 2023-06-19 12:04:52.000000 amqp_mqtt_transport-0.1.6/.gitignore
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1072 2023-06-19 12:17:58.000000 amqp_mqtt_transport-0.1.6/LICENSE
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1054 2023-06-19 13:51:37.000000 amqp_mqtt_transport-0.1.6/Makefile
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 20:54:33.803720 amqp_mqtt_transport-0.1.6/PKG-INFO
+-rw-r--r--   0 igor      (1001) igor      (1001)      788 2023-06-19 13:04:30.000000 amqp_mqtt_transport-0.1.6/README.md
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 20:54:33.795719 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/
+-rw-rw-r--   0 igor      (1001) igor      (1001)      152 2023-06-20 19:34:21.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      941 2023-06-20 20:42:25.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/abc.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 20:54:33.799720 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       75 2023-06-19 12:15:27.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1738 2023-06-20 19:43:16.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/consumer.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     5549 2023-06-20 20:39:00.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1532 2023-06-20 20:39:25.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2146 2023-06-20 20:41:28.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/message_scheduler.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 20:54:33.799720 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/mqtt/
+-rw-rw-r--   0 igor      (1001) igor      (1001)       51 2023-06-19 12:15:30.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/mqtt/__init__.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     3127 2023-06-20 20:39:47.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/mqtt/controller.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)      818 2023-06-20 20:40:10.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/mqtt/publisher.py
+-rw-rw-r--   0 igor      (1001) igor      (1001)     2450 2023-06-20 20:41:01.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/scheduled_publisher.py
+drwxrwxr-x   0 igor      (1001) igor      (1001)        0 2023-06-20 20:54:33.795719 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/
+-rw-rw-r--   0 igor      (1001) igor      (1001)     1255 2023-06-20 20:54:33.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/PKG-INFO
+-rw-rw-r--   0 igor      (1001) igor      (1001)      698 2023-06-20 20:54:33.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/SOURCES.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)        1 2023-06-20 20:54:33.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/dependency_links.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       65 2023-06-20 20:54:33.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/requires.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)       20 2023-06-20 20:54:33.000000 amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/top_level.txt
+-rw-rw-r--   0 igor      (1001) igor      (1001)      758 2023-06-20 20:53:22.000000 amqp_mqtt_transport-0.1.6/pyproject.toml
+-rw-rw-r--   0 igor      (1001) igor      (1001)       38 2023-06-20 20:54:33.803720 amqp_mqtt_transport-0.1.6/setup.cfg
+-rw-rw-r--   0 igor      (1001) igor      (1001)       37 2023-06-19 12:41:38.000000 amqp_mqtt_transport-0.1.6/setup.py
```

### Comparing `amqp_mqtt_transport-0.1.5/LICENSE` & `amqp_mqtt_transport-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.5/Makefile` & `amqp_mqtt_transport-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.5/PKG-INFO` & `amqp_mqtt_transport-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp_mqtt_transport
-Version: 0.1.5
+Version: 0.1.6
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp_mqtt_transport-0.1.5/README.md` & `amqp_mqtt_transport-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/abc.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/abc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import abc
-import logging
 import typing
 
 __all__ = ['Controller']
 
 
 class Controller(abc.ABC):
     @abc.abstractmethod
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/consumer.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/consumer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from . import AMQPController, BindingsParams, QueueParams, ExchangeParams, setup_queue
 import typing
 import logging
 import aio_pika
-import transport.abc
+from amqp_mqtt_transport.abc import Consumer
 
 __all__ = ['AMQPConsumer']
 logger = logging.getLogger(__name__)
 
 
-class AMQPConsumer(transport.abc.Consumer):
+class AMQPConsumer(Consumer):
     def __init__(self, channel: aio_pika.abc.AbstractChannel):
         self._channel = channel
 
     @property
     def queue_name(self) -> str:
         return self._binding_params.queue_params.name
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/controller.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 import tenacity
 import tenacity.stop
 import tenacity.wait
 import functools
 import typing
-import transport.abc
+from amqp_mqtt_transport.abc import Controller
 
 
 __all__ = [
     'AMQPController',
     'ConnectionParams',
     'ExchangeParams',
     'QueueParams',
@@ -65,15 +65,15 @@
             except Exception as e:
                 manager.close()
                 raise e
         return wrapped
     return wrapper
 
 
-class AMQPController(transport.abc.Controller):
+class AMQPController(abc.Controller):
     def __init__(self, connection_params: ConnectionParams):
         self._host = connection_params.host
         self._port = connection_params.port
         self._login = connection_params.login
         self._password = connection_params.password
         self._virtual_host = connection_params.virtual_host
         self._ssl: bool = connection_params.ssl
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/amqp/publisher.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/amqp/publisher.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import aio_pika
 from typing import Union
-import transport.abc
+from amqp_mqtt_transport.abc import Publisher
 import logging
 import aiormq.abc
 from . import AMQPController, BindingsParams, QueueParams, ExchangeParams, setup_queue
 
 __all__ = ['AMQPPublisher']
 logger = logging.getLogger(__name__)
 
 
-class AMQPPublisher(transport.abc.Publisher):
+class AMQPPublisher(Publisher):
     def __init__(self, connection: AMQPController, channel: aio_pika.abc.AbstractChannel):
         self._connection = connection
         self._channel = channel
 
     @property
     def queue_params(self) -> QueueParams:
         return self._q_param
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/message_scheduler.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/message_scheduler.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 
 import logging
 import typing
-import transport
+import amqp_mqtt_transport.abc
 import asyncio
 
 __all__ = ['MessageSheduler']
 logger = logging.getLogger(__name__)
 
 
 class ScheduledPublisherWrapper(typing.NamedTuple):
     """Basic data struct to hold ScheduledPublisher instance with future assigned to it"""
     id: str
-    scheduled_publisher: transport.ScheduledPublisher
+    scheduled_publisher: amqp_mqtt_transport.ScheduledPublisher
     task: asyncio.Task
 
 
 class MessageSheduler():
     """Class manager for list of amqp_controller.ScheduledPublisher
     """
 
     def __init__(self) -> None:
         self._publishers: typing.Dict[str, ScheduledPublisherWrapper] = {}
 
     async def add_sheduled_publisher(self, id: str,
                                      messages: typing.List[typing.Dict],
                                      interval_seconds: float,
-                                     publisher: transport.abc.Publisher,
+                                     publisher: amqp_mqtt_transport.abc.Publisher,
                                      delay_seconds: float = 0,
                                      stop_after_n_runs: int = -1):
         if id in self._publishers:
             logger.error(f'Publisher with id={id} already exists')
             return
-        sh_publisher = transport.ScheduledPublisher(publisher)
+        sh_publisher = amqp_mqtt_transport.ScheduledPublisher(publisher)
         for msg in messages:
             sh_publisher.add_message_to_list(msg)
         sh_publisher.interval_seconds = interval_seconds
         sh_publisher.sleep(delay_seconds)
         if stop_after_n_runs >= 0:
             sh_publisher.stop_after_n_runs = stop_after_n_runs
         task = asyncio.create_task(sh_publisher.run())
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/controller.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/mqtt/controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import mqtt
 
 import logging
 import tenacity
 import tenacity.stop
 import tenacity.wait
 import functools
-import transport.abc
+from amqp_mqtt_transport.abc import Controller
 import uuid
 
 
 __all__ = ['MQTTController', 'reconnect']
 
 logger = logging.getLogger(__name__)
 
@@ -25,15 +25,15 @@
             except Exception as e:
                 await manager.close()
                 raise e
         return wrapped
     return wrapper
 
 
-class MQTTController(transport.abc.Controller):
+class MQTTController(Controller):
     def __init__(self, host: str, port: int,
                  login: str, password: str,
                  ssl: bool):
         self._host = host
         self._port = port
         self._login = login
         self._password = password
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/mqtt/publisher.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/mqtt/publisher.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-import transport.abc
+from amqp_mqtt_transport.abc import Publisher
 from . import MQTTController
 import logging
 
 __all__ = ['MQTTPublisher']
 logger = logging.getLogger(__name__)
 
 
-class MQTTPublisher(transport.abc.Publisher):
+class MQTTPublisher(Publisher):
     def __init__(self, controller: MQTTController):
         self.__controller = controller
 
     @property
     def queue_name(self) -> str:
         return self.__queue_name
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport/scheduled_publisher.py` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport/scheduled_publisher.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import transport
+import amqp_mqtt_transport
 import logging
 import typing
 import asyncio
 import json
 
 
 __all__ = ['ScheduledPublisher']
@@ -25,15 +25,15 @@
     @interval_seconds.setter
     def interval_seconds(self, value: float):
         self._interval_sec = value
 
     def sleep(self, delay_seconds: float):
         self._delay_sec = delay_seconds
 
-    def __init__(self, publisher: transport.abc.Publisher) -> None:
+    def __init__(self, publisher: amqp_mqtt_transport.abc.Publisher) -> None:
         self._messages: typing.List[bytes] = []
         self._publisher = publisher  # amqp_controller.Publisher(self._amqp_connection)
         self._interval_sec: float = 0
         self.stop_after_n_runs: int = -1
 
     def add_message_to_list(self, message: typing.Dict):
         """Appends message to list of messages thats going to be published"""
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/PKG-INFO` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amqp-mqtt-transport
-Version: 0.1.5
+Version: 0.1.6
 Summary: Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers
 Author-email: Igor Toropov <it.cups.54@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `amqp_mqtt_transport-0.1.5/amqp_mqtt_transport.egg-info/SOURCES.txt` & `amqp_mqtt_transport-0.1.6/amqp_mqtt_transport.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amqp_mqtt_transport-0.1.5/pyproject.toml` & `amqp_mqtt_transport-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "amqp_mqtt_transport"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Igor Toropov", email="it.cups.54@gmail.com" },
 ]
 description = "Small wrapper for pykka-amqp and paho-mqtt packages. Makes it easier to create consumers/publishers"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

