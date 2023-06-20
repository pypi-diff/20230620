# Comparing `tmp/tasktiger-0.9.5.tar.gz` & `tmp/tasktiger-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tasktiger-0.9.5.tar", last modified: Tue Jul 30 11:24:25 2019, max compression
+gzip compressed data, was "dist/tasktiger-0.9.6.tar", last modified: Thu Sep 12 19:17:18 2019, max compression
```

## Comparing `tasktiger-0.9.5.tar` & `tasktiger-0.9.6.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 joe        (501) staff       (20)        0 2019-07-30 11:24:25.000000 tasktiger-0.9.5/
--rw-r--r--   0 joe        (501) staff       (20)     1089 2018-09-26 18:29:44.000000 tasktiger-0.9.5/LICENSE
--rw-r--r--   0 joe        (501) staff       (20)       53 2018-09-26 18:29:44.000000 tasktiger-0.9.5/MANIFEST.in
--rw-r--r--   0 joe        (501) staff       (20)    31848 2019-07-30 11:24:25.000000 tasktiger-0.9.5/PKG-INFO
--rw-r--r--   0 joe        (501) staff       (20)    25328 2019-06-18 11:48:07.000000 tasktiger-0.9.5/README.rst
--rw-r--r--   0 joe        (501) staff       (20)       71 2019-07-30 11:24:25.000000 tasktiger-0.9.5/setup.cfg
--rw-r--r--   0 joe        (501) staff       (20)     1530 2019-07-30 11:22:09.000000 tasktiger-0.9.5/setup.py
-drwxr-xr-x   0 joe        (501) staff       (20)        0 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger/
--rw-r--r--   0 joe        (501) staff       (20)    17386 2019-07-30 11:22:09.000000 tasktiger-0.9.5/tasktiger/__init__.py
--rw-r--r--   0 joe        (501) staff       (20)     3797 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/_internal.py
--rw-r--r--   0 joe        (501) staff       (20)     1584 2019-01-07 14:58:40.000000 tasktiger-0.9.5/tasktiger/exceptions.py
--rw-r--r--   0 joe        (501) staff       (20)     1137 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/flask_script.py
--rw-r--r--   0 joe        (501) staff       (20)      344 2019-03-06 15:17:08.000000 tasktiger-0.9.5/tasktiger/logging.py
-drwxr-xr-x   0 joe        (501) staff       (20)        0 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger/lua/
--rw-r--r--   0 joe        (501) staff       (20)     1983 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/lua/execute_pipeline.lua
--rw-r--r--   0 joe        (501) staff       (20)     1968 2019-01-18 14:24:56.000000 tasktiger-0.9.5/tasktiger/lua/semaphore.lua
--rw-r--r--   0 joe        (501) staff       (20)     5701 2018-09-26 19:46:20.000000 tasktiger-0.9.5/tasktiger/redis_lock.py
--rw-r--r--   0 joe        (501) staff       (20)    20051 2018-11-06 13:44:16.000000 tasktiger-0.9.5/tasktiger/redis_scripts.py
--rw-r--r--   0 joe        (501) staff       (20)     3142 2019-01-18 14:24:56.000000 tasktiger-0.9.5/tasktiger/redis_semaphore.py
--rw-r--r--   0 joe        (501) staff       (20)      756 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/retry.py
--rw-r--r--   0 joe        (501) staff       (20)     1785 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/rollbar.py
--rw-r--r--   0 joe        (501) staff       (20)     1291 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/schedule.py
--rw-r--r--   0 joe        (501) staff       (20)     2162 2018-11-28 20:32:47.000000 tasktiger-0.9.5/tasktiger/stats.py
--rw-r--r--   0 joe        (501) staff       (20)    15881 2019-06-19 13:21:35.000000 tasktiger-0.9.5/tasktiger/task.py
--rw-r--r--   0 joe        (501) staff       (20)     1142 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/test_helpers.py
--rw-r--r--   0 joe        (501) staff       (20)     2017 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tasktiger/timeouts.py
--rw-r--r--   0 joe        (501) staff       (20)    38805 2019-07-30 11:22:09.000000 tasktiger-0.9.5/tasktiger/worker.py
-drwxr-xr-x   0 joe        (501) staff       (20)        0 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/
--rw-r--r--   0 joe        (501) staff       (20)    31848 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/PKG-INFO
--rw-r--r--   0 joe        (501) staff       (20)      964 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/SOURCES.txt
--rw-r--r--   0 joe        (501) staff       (20)        1 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/dependency_links.txt
--rw-r--r--   0 joe        (501) staff       (20)       52 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/entry_points.txt
--rw-r--r--   0 joe        (501) staff       (20)       28 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/requires.txt
--rw-r--r--   0 joe        (501) staff       (20)       10 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tasktiger.egg-info/top_level.txt
-drwxr-xr-x   0 joe        (501) staff       (20)        0 2019-07-30 11:24:25.000000 tasktiger-0.9.5/tests/
--rw-r--r--   0 joe        (501) staff       (20)        1 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tests/__init__.py
--rw-r--r--   0 joe        (501) staff       (20)      150 2018-11-05 16:11:35.000000 tasktiger-0.9.5/tests/config.py
--rw-r--r--   0 joe        (501) staff       (20)     3229 2019-06-19 13:21:35.000000 tasktiger-0.9.5/tests/tasks.py
--rw-r--r--   0 joe        (501) staff       (20)      548 2019-07-30 11:22:09.000000 tasktiger-0.9.5/tests/tasks_periodic.py
--rw-r--r--   0 joe        (501) staff       (20)    36627 2019-02-18 16:10:32.000000 tasktiger-0.9.5/tests/test_base.py
--rw-r--r--   0 joe        (501) staff       (20)     1678 2019-01-18 15:53:31.000000 tasktiger-0.9.5/tests/test_context_manager.py
--rw-r--r--   0 joe        (501) staff       (20)     2012 2019-03-06 15:17:08.000000 tasktiger-0.9.5/tests/test_logging.py
--rw-r--r--   0 joe        (501) staff       (20)     3908 2019-07-30 11:22:09.000000 tasktiger-0.9.5/tests/test_periodic.py
--rw-r--r--   0 joe        (501) staff       (20)     2735 2019-01-07 14:58:40.000000 tasktiger-0.9.5/tests/test_queue_size.py
--rw-r--r--   0 joe        (501) staff       (20)    12675 2018-09-26 18:29:44.000000 tasktiger-0.9.5/tests/test_redis_scripts.py
--rw-r--r--   0 joe        (501) staff       (20)     5589 2019-01-18 14:24:56.000000 tasktiger-0.9.5/tests/test_semaphore.py
--rw-r--r--   0 joe        (501) staff       (20)     4903 2019-06-19 13:21:35.000000 tasktiger-0.9.5/tests/test_workers.py
--rw-r--r--   0 joe        (501) staff       (20)     2125 2019-07-30 11:22:09.000000 tasktiger-0.9.5/tests/utils.py
--rw-r--r--   0 joe        (501) staff       (20)      113 2019-01-14 14:16:35.000000 tasktiger-0.9.5/tox.ini
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-09-12 19:17:18.000000 tasktiger-0.9.6/
+-rw-r--r--   0 tom        (501) staff       (20)     1089 2018-08-02 20:27:14.000000 tasktiger-0.9.6/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       53 2018-08-02 20:27:14.000000 tasktiger-0.9.6/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)    31844 2019-09-12 19:17:18.000000 tasktiger-0.9.6/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    25324 2019-08-30 18:47:56.000000 tasktiger-0.9.6/README.rst
+-rw-r--r--   0 tom        (501) staff       (20)       71 2019-09-12 19:17:18.000000 tasktiger-0.9.6/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)     1530 2019-09-12 19:17:00.000000 tasktiger-0.9.6/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger/
+-rw-r--r--   0 tom        (501) staff       (20)    18310 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tasktiger/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3797 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/_internal.py
+-rw-r--r--   0 tom        (501) staff       (20)     1584 2019-01-14 20:02:14.000000 tasktiger-0.9.6/tasktiger/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)     1137 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/flask_script.py
+-rw-r--r--   0 tom        (501) staff       (20)      344 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tasktiger/logging.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger/lua/
+-rw-r--r--   0 tom        (501) staff       (20)     1983 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/lua/execute_pipeline.lua
+-rw-r--r--   0 tom        (501) staff       (20)     1968 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tasktiger/lua/semaphore.lua
+-rw-r--r--   0 tom        (501) staff       (20)     5701 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/redis_lock.py
+-rw-r--r--   0 tom        (501) staff       (20)    20051 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/redis_scripts.py
+-rw-r--r--   0 tom        (501) staff       (20)     3142 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tasktiger/redis_semaphore.py
+-rw-r--r--   0 tom        (501) staff       (20)      756 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/retry.py
+-rw-r--r--   0 tom        (501) staff       (20)     1785 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/rollbar.py
+-rw-r--r--   0 tom        (501) staff       (20)     1291 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/schedule.py
+-rw-r--r--   0 tom        (501) staff       (20)     2162 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/stats.py
+-rw-r--r--   0 tom        (501) staff       (20)    15881 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tasktiger/task.py
+-rw-r--r--   0 tom        (501) staff       (20)     1142 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/test_helpers.py
+-rw-r--r--   0 tom        (501) staff       (20)     2017 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tasktiger/timeouts.py
+-rw-r--r--   0 tom        (501) staff       (20)    38990 2019-09-12 19:17:00.000000 tasktiger-0.9.6/tasktiger/worker.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)    31844 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      988 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)       52 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/entry_points.txt
+-rw-r--r--   0 tom        (501) staff       (20)       28 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       10 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tasktiger.egg-info/top_level.txt
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-09-12 19:17:18.000000 tasktiger-0.9.6/tests/
+-rw-r--r--   0 tom        (501) staff       (20)        1 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tests/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)      150 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tests/config.py
+-rw-r--r--   0 tom        (501) staff       (20)     3229 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/tasks.py
+-rw-r--r--   0 tom        (501) staff       (20)      548 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/tasks_periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)    36627 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     1678 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_context_manager.py
+-rw-r--r--   0 tom        (501) staff       (20)      586 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_lazy_init.py
+-rw-r--r--   0 tom        (501) staff       (20)     2012 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_logging.py
+-rw-r--r--   0 tom        (501) staff       (20)     3908 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_periodic.py
+-rw-r--r--   0 tom        (501) staff       (20)     2735 2019-01-14 20:02:14.000000 tasktiger-0.9.6/tests/test_queue_size.py
+-rw-r--r--   0 tom        (501) staff       (20)    12675 2018-08-02 20:27:14.000000 tasktiger-0.9.6/tests/test_redis_scripts.py
+-rw-r--r--   0 tom        (501) staff       (20)     5589 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_semaphore.py
+-rw-r--r--   0 tom        (501) staff       (20)     4903 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/test_workers.py
+-rw-r--r--   0 tom        (501) staff       (20)     2201 2019-08-30 18:47:56.000000 tasktiger-0.9.6/tests/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      113 2019-01-14 20:02:14.000000 tasktiger-0.9.6/tox.ini
```

### Comparing `tasktiger-0.9.5/LICENSE` & `tasktiger-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/PKG-INFO` & `tasktiger-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 1.1
 Name: tasktiger
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python task queue
 Home-page: http://github.com/closeio/tasktiger
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: =========
         TaskTiger
         =========
         .. image:: https://circleci.com/gh/closeio/tasktiger/tree/master.svg?style=svg&circle-token=a86617952aa9b4cfee784b6ac43358cd042a6672
             :target: https://circleci.com/gh/closeio/tasktiger/tree/master
         
         *TaskTiger* is a Python task queue using Redis.
         
         
