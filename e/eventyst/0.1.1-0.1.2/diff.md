# Comparing `tmp/eventyst-0.1.1.tar.gz` & `tmp/eventyst-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventyst-0.1.1.tar", max compression
+gzip compressed data, was "eventyst-0.1.2.tar", max compression
```

## Comparing `eventyst-0.1.1.tar` & `eventyst-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    10757 2023-06-20 19:41:31.498604 eventyst-0.1.1/LICENSE
--rw-r--r--   0        0        0      705 2023-05-04 14:23:23.918279 eventyst-0.1.1/README.md
--rw-r--r--   0        0        0     1247 2023-06-20 19:49:45.811683 eventyst-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1203 2023-06-20 19:49:45.803683 eventyst-0.1.1/src/eventyst/__init__.py
--rw-r--r--   0        0        0      772 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/__main__.py
--rw-r--r--   0        0        0      839 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/_enums.py
--rw-r--r--   0        0        0     1312 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/_exceptions.py
--rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/adapters/__init__.py
--rw-r--r--   0        0        0      727 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/adapters/aws/__init__.py
--rw-r--r--   0        0        0    10743 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/adapters/aws/schema_registry.py
--rw-r--r--   0        0        0     5386 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/adapters/kafka.py
--rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/cli/__init__.py
--rw-r--r--   0        0        0     3823 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/cli/main.py
--rw-r--r--   0        0        0     2440 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/cli/styles.py
--rw-r--r--   0        0        0     4216 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/cli/utilities.py
--rw-r--r--   0        0        0     3315 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/configuration.py
--rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/core/__init__.py
--rw-r--r--   0        0        0     7637 2023-06-20 19:49:24.287290 eventyst-0.1.1/src/eventyst/core/application.py
--rw-r--r--   0        0        0      711 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/core/commands.py
--rw-r--r--   0        0        0    11157 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/core/dependency.py
--rw-r--r--   0        0        0     3382 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/core/events.py
--rw-r--r--   0        0        0     6385 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/core/handler_registry.py
--rw-r--r--   0        0        0     4484 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/core/message_bus.py
--rw-r--r--   0        0        0     3738 2023-06-20 19:48:10.909950 eventyst-0.1.1/src/eventyst/schema.py
--rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/serialization/__init__.py
--rw-r--r--   0        0        0     4639 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/serialization/codec.py
--rw-r--r--   0        0        0     2374 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/serialization/naming.py
--rw-r--r--   0        0        0     1962 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/serialization/registry.py
--rw-r--r--   0        0        0     6314 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/serialization/serializers.py
--rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/utilities/__init__.py
--rw-r--r--   0        0        0      875 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/utilities/async_tools.py
--rw-r--r--   0        0        0    32953 2023-06-20 19:43:16.980509 eventyst-0.1.1/src/eventyst/utilities/avro_schema.py
--rw-r--r--   0        0        0     1735 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/utilities/function_inspection.py
--rw-r--r--   0        0        0     1425 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/utilities/log.py
--rw-r--r--   0        0        0     3828 2023-06-20 19:41:56.319039 eventyst-0.1.1/src/eventyst/utilities/plotting.py
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 eventyst-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10757 2023-06-20 19:41:31.498604 eventyst-0.1.2/LICENSE
+-rw-r--r--   0        0        0      705 2023-05-04 14:23:23.918279 eventyst-0.1.2/README.md
+-rw-r--r--   0        0        0     1267 2023-06-20 19:56:22.330849 eventyst-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1203 2023-06-20 19:56:22.318849 eventyst-0.1.2/src/eventyst/__init__.py
+-rw-r--r--   0        0        0      772 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/__main__.py
+-rw-r--r--   0        0        0      839 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/_enums.py
+-rw-r--r--   0        0        0     1312 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/_exceptions.py
+-rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/adapters/__init__.py
+-rw-r--r--   0        0        0      727 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/adapters/aws/__init__.py
+-rw-r--r--   0        0        0    10743 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/adapters/aws/schema_registry.py
+-rw-r--r--   0        0        0     5386 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/adapters/kafka.py
+-rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/cli/__init__.py
+-rw-r--r--   0        0        0     3823 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/cli/main.py
+-rw-r--r--   0        0        0     2440 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/cli/styles.py
+-rw-r--r--   0        0        0     4216 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/cli/utilities.py
+-rw-r--r--   0        0        0     3315 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/configuration.py
+-rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/core/__init__.py
+-rw-r--r--   0        0        0     7637 2023-06-20 19:49:24.287290 eventyst-0.1.2/src/eventyst/core/application.py
+-rw-r--r--   0        0        0      711 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/core/commands.py
+-rw-r--r--   0        0        0    11157 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/core/dependency.py
+-rw-r--r--   0        0        0     3382 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/core/events.py
+-rw-r--r--   0        0        0     6385 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/core/handler_registry.py
+-rw-r--r--   0        0        0     4484 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/core/message_bus.py
+-rw-r--r--   0        0        0     3738 2023-06-20 19:48:10.909950 eventyst-0.1.2/src/eventyst/schema.py
+-rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/serialization/__init__.py
+-rw-r--r--   0        0        0     4639 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/serialization/codec.py
+-rw-r--r--   0        0        0     2374 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/serialization/naming.py
+-rw-r--r--   0        0        0     1962 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/serialization/registry.py
+-rw-r--r--   0        0        0     6314 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/serialization/serializers.py
+-rw-r--r--   0        0        0      596 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/utilities/__init__.py
+-rw-r--r--   0        0        0      875 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/utilities/async_tools.py
+-rw-r--r--   0        0        0    32953 2023-06-20 19:43:16.980509 eventyst-0.1.2/src/eventyst/utilities/avro_schema.py
+-rw-r--r--   0        0        0     1735 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/utilities/function_inspection.py
+-rw-r--r--   0        0        0     1425 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/utilities/log.py
+-rw-r--r--   0        0        0     3828 2023-06-20 19:41:56.319039 eventyst-0.1.2/src/eventyst/utilities/plotting.py
+-rw-r--r--   0        0        0     1714 1970-01-01 00:00:00.000000 eventyst-0.1.2/PKG-INFO
```

### Comparing `eventyst-0.1.1/LICENSE` & `eventyst-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/README.md` & `eventyst-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/pyproject.toml` & `eventyst-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,30 +6,31 @@
 line-length = 120
 skip-string-normalization = true
 target-version = ['py37', 'py38', 'py39', 'py310']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 tag_format = "v$version"
