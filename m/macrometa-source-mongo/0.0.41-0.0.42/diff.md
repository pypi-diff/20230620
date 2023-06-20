# Comparing `tmp/macrometa-source-mongo-0.0.41.tar.gz` & `tmp/macrometa-source-mongo-0.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.41.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.42.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.41.tar` & `macrometa-source-mongo-0.0.42.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/LICENSE
--rw-r--r--   0        0        0    21264 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7271 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-06-14 08:48:52.103778 macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-06-14 08:48:52.343782 macrometa-source-mongo-0.0.41/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.41/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.41/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-06-20 13:34:30.257043 macrometa-source-mongo-0.0.42/LICENSE
+-rw-r--r--   0        0        0    22600 2023-06-20 13:34:30.257043 macrometa-source-mongo-0.0.42/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7271 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-06-20 13:34:30.261042 macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-06-20 13:34:30.501037 macrometa-source-mongo-0.0.42/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.42/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.42/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.41/LICENSE` & `macrometa-source-mongo-0.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python3
 import copy
 import json
 import sys
 from typing import List, Dict
+import time
 
 import pkg_resources
 import singer
 from pymongo import MongoClient
 from singer import metadata, metrics, utils
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
@@ -325,24 +326,53 @@
     database_name = metadata.get(md_map, (), 'database-name')
 
     # Emit a state message to indicate that we've started this stream
     state = clear_state_on_replication_change(stream, state, replication_method)
     state = singer.set_currently_syncing(state, stream['tap_stream_id'])
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
+    if replication_method == LOG_BASED_METHOD:
+        resume_token = singer.get_bookmark(state,
+                                          stream['tap_stream_id'],
+                                          'token')
+        start_after = resume_token.get('_data') if resume_token else None
+        cursor = client[database_name].watch(
+                        [{'$match': {
+                            '$or': [
+                                {'operationType': 'insert'}, {'operationType': 'update'}, {'operationType': 'delete'}
+                            ],
+                            '$and': [
+                                # watch collections of selected streams
+                                {'ns.coll': {'$in': [stream['table_name']]}}
+                            ]
+                        }}],
+                        max_await_time_ms=500,
+                        start_after=start_after
+                    )
+        cursor.try_next()
+        # Get resume token from '_data' to resume LOG_BASED
+        resume_token = {
+            '_data': cursor.resume_token['_data']
+        }
+        state = singer.write_bookmark(state, stream['tap_stream_id'], 'token', resume_token)
+
+    LOGGER.info("Starting full table sync")
     write_schema_message(stream)
     common.SCHEMA_COUNT[tap_stream_id] += 1
 
     with metrics.job_timer('sync_table') as timer:
         timer.tags['database'] = database_name
         timer.tags['table'] = stream['table_name']
 
         collection = client[database_name][stream["table_name"]]
         full_table.sync_database(collection, stream, state)
 
+    LOGGER.info("Sleeping")
+    time.sleep(300)
+    LOGGER.info("Full table sync completed")
     state = singer.set_currently_syncing(state, None)
 
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def sync_traditional_streams(client: MongoClient, traditional_streams: List[Dict], state: Dict,
                              replication_method: str):
```

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.42/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.41/pyproject.toml` & `macrometa-source-mongo-0.0.42/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.41'
+version='0.0.42'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.41/setup.py` & `macrometa-source-mongo-0.0.42/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.41',
+    'version': '0.0.42',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.41/PKG-INFO` & `macrometa-source-mongo-0.0.42/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.41
+Version: 0.0.42
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