-        (Interested in working on projects like this? `Close.io`_ is looking for `great engineers`_ to join our team)
+        (Interested in working on projects like this? `Close`_ is looking for `great engineers`_ to join our team)
         
-        .. _Close.io: http://close.io
-        .. _great engineers: http://jobs.close.io
+        .. _Close: http://close.com
+        .. _great engineers: http://jobs.close.com
         
         
         .. contents:: Contents
         
         Features
         --------
```

### Comparing `tasktiger-0.9.5/README.rst` & `tasktiger-0.9.6/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 =========
 .. image:: https://circleci.com/gh/closeio/tasktiger/tree/master.svg?style=svg&circle-token=a86617952aa9b4cfee784b6ac43358cd042a6672
     :target: https://circleci.com/gh/closeio/tasktiger/tree/master
 
 *TaskTiger* is a Python task queue using Redis.
 
 
-(Interested in working on projects like this? `Close.io`_ is looking for `great engineers`_ to join our team)
+(Interested in working on projects like this? `Close`_ is looking for `great engineers`_ to join our team)
 
-.. _Close.io: http://close.io
-.. _great engineers: http://jobs.close.io
+.. _Close: http://close.com
+.. _great engineers: http://jobs.close.com
 
 
 .. contents:: Contents
 
 Features
 --------
