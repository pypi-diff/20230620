# Comparing `tmp/macrometa-source-mongo-0.0.45.tar.gz` & `tmp/macrometa-source-mongo-0.0.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.45.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.46.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.45.tar` & `macrometa-source-mongo-0.0.46.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/LICENSE
--rw-r--r--   0        0        0    22638 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7337 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-06-20 14:13:14.522931 macrometa-source-mongo-0.0.45/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.45/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.45/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/LICENSE
+-rw-r--r--   0        0        0    22504 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7181 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-06-20 15:02:15.649089 macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-06-20 15:02:15.893093 macrometa-source-mongo-0.0.46/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.46/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.46/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.45/LICENSE` & `macrometa-source-mongo-0.0.46/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python3
 import copy
 import json
 import sys
 from typing import List, Dict
-import time
 
 import pkg_resources
 import singer
 from pymongo import MongoClient
 from singer import metadata, metrics, utils
 from c8connector import (
     C8Connector, ConfigProperty, Sample, Schema,
@@ -350,30 +349,26 @@
                     )
         cursor.try_next()
         # Get resume token from '_data' to resume LOG_BASED
         resume_token = {
             '_data': cursor.resume_token['_data']
         }
         cursor.close()
-        state = singer.write_bookmark(state, stream['tap_stream_id'], 'token', resume_token)
+        state = singer.write_bookmark(state, stream['tap_stream_id'], log_based.BOOKMARK_KEY, resume_token)
 
-    LOGGER.info("Starting full table sync")
     write_schema_message(stream)
     common.SCHEMA_COUNT[tap_stream_id] += 1
 
     with metrics.job_timer('sync_table') as timer:
         timer.tags['database'] = database_name
         timer.tags['table'] = stream['table_name']
 
         collection = client[database_name][stream["table_name"]]
         full_table.sync_database(collection, stream, state)
 
-    LOGGER.info("Sleeping")
-    time.sleep(100)
-    LOGGER.info("Full table sync completed")
     state = singer.set_currently_syncing(state, None)
 
     singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
 
 
 def sync_traditional_streams(client: MongoClient, traditional_streams: List[Dict], state: Dict,
                              replication_method: str):
```

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,52 +92,51 @@
                     resume_token = {
                         '_data': cursor.resume_token['_data']
                     }
         
                     # After MAX_AWAIT_TIME_MS has elapsed, the cursor will return None.
                     if change is None:
                         continue
-                    LOGGER.info(f'DB: {database.name}, collection: {change["ns"]["coll"]}')
+
                     tap_stream_id = f'{database.name}-{change["ns"]["coll"]}'
-        
                     operation = change['operationType']
-        
+
                     if operation == 'delete':
                         # Delete ops only contain the _id of the row deleted
                         singer.write_message(common.row_to_singer_record(
                             stream=streams_to_sync[tap_stream_id],
                             row={'_id': change['documentKey']['_id']},
                             time_extracted=utils.now(),
                             time_deleted=change[
                                 'clusterTime'].as_datetime()))  # returns python's datetime.datetime instance in UTC
-        
+
                         rows_saved[tap_stream_id] += 1
-        
+
                     elif operation == 'insert':
                         singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
                                                                          row=change['fullDocument'],
                                                                          time_extracted=utils.now(),
                                                                          time_deleted=None))
         
                         rows_saved[tap_stream_id] += 1
-        
+
                     elif operation == 'update':
                         # update operation only return _id and updated fields in the row,
                         query = {'_id': change['documentKey']['_id']}
                         row = database[streams_to_sync[tap_stream_id]['table_name']].find_one(query)
                         singer.write_message(common.row_to_singer_record(stream=streams_to_sync[tap_stream_id],
                                                                          row=row,
                                                                          time_extracted=utils.now(),
                                                                          time_deleted=None))
-        
+
                         rows_saved[tap_stream_id] += 1
-        
+
                     # update the states of all streams
                     state = update_bookmarks(state, stream_ids, resume_token)
-        
+
                     # Write state after every 1000 records
                     if sum(rows_saved.values()) % 1000 == 0:
                         # write state
                         singer.write_message(singer.StateMessage(value=copy.deepcopy(state)))
         except Exception as e:
             # Log the error
             LOGGER.error('Error received while syncing database: %s', str(e))
@@ -151,8 +150,8 @@
                 LOGGER.error('Unhandled error type, exiting...')
                 raise e
         for stream_id in stream_ids:
             common.TIMES[stream_id] += time.time() - start_time
             if rows_saved[stream_id] - rows_saved_iter_start[stream_id] > 0:
                 common.COUNTS[stream_id] += (rows_saved[stream_id] - rows_saved_iter_start[stream_id])
                 LOGGER.info('The number of records synchronized till now for %s is %s.', stream_id, rows_saved[stream_id])
-        time.sleep(10)
+        time.sleep(30)
```

### Comparing `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.46/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.45/pyproject.toml` & `macrometa-source-mongo-0.0.46/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.45'
+version='0.0.46'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.45/setup.py` & `macrometa-source-mongo-0.0.46/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.45',
+    'version': '0.0.46',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.45/PKG-INFO` & `macrometa-source-mongo-0.0.46/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.45
+Version: 0.0.46
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

