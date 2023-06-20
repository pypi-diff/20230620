# Comparing `tmp/macrometa-source-postgres-0.0.49.tar.gz` & `tmp/macrometa-source-postgres-0.0.50.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-postgres-0.0.49.tar", max compression
+gzip compressed data, was "macrometa-source-postgres-0.0.50.tar", max compression
```

## Comparing `macrometa-source-postgres-0.0.49.tar` & `macrometa-source-postgres-0.0.50.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11899 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/LICENSE
--rw-r--r--   0        0        0    35738 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/__init__.py
--rw-r--r--   0        0        0     8580 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/connection.py
--rw-r--r--   0        0        0    20349 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/helper.py
--rw-r--r--   0        0        0        0 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/__init__.py
--rw-r--r--   0        0        0     1212 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/common.py
--rw-r--r--   0        0        0     8974 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/full_table.py
--rw-r--r--   0        0        0    28329 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/log_based.py
--rw-r--r--   0        0        0     3698 2023-06-14 08:08:09.000997 macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/sample_data.py
--rw-r--r--   0        0        0     1512 2023-06-14 08:08:09.268998 macrometa-source-postgres-0.0.49/pyproject.toml
--rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.49/setup.py
--rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.49/PKG-INFO
+-rw-r--r--   0        0        0    11899 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/LICENSE
+-rw-r--r--   0        0        0    35738 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/__init__.py
+-rw-r--r--   0        0        0     8580 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/connection.py
+-rw-r--r--   0        0        0    20349 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/helper.py
+-rw-r--r--   0        0        0        0 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/__init__.py
+-rw-r--r--   0        0        0     1212 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/common.py
+-rw-r--r--   0        0        0     8974 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/full_table.py
+-rw-r--r--   0        0        0    28063 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/log_based.py
+-rw-r--r--   0        0        0     3698 2023-06-20 15:04:10.363716 macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/sample_data.py
+-rw-r--r--   0        0        0     1512 2023-06-20 15:04:10.619716 macrometa-source-postgres-0.0.50/pyproject.toml
+-rw-r--r--   0        0        0     1077 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.50/setup.py
+-rw-r--r--   0        0        0      877 1970-01-01 00:00:00.000000 macrometa-source-postgres-0.0.50/PKG-INFO
```

### Comparing `macrometa-source-postgres-0.0.49/LICENSE` & `macrometa-source-postgres-0.0.50/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/__init__.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/connection.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/connection.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/helper.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/helper.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/common.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/common.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/full_table.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/full_table.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/log_based.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/log_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -624,19 +624,15 @@
             else:
                 with contextlib.suppress(InterruptedError):
                      # Pause for one second if no message is received yet.
                      select([cur], [], [], 1)
 
             # Update the latest committed LSN position from the state file every poll_interval.
             if datetime.datetime.utcnow() >= poll_timestamp + datetime.timedelta(seconds=poll_interval):
-                if lsn_currently_processing is None:
-                    LOGGER.info('Awaiting the initial WAL (Write-Ahead Log) message.')
-                else:
-                    LOGGER.info('The most recent write-ahead log (WAL) message received was %s',
-                                int_to_lsn(lsn_last_processed))
+                if lsn_currently_processing is not None:
                     try:
                         with open(state_file, mode="r", encoding="utf-8") as fh:
                             state_committed = json.load(fh)
                     except Exception as e:
                         LOGGER.debug('Failed to open and parse json file %s: %s', state_file, e)
                     else:
                         lsn_committed = min(
```

### Comparing `macrometa-source-postgres-0.0.49/macrometa_source_postgres/sync_strategies/sample_data.py` & `macrometa-source-postgres-0.0.50/macrometa_source_postgres/sync_strategies/sample_data.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-postgres-0.0.49/pyproject.toml` & `macrometa-source-postgres-0.0.50/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-postgres"
-version='0.0.49'
+version='0.0.50'
 description = "Macrometa Source for extracting data from PostgreSQL."
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-postgres-0.0.49/setup.py` & `macrometa-source-postgres-0.0.50/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-postgres = '
                      'macrometa_source_postgres:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-postgres',
-    'version': '0.0.49',
+    'version': '0.0.50',
     'description': 'Macrometa Source for extracting data from PostgreSQL.',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-postgres-0.0.49/PKG-INFO` & `macrometa-source-postgres-0.0.50/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-postgres
-Version: 0.0.49
+Version: 0.0.50
 Summary: Macrometa Source for extracting data from PostgreSQL.
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,PostgreSQL,Source
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

