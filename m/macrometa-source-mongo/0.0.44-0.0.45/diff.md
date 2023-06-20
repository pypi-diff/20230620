# Comparing `tmp/macrometa-source-mongo-0.0.44.tar.gz` & `tmp/macrometa-source-mongo-0.0.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-mongo-0.0.44.tar", max compression
+gzip compressed data, was "macrometa-source-mongo-0.0.45.tar", max compression
```

## Comparing `macrometa-source-mongo-0.0.44.tar` & `macrometa-source-mongo-0.0.45.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    10765 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/LICENSE
--rw-r--r--   0        0        0    22634 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/__init__.py
--rw-r--r--   0        0        0     6577 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/connection.py
--rw-r--r--   0        0        0      895 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/exceptions.py
--rw-r--r--   0        0        0     7252 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/helper.py
--rw-r--r--   0        0        0    10251 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/common.py
--rw-r--r--   0        0        0     3647 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/full_table.py
--rw-r--r--   0        0        0     7337 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/log_based.py
--rw-r--r--   0        0        0     2292 2023-06-20 14:10:50.939152 macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1548 2023-06-20 14:10:51.191160 macrometa-source-mongo-0.0.44/pyproject.toml
--rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.44/setup.py
--rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.44/PKG-INFO
+-rw-r--r--   0        0        0    10765 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/LICENSE
+-rw-r--r--   0        0        0    22638 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/__init__.py
+-rw-r--r--   0        0        0     6577 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/connection.py
+-rw-r--r--   0        0        0      895 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/exceptions.py
+-rw-r--r--   0        0        0     7252 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/helper.py
+-rw-r--r--   0        0        0    10251 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/common.py
+-rw-r--r--   0        0        0     3647 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/full_table.py
+-rw-r--r--   0        0        0     7337 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     2292 2023-06-20 14:13:14.214965 macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1548 2023-06-20 14:13:14.522931 macrometa-source-mongo-0.0.45/pyproject.toml
+-rw-r--r--   0        0        0     1095 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.45/setup.py
+-rw-r--r--   0        0        0      956 1970-01-01 00:00:00.000000 macrometa-source-mongo-0.0.45/PKG-INFO
```

### Comparing `macrometa-source-mongo-0.0.44/LICENSE` & `macrometa-source-mongo-0.0.45/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/__init__.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,17 +349,17 @@
                         start_after=start_after
                     )
         cursor.try_next()
         # Get resume token from '_data' to resume LOG_BASED
         resume_token = {
             '_data': cursor.resume_token['_data']
         }
+        cursor.close()
         state = singer.write_bookmark(state, stream['tap_stream_id'], 'token', resume_token)
 
-    cursor.close()
     LOGGER.info("Starting full table sync")
     write_schema_message(stream)
     common.SCHEMA_COUNT[tap_stream_id] += 1
 
     with metrics.job_timer('sync_table') as timer:
         timer.tags['database'] = database_name
         timer.tags['table'] = stream['table_name']
```

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/connection.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/exceptions.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/helper.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/common.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/full_table.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/log_based.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/log_based.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/macrometa_source_mongo/sync_strategies/sample_data.py` & `macrometa-source-mongo-0.0.45/macrometa_source_mongo/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-mongo-0.0.44/pyproject.toml` & `macrometa-source-mongo-0.0.45/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-mongo"
-version='0.0.44'
+version='0.0.45'
 description = "Macrometa Source for extracting data from MongoDB."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-mongo-0.0.44/setup.py` & `macrometa-source-mongo-0.0.45/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
  'tzlocal>=2.1.0,<2.2.0']
 
 entry_points = \
 {'console_scripts': ['macrometa-source-mongo = macrometa_source_mongo:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-mongo',
-    'version': '0.0.44',
+    'version': '0.0.45',
     'description': 'Macrometa Source for extracting data from MongoDB.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-mongo-0.0.44/PKG-INFO` & `macrometa-source-mongo-0.0.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-mongo
-Version: 0.0.44
+Version: 0.0.45
 Summary: Macrometa Source for extracting data from MongoDB.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,MongoDB,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