-version = "0.1.1"
+version = "0.1.2"
 version_files = [
   "pyproject.toml:version",
   "src/eventyst/__init__.py"
 ]
 
 [tool.poetry]
 authors = ["Michael Statt <michael.statt@modelyst.io>"]
 description = ""
 name = "eventyst"
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 
 [tool.poetry.dependencies]
 aiokafka = "^0.8.0"
 avro = "^1.11.1"
+boto3 = "^1.26.156"
 fastapi = "^0.95.1"
 fastavro = "^1.7.4"
 networkx = "^3.1"
 orjson = "^3.8.12"
 pendulum = "^2.1.2"
 poetry = "^1.4.2"
 pydantic = {version = "^1.10.7", extras = ["dotenv"]}
```

### Comparing `eventyst-0.1.1/src/eventyst/__init__.py` & `eventyst-0.1.2/src/eventyst/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,11 +22,11 @@
 from eventyst.core.events import Event  # noqa: F401
 from eventyst.core.message_bus import MessageBus  # noqa: F401
 
 __author__ = "Michael Statt"
 __email__ = "michael.statt@modelyst.io"
 __maintainer__ = "Michael Statt"
 __maintainer_email__ = "michael.statt@modelyst.io"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 
 
 version_uuid = UUID(hashlib.md5(__version__.encode()).hexdigest())