```

### Comparing `tasktiger-0.9.5/setup.py` & `tasktiger-0.9.6/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'freezefrog',
     'pytest',
     'psutil',
 ]
 
 setup(
     name='tasktiger',
-    version='0.9.5',
+    version='0.9.6',
     url='http://github.com/closeio/tasktiger',
     license='MIT',
     description='Python task queue',
     long_description=long_description,
     test_suite='tests',
     tests_require=tests_require,
     platforms='any',
```

### Comparing `tasktiger-0.9.5/tasktiger/__init__.py` & `tasktiger-0.9.6/tasktiger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,20 +71,52 @@
 Queue locks scored by timeout
 ZSET <prefix>:qslock:<queue>
 STRING <prefix>:qlock:<queue> (Legacy queue locks that are no longer used)
 """
 
 
 class TaskTiger(object):
-    def __init__(self, connection=None, config=None, setup_structlog=False):
+    def __init__(
+            self,
+            connection=None,
+            config=None,
+            setup_structlog=False,
+            lazy_init=False):
         """
         Initializes TaskTiger with the given Redis connection and config
         options. Optionally sets up structlog.
+
+        Lazy initialization can be used to create a TaskTiger instance
+        and import decorated tasks before Redis connection and configuration
+        is available.
+
+        You will have to provide Redis and config before scheduling any tasks
+        using init method.
         """
 
+        self.config = None
+
+        # List of task functions that are executed periodically.
+        self.periodic_task_funcs = {}
+
+        if lazy_init:
+            assert connection is None and config is None and setup_structlog is False
+        else:
+            self.init(
+                connection=connection,
+                config=config,
+                setup_structlog=setup_structlog
+            )
+
+    def init(self, connection=None, config=None, setup_structlog=False):
+        """Provide Redis connection and config when lazy initialization is used."""
+
+        if self.config is not None:
+            raise RuntimeError('TaskTiger was already initialized')
+
         self.config = {
             # String that is used to prefix all Redis keys
             'REDIS_PREFIX': 't',
 
             # Name of the Python (structlog) logger
             'LOGGER_NAME': 'tasktiger',
 
@@ -197,17 +229,14 @@
             self.config['LOGGER_NAME'],
         ).bind()
 
         if setup_structlog:
             self.log.setLevel(logging.DEBUG)
             logging.basicConfig(format='%(message)s')
 
-        # List of task functions that are executed periodically.
-        self.periodic_task_funcs = {}
-
         self.connection = connection or redis.Redis(decode_responses=True)
         self.scripts = RedisScripts(self.connection)
 
     def _get_current_task(self):
         if g['current_tasks'] is None:
             raise RuntimeError('Must be accessed from within a task')
         if g['current_task_is_batch']:
```

### Comparing `tasktiger-0.9.5/tasktiger/_internal.py` & `tasktiger-0.9.6/tasktiger/_internal.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/exceptions.py` & `tasktiger-0.9.6/tasktiger/exceptions.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/flask_script.py` & `tasktiger-0.9.6/tasktiger/flask_script.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/lua/execute_pipeline.lua` & `tasktiger-0.9.6/tasktiger/lua/execute_pipeline.lua`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/lua/semaphore.lua` & `tasktiger-0.9.6/tasktiger/lua/semaphore.lua`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/redis_lock.py` & `tasktiger-0.9.6/tasktiger/redis_lock.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/redis_scripts.py` & `tasktiger-0.9.6/tasktiger/redis_scripts.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/redis_semaphore.py` & `tasktiger-0.9.6/tasktiger/redis_semaphore.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/retry.py` & `tasktiger-0.9.6/tasktiger/retry.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/rollbar.py` & `tasktiger-0.9.6/tasktiger/rollbar.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/schedule.py` & `tasktiger-0.9.6/tasktiger/schedule.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/stats.py` & `tasktiger-0.9.6/tasktiger/stats.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/task.py` & `tasktiger-0.9.6/tasktiger/task.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/test_helpers.py` & `tasktiger-0.9.6/tasktiger/test_helpers.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/timeouts.py` & `tasktiger-0.9.6/tasktiger/timeouts.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tasktiger/worker.py` & `tasktiger-0.9.6/tasktiger/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -623,15 +623,15 @@
         for tasks in tasks_by_func.values():
             success, processed_tasks = self._execute_task_group(queue,
                     tasks, valid_task_ids, queue_lock)
             processed_count = processed_count + len(processed_tasks)
             log.debug('processed', attempted=len(tasks),
                       processed=processed_count)
             for task in processed_tasks:
-                self._finish_task_processing(queue, task, success)
+                self._finish_task_processing(queue, task, success, now)
 
         return processed_count
 
     def _process_from_queue(self, queue):
         """
         Internal method to process a task batch from the given queue.
 
@@ -752,26 +752,29 @@
             self.stats_thread.report_task_end()
 
         for lock in locks:
             lock.release()
 
         return success, ready_tasks
 
-    def _finish_task_processing(self, queue, task, success):
+    def _finish_task_processing(self, queue, task, success, start_time):
         """
         After a task is executed, this method is called and ensures that
         the task gets properly removed from the ACTIVE queue and, in case of an
         error, retried or marked as failed.
         """
         log = self.log.bind(queue=queue, task_id=task.id)
 
+        now = time.time()
+        processing_duration = now - start_time
+
         def _mark_done():
             # Remove the task from active queue
             task._move(from_state=ACTIVE)
-            log.info('done')
+            log.info('done', processing_duration=processing_duration)
 
         if success:
             _mark_done()
         else:
             should_retry = False
             should_log_error = True
             # Get execution info (for logging and retry purposes)
@@ -805,18 +808,19 @@
                             if task.should_retry_on(exception_class, logger=log):
                                 should_retry = True
                 else:
                     should_retry = True
 
             state = ERROR
 
-            when = time.time()
+            when = now
 
             log_context = {
-                'func': task.serialized_func
+                'func': task.serialized_func,
+                'processing_duration': processing_duration,
             }
 
             if should_retry:
                 retry_num = task.n_executions()
                 log_context['retry_func'] = retry_func
                 log_context['retry_num'] = retry_num
```

### Comparing `tasktiger-0.9.5/tasktiger.egg-info/PKG-INFO` & `tasktiger-0.9.6/tasktiger.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 1.1
 Name: tasktiger
-Version: 0.9.5
+Version: 0.9.6
 Summary: Python task queue
 Home-page: http://github.com/closeio/tasktiger
 Author: UNKNOWN
 Author-email: UNKNOWN
 License: MIT
 Description: =========
         TaskTiger
         =========
         .. image:: https://circleci.com/gh/closeio/tasktiger/tree/master.svg?style=svg&circle-token=a86617952aa9b4cfee784b6ac43358cd042a6672
             :target: https://circleci.com/gh/closeio/tasktiger/tree/master
         
         *TaskTiger* is a Python task queue using Redis.
         
         
-        (Interested in working on projects like this? `Close.io`_ is looking for `great engineers`_ to join our team)
+        (Interested in working on projects like this? `Close`_ is looking for `great engineers`_ to join our team)
         
-        .. _Close.io: http://close.io
-        .. _great engineers: http://jobs.close.io
+        .. _Close: http://close.com
+        .. _great engineers: http://jobs.close.com
         
         
         .. contents:: Contents
         
         Features
         --------
```

### Comparing `tasktiger-0.9.5/tasktiger.egg-info/SOURCES.txt` & `tasktiger-0.9.6/tasktiger.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 tasktiger/lua/semaphore.lua
 tests/__init__.py
 tests/config.py
 tests/tasks.py
 tests/tasks_periodic.py
 tests/test_base.py
 tests/test_context_manager.py
+tests/test_lazy_init.py
 tests/test_logging.py
 tests/test_periodic.py
 tests/test_queue_size.py
 tests/test_redis_scripts.py
 tests/test_semaphore.py
 tests/test_workers.py
 tests/utils.py
```

### Comparing `tasktiger-0.9.5/tests/tasks.py` & `tasktiger-0.9.6/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/tasks_periodic.py` & `tasktiger-0.9.6/tests/tasks_periodic.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_base.py` & `tasktiger-0.9.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_context_manager.py` & `tasktiger-0.9.6/tests/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_logging.py` & `tasktiger-0.9.6/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_periodic.py` & `tasktiger-0.9.6/tests/test_periodic.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_queue_size.py` & `tasktiger-0.9.6/tests/test_queue_size.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_redis_scripts.py` & `tasktiger-0.9.6/tests/test_redis_scripts.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_semaphore.py` & `tasktiger-0.9.6/tests/test_semaphore.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/test_workers.py` & `tasktiger-0.9.6/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `tasktiger-0.9.5/tests/utils.py` & `tasktiger-0.9.6/tests/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,36 @@
 import logging
 import redis
 import structlog
 from tasktiger import TaskTiger, Worker, fixed
 
 from .config import DELAY, TEST_DB
 
+TEST_TIGER_CONFIG = {
+    # We need this 0 here so we don't pick up scheduled tasks when
+    # doing a single worker run.
+    'SELECT_TIMEOUT': 0,
+
+    'ACTIVE_TASK_UPDATE_TIMEOUT': 2 * DELAY,
+
+    'REQUEUE_EXPIRED_TASKS_INTERVAL': DELAY,
+
+    'LOCK_RETRY': DELAY * 2.,
+
+    'DEFAULT_RETRY_METHOD': fixed(DELAY, 2),
+
+    'BATCH_QUEUES': {
+        'batch': 3,
+    },
+
+    'SINGLE_WORKER_QUEUES': ['swq'],
+
+    'EXCLUDE_QUEUES': ['periodic_ignore'],
+}
+
 
 class Patch(object):
     """
     Simple context manager to patch a function, e.g.:
 
     with Patch(module, 'func_name', mocked_func):
         module.func_name() # will use mocked_func
@@ -24,45 +46,33 @@
         self.orig_func = getattr(self.orig_obj, self.func_name)
         setattr(self.orig_obj, self.func_name, self.new_func)
 
     def __exit__(self, *args):
         setattr(self.orig_obj, self.func_name, self.orig_func)
 
 
-def get_tiger():
-    """
-    Sets up logging and returns a new tasktiger instance.
-    """
+def setup_structlog():
     structlog.configure(
         logger_factory=structlog.stdlib.LoggerFactory(),
         wrapper_class=structlog.stdlib.BoundLogger,
     )
     logging.basicConfig(format='%(message)s')
-    conn = redis.Redis(db=TEST_DB, decode_responses=True)
-    tiger = TaskTiger(connection=conn, config={
-        # We need this 0 here so we don't pick up scheduled tasks when
-        # doing a single worker run.
-        'SELECT_TIMEOUT': 0,
-
-        'ACTIVE_TASK_UPDATE_TIMEOUT': 2 * DELAY,
-
-        'REQUEUE_EXPIRED_TASKS_INTERVAL': DELAY,
-
-        'LOCK_RETRY': DELAY * 2.,
 
-        'DEFAULT_RETRY_METHOD': fixed(DELAY, 2),
 
-        'BATCH_QUEUES': {
-            'batch': 3,
-        },
+def get_redis():
+    return redis.Redis(db=TEST_DB, decode_responses=True)
 
-        'SINGLE_WORKER_QUEUES': ['swq'],
 
-        'EXCLUDE_QUEUES': ['periodic_ignore'],
-    })
+def get_tiger():
+    """
+    Sets up logging and returns a new tasktiger instance.
+    """
+    setup_structlog()
+    conn = get_redis()
+    tiger = TaskTiger(connection=conn, config=TEST_TIGER_CONFIG)
     tiger.log.setLevel(logging.CRITICAL)
     return tiger
 
 
 def external_worker(n=None, patch_config=None, max_workers_per_queue=None):
     """
     Runs a worker. To be used with multiprocessing.Pool.map.
```

