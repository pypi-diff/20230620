# Comparing `tmp/django_cqrs-2.7.0.tar.gz` & `tmp/django_cqrs-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_cqrs-2.7.0.tar", max compression
+gzip compressed data, was "django_cqrs-2.7.1.tar", max compression
```

## Comparing `django_cqrs-2.7.0.tar` & `django_cqrs-2.7.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0    11369 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/LICENSE
--rw-r--r--   0        0        0     9131 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/README.md
--rw-r--r--   0        0        0      196 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/__init__.py
--rw-r--r--   0        0        0     7634 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/_validation.py
--rw-r--r--   0        0        0     1842 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/admin.py
--rw-r--r--   0        0        0      289 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/apps.py
--rw-r--r--   0        0        0      728 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/constants.py
--rw-r--r--   0        0        0       60 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/controller/__init__.py
--rw-r--r--   0        0        0     3168 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/controller/consumer.py
--rw-r--r--   0        0        0      284 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/controller/producer.py
--rw-r--r--   0        0        0      698 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/correlation.py
--rw-r--r--   0        0        0     4722 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/dataclasses.py
--rw-r--r--   0        0        0     2232 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/delay.py
--rw-r--r--   0        0        0       60 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/__init__.py
--rw-r--r--   0        0        0       60 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/__init__.py
--rw-r--r--   0        0        0     4512 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_dump.py
--rw-r--r--   0        0        0     3612 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_load.py
--rw-r--r--   0        0        0     5805 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_consume.py
--rw-r--r--   0        0        0     5196 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_dead_letters.py
--rw-r--r--   0        0        0     1569 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
--rw-r--r--   0        0        0     2433 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
--rw-r--r--   0        0        0     1178 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
--rw-r--r--   0        0        0     2538 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_master.py
--rw-r--r--   0        0        0     1866 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_replica.py
--rw-r--r--   0        0        0     2156 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_sync.py
--rw-r--r--   0        0        0     4675 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_sync.py
--rw-r--r--   0        0        0      484 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/management/utils.py
--rw-r--r--   0        0        0    13276 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/managers.py
--rw-r--r--   0        0        0     5316 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/metas.py
--rw-r--r--   0        0        0    17146 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/mixins.py
--rw-r--r--   0        0        0     1390 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/registries.py
--rw-r--r--   0        0        0     5196 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/signals.py
--rw-r--r--   0        0        0     1807 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/tracker.py
--rw-r--r--   0        0        0      545 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/__init__.py
--rw-r--r--   0        0        0     1003 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/base.py
--rw-r--r--   0        0        0     6620 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/kombu.py
--rw-r--r--   0        0        0     3292 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/mixins.py
--rw-r--r--   0        0        0      316 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/mock.py
--rw-r--r--   0        0        0    15631 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/transport/rabbit_mq.py
--rw-r--r--   0        0        0     1501 2023-06-15 08:07:16.838540 django_cqrs-2.7.0/dj_cqrs/utils.py
--rw-r--r--   0        0        0     3332 2023-06-15 08:09:10.606085 django_cqrs-2.7.0/pyproject.toml
--rw-r--r--   0        0        0    10408 1970-01-01 00:00:00.000000 django_cqrs-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11369 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/LICENSE
+-rw-r--r--   0        0        0     9131 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/README.md
+-rw-r--r--   0        0        0      196 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/__init__.py
+-rw-r--r--   0        0        0     7634 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/_validation.py
+-rw-r--r--   0        0        0     1842 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/admin.py
+-rw-r--r--   0        0        0      289 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/apps.py
+-rw-r--r--   0        0        0      728 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/constants.py
+-rw-r--r--   0        0        0       60 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/controller/__init__.py
+-rw-r--r--   0        0        0     3880 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/controller/consumer.py
+-rw-r--r--   0        0        0      284 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/controller/producer.py
+-rw-r--r--   0        0        0      698 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/correlation.py
+-rw-r--r--   0        0        0     4722 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/dataclasses.py
+-rw-r--r--   0        0        0     2232 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/delay.py
+-rw-r--r--   0        0        0       60 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/__init__.py
+-rw-r--r--   0        0        0       60 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/__init__.py
+-rw-r--r--   0        0        0     4512 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_bulk_dump.py
+-rw-r--r--   0        0        0     3612 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_bulk_load.py
+-rw-r--r--   0        0        0     5805 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_consume.py
+-rw-r--r--   0        0        0     5196 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_dead_letters.py
+-rw-r--r--   0        0        0     1569 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_deleted_diff_master.py
+-rw-r--r--   0        0        0     2433 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py
+-rw-r--r--   0        0        0     1178 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py
+-rw-r--r--   0        0        0     2538 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_diff_master.py
+-rw-r--r--   0        0        0     1866 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_diff_replica.py
+-rw-r--r--   0        0        0     2156 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_diff_sync.py
+-rw-r--r--   0        0        0     4675 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_sync.py
+-rw-r--r--   0        0        0      484 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/management/utils.py
+-rw-r--r--   0        0        0    13276 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/managers.py
+-rw-r--r--   0        0        0     5316 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/metas.py
+-rw-r--r--   0        0        0    17146 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/mixins.py
+-rw-r--r--   0        0        0     1390 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/registries.py
+-rw-r--r--   0        0        0     5196 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/signals.py
+-rw-r--r--   0        0        0     1807 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/tracker.py
+-rw-r--r--   0        0        0      545 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/transport/__init__.py
+-rw-r--r--   0        0        0     1003 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/transport/base.py
+-rw-r--r--   0        0        0     6620 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/transport/kombu.py
+-rw-r--r--   0        0        0     3292 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/transport/mixins.py
+-rw-r--r--   0        0        0      316 2023-06-20 12:09:30.860488 django_cqrs-2.7.1/dj_cqrs/transport/mock.py
+-rw-r--r--   0        0        0    15631 2023-06-20 12:09:30.864488 django_cqrs-2.7.1/dj_cqrs/transport/rabbit_mq.py
+-rw-r--r--   0        0        0     1501 2023-06-20 12:09:30.864488 django_cqrs-2.7.1/dj_cqrs/utils.py
+-rw-r--r--   0        0        0     3332 2023-06-20 12:11:26.728319 django_cqrs-2.7.1/pyproject.toml
+-rw-r--r--   0        0        0    10408 1970-01-01 00:00:00.000000 django_cqrs-2.7.1/PKG-INFO
```

### Comparing `django_cqrs-2.7.0/LICENSE` & `django_cqrs-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/README.md` & `django_cqrs-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/_validation.py` & `django_cqrs-2.7.1/dj_cqrs/_validation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/admin.py` & `django_cqrs-2.7.1/dj_cqrs/admin.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/constants.py` & `django_cqrs-2.7.1/dj_cqrs/constants.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/controller/consumer.py` & `django_cqrs-2.7.1/dj_cqrs/controller/consumer.py`

 * *Files 19% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 
     db_is_needed = not model_cls.CQRS_NO_DB_OPERATIONS
     if db_is_needed:
         close_old_connections()
 
     is_meta_supported = model_cls.CQRS_META
     try:
+        if db_is_needed:
+            _apply_query_timeouts(model_cls)
+
         with transaction.atomic(savepoint=False) if db_is_needed else ExitStack():
             if signal_type == SignalType.DELETE:
                 if is_meta_supported:
                     return model_cls.cqrs_delete(instance_data, meta=meta)
 
                 return model_cls.cqrs_delete(instance_data)
 
@@ -93,7 +96,28 @@
                 str(e),
                 signal_type,
                 pk_value,
                 cqrs_revision,
                 model_cls.CQRS_ID,
             ),
         )
+
+
+def _apply_query_timeouts(model_cls):  # pragma: no cover
+    query_timeout = int(settings.CQRS['replica'].get('CQRS_QUERY_TIMEOUT', 0))
+    if query_timeout <= 0:
+        return
+
+    model_db = model_cls._default_manager.db
+    conn = transaction.get_connection(using=model_db)
+    conn_vendor = getattr(conn, 'vendor', '')
+
+    if conn_vendor not in {'postgresql', 'mysql'}:
+        return
+
+    if conn_vendor == 'postgresql':
+        statement = 'SET statement_timeout TO %s'
+    else:
+        statement = 'SET SESSION MAX_EXECUTION_TIME=%s'
+
+    with conn.cursor() as cursor:
+        cursor.execute(statement, params=(query_timeout,))
```