```

### Comparing `eventyst-0.1.1/src/eventyst/__main__.py` & `eventyst-0.1.2/src/eventyst/__main__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/_enums.py` & `eventyst-0.1.2/src/eventyst/_enums.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/_exceptions.py` & `eventyst-0.1.2/src/eventyst/_exceptions.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/adapters/__init__.py` & `eventyst-0.1.2/src/eventyst/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/adapters/aws/__init__.py` & `eventyst-0.1.2/src/eventyst/adapters/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/adapters/aws/schema_registry.py` & `eventyst-0.1.2/src/eventyst/adapters/aws/schema_registry.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/adapters/kafka.py` & `eventyst-0.1.2/src/eventyst/adapters/kafka.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/cli/__init__.py` & `eventyst-0.1.2/src/eventyst/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/cli/main.py` & `eventyst-0.1.2/src/eventyst/cli/main.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/cli/styles.py` & `eventyst-0.1.2/src/eventyst/cli/styles.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/cli/utilities.py` & `eventyst-0.1.2/src/eventyst/cli/utilities.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/configuration.py` & `eventyst-0.1.2/src/eventyst/configuration.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/__init__.py` & `eventyst-0.1.2/src/eventyst/core/__init__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/application.py` & `eventyst-0.1.2/src/eventyst/core/application.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/commands.py` & `eventyst-0.1.2/src/eventyst/core/commands.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/dependency.py` & `eventyst-0.1.2/src/eventyst/core/dependency.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/events.py` & `eventyst-0.1.2/src/eventyst/core/events.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/handler_registry.py` & `eventyst-0.1.2/src/eventyst/core/handler_registry.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/core/message_bus.py` & `eventyst-0.1.2/src/eventyst/core/message_bus.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/schema.py` & `eventyst-0.1.2/src/eventyst/schema.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/serialization/__init__.py` & `eventyst-0.1.2/src/eventyst/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/serialization/codec.py` & `eventyst-0.1.2/src/eventyst/serialization/codec.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/serialization/naming.py` & `eventyst-0.1.2/src/eventyst/serialization/naming.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/serialization/registry.py` & `eventyst-0.1.2/src/eventyst/serialization/registry.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/serialization/serializers.py` & `eventyst-0.1.2/src/eventyst/serialization/serializers.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/utilities/__init__.py` & `eventyst-0.1.2/src/eventyst/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/utilities/async_tools.py` & `eventyst-0.1.2/src/eventyst/utilities/async_tools.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/utilities/avro_schema.py` & `eventyst-0.1.2/src/eventyst/utilities/avro_schema.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/utilities/function_inspection.py` & `eventyst-0.1.2/src/eventyst/utilities/function_inspection.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/utilities/log.py` & `eventyst-0.1.2/src/eventyst/utilities/log.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/src/eventyst/utilities/plotting.py` & `eventyst-0.1.2/src/eventyst/utilities/plotting.py`

 * *Files identical despite different names*

### Comparing `eventyst-0.1.1/PKG-INFO` & `eventyst-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: eventyst
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Michael Statt
 Author-email: michael.statt@modelyst.io
 Requires-Python: >=3.8.1,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiokafka (>=0.8.0,<0.9.0)
 Requires-Dist: avro (>=1.11.1,<2.0.0)
+Requires-Dist: boto3 (>=1.26.156,<2.0.0)
 Requires-Dist: fastapi (>=0.95.1,<0.96.0)
 Requires-Dist: fastavro (>=1.7.4,<2.0.0)
 Requires-Dist: networkx (>=3.1,<4.0)
 Requires-Dist: orjson (>=3.8.12,<4.0.0)
 Requires-Dist: pendulum (>=2.1.2,<3.0.0)
 Requires-Dist: poetry (>=1.4.2,<2.0.0)
 Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
```