### Comparing `django_cqrs-2.7.0/dj_cqrs/correlation.py` & `django_cqrs-2.7.1/dj_cqrs/correlation.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/dataclasses.py` & `django_cqrs-2.7.1/dj_cqrs/dataclasses.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/delay.py` & `django_cqrs-2.7.1/dj_cqrs/delay.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_dump.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_bulk_dump.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_bulk_load.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_bulk_load.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_consume.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_consume.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_dead_letters.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_dead_letters.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_master.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_deleted_diff_master.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_deleted_diff_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_deleted_sync_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_master.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_diff_master.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_replica.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_diff_replica.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_diff_sync.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_diff_sync.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/management/commands/cqrs_sync.py` & `django_cqrs-2.7.1/dj_cqrs/management/commands/cqrs_sync.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/managers.py` & `django_cqrs-2.7.1/dj_cqrs/managers.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/metas.py` & `django_cqrs-2.7.1/dj_cqrs/metas.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/mixins.py` & `django_cqrs-2.7.1/dj_cqrs/mixins.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/registries.py` & `django_cqrs-2.7.1/dj_cqrs/registries.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/signals.py` & `django_cqrs-2.7.1/dj_cqrs/signals.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/tracker.py` & `django_cqrs-2.7.1/dj_cqrs/tracker.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/transport/__init__.py` & `django_cqrs-2.7.1/dj_cqrs/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/transport/base.py` & `django_cqrs-2.7.1/dj_cqrs/transport/base.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/transport/kombu.py` & `django_cqrs-2.7.1/dj_cqrs/transport/kombu.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/transport/mixins.py` & `django_cqrs-2.7.1/dj_cqrs/transport/mixins.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/transport/rabbit_mq.py` & `django_cqrs-2.7.1/dj_cqrs/transport/rabbit_mq.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/dj_cqrs/utils.py` & `django_cqrs-2.7.1/dj_cqrs/utils.py`

 * *Files identical despite different names*

### Comparing `django_cqrs-2.7.0/pyproject.toml` & `django_cqrs-2.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-cqrs"
-version = "2.7.0"
+version = "2.7.1"
 description = "Django CQRS data synchronisation"
 authors = ["CloudBlue LLC"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_cqrs" }
 ]
 readme = "./README.md"
```

### Comparing `django_cqrs-2.7.0/PKG-INFO` & `django_cqrs-2.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-cqrs
-Version: 2.7.0
+Version: 2.7.1
 Summary: Django CQRS data synchronisation
 Home-page: https://django-cqrs.readthedocs.org
 License: Apache-2.0
 Keywords: django,cqrs,sql,mixin,amqp
 Author: CloudBlue LLC
 Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
```

