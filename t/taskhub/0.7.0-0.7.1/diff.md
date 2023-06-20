# Comparing `tmp/taskhub-0.7.0.tar.gz` & `tmp/taskhub-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\taskhub-0.7.0.tar", last modified: Tue Aug 17 04:14:14 2021, max compression
+gzip compressed data, was "dist\taskhub-0.7.1.tar", last modified: Tue Jun 20 08:25:59 2023, max compression
```

## Comparing `taskhub-0.7.0.tar` & `taskhub-0.7.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2021-08-17 04:14:14.000000 taskhub-0.7.0/
--rw-rw-rw-   0        0        0      291 2021-08-17 04:14:14.000000 taskhub-0.7.0/PKG-INFO
--rw-rw-rw-   0        0        0       64 2021-08-17 04:14:14.000000 taskhub-0.7.0/setup.cfg
--rw-rw-rw-   0        0        0      469 2021-08-17 04:14:13.000000 taskhub-0.7.0/setup.py
-drwxrwxrwx   0        0        0        0 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub/
--rw-rw-rw-   0        0        0      473 2021-04-29 08:13:58.000000 taskhub-0.7.0/taskhub/connector.py
--rw-rw-rw-   0        0        0     6972 2021-08-17 04:12:58.000000 taskhub-0.7.0/taskhub/hub.py
--rw-rw-rw-   0        0        0     1013 2021-06-15 07:48:51.000000 taskhub-0.7.0/taskhub/server.py
--rw-rw-rw-   0        0        0        0 2021-04-29 07:43:00.000000 taskhub-0.7.0/taskhub/__init__.py
-drwxrwxrwx   0        0        0        0 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub.egg-info/
--rw-rw-rw-   0        0        0        1 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      291 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub.egg-info/requires.txt
--rw-rw-rw-   0        0        0      268 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        8 2021-08-17 04:14:14.000000 taskhub-0.7.0/taskhub.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-08-17 04:14:14.000000 taskhub-0.7.0/test/
--rw-rw-rw-   0        0        0      432 2021-04-29 07:25:16.000000 taskhub-0.7.0/test/test.py
--rw-rw-rw-   0        0        0      889 2021-08-17 04:07:25.000000 taskhub-0.7.0/test/test_serve.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/
+-rw-rw-rw-   0        0        0      291 2023-06-20 08:25:59.000000 taskhub-0.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-20 08:25:59.000000 taskhub-0.7.1/setup.cfg
+-rw-rw-rw-   0        0        0      483 2023-06-20 08:02:46.000000 taskhub-0.7.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub/
+-rw-rw-rw-   0        0        0        0 2023-06-20 07:32:14.000000 taskhub-0.7.1/taskhub/__init__.py
+-rw-rw-rw-   0        0        0      473 2023-06-20 07:32:14.000000 taskhub-0.7.1/taskhub/connector.py
+-rw-rw-rw-   0        0        0     6979 2023-06-20 08:06:58.000000 taskhub-0.7.1/taskhub/hub.py
+-rw-rw-rw-   0        0        0     1345 2023-06-20 08:25:53.000000 taskhub-0.7.1/taskhub/log.py
+-rw-rw-rw-   0        0        0     1013 2023-06-20 07:38:40.000000 taskhub-0.7.1/taskhub/server.py
+drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/
+-rw-rw-rw-   0        0        0      291 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-20 08:25:59.000000 taskhub-0.7.1/taskhub.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-20 08:25:59.000000 taskhub-0.7.1/test/
+-rw-rw-rw-   0        0        0      432 2023-06-20 07:32:14.000000 taskhub-0.7.1/test/test.py
+-rw-rw-rw-   0        0        0      901 2023-06-20 07:38:55.000000 taskhub-0.7.1/test/test_serve.py
```

### Comparing `taskhub-0.7.0/taskhub/hub.py` & `taskhub-0.7.1/taskhub/hub.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import random
 import time
 import json
-import requests
 import traceback
 from multiprocessing.managers import BaseManager
 
-
-from retry import retry
-from loger import log
-
+from taskhub.log import logger
 
 class HubManager(BaseManager):
     pass
 
 
 class Task():
     key = ""
@@ -35,15 +31,14 @@
             TaskInitError: [初始化错误，检查数据格式与范围]
         """
         if isinstance(key, str) and isinstance(priority, int) and isinstance(data, dict)\
                 and isinstance(task_type, str) and 0 < priority < 1000000:
             self.key = key
             self.priority = priority if priority < 1000000 else 1000000
             self.data = data
-            self.task_type = task_type
         else:
             raise TaskInitError()
 
     def get_dict(self):
         return {
             "key": self.key,
             "priority": self.priority,
@@ -84,15 +79,15 @@
 
         # 加锁
         self.get_lock()
         # 检查是否存在
         if not self.tasks.get(task.key):
             # 不存在则添加
             self.tasks[task.key] = task
-            log("task added!", 4)
+            logger.info("task added!", 4)
             # 释放锁并返回
             self.release_lock()
             return True
         else:
             # 存在则释放锁并抛出异常
             self.release_lock()
             raise TaskAlreadyExist()
@@ -157,79 +152,77 @@
 
                 try:
                     # 加锁
                     self.get_lock()
                     # 输出状态
                     status_count = dict()
                     for key, task in self.tasks.items():
-                        status_count[task.status] = status_count[task.status] + 1 if status_count.get(task.status) else 1
+                        status_count[task.status] = status_count[task.status] + \
+                            1 if status_count.get(task.status) else 1
                     status_str = ""
                     for statu, amount in status_count.items():
                         status_str += "{}:{}  ".format(statu, amount)
-                    log(status_str)
+                    logger.info(status_str)
 
                     # 检查需要同步的数据
                     for_del_key = []
                     for key, task in self.tasks.items():
                         if task.status == "done":
                             # 将数据同步到后端
                             if self.sync(task):
                                 for_del_key.append(key)
                     # 删除同步成功的
                     for key in for_del_key:
                         del self.tasks[key]
 
                 except:
-                    log("未知异常：{}".format(traceback.format_exc()), 1)
+                    logger.error("未知异常：{}".format(traceback.format_exc()), 1)
 
                 finally:
                     # 释放锁
                     self.release_lock()
 
                 t = time.time()
                 time.sleep(1)
 
     def get_lock(self):
-        # log("getting lock ....")
         while self.lock:
             time.sleep(random.random())
         self.lock = True
-        # log("lock got!")
 
     def release_lock(self):
         self.lock = False
-        # log("lock released!")
 
 
 class TaskIdExitRequired(Exception):
-    def __str__(self, task):
+    def __str__(task):
         return "id is required for a task dict!{}".format(task)
 
 
 class TaskAlreadyExist(Exception):
-    def __str__(self):
-        return "task already exist! "
+    def __str__(task_id):
+        return "task {} already exist! ".format(task_id)
 
 
 class TaskNotExist(Exception):
-    def __str__(self, ):
+    def __str__():
         return "task not exist! "
 
 
 class TaskInitError(Exception):
-    def __str__(self):
+    def __str__(task_id):
         return "task pramar invalid! key:str priority:0<int<1000000 data:dict"
 
 
 class TaskNotRunning(Exception):
-    def __str__(self):
-        return "task should be running but it in {} now"
+    def __str__(self, task):
+        return "task should be running but it in {} now".format(task.status)
 
 
 class NodeIdTypeError(Exception):
-    def __str__(self):
+    def __str__(nodeId):
         return "nodeId must be int!"
 
 
 class NodeIdNotMatch(Exception):
-    def __str__(self):
-        return "nodeId doesn`t match!"
+    def __str__(self, task_nodeId, nodeId):
+        return "nodeId doesn`t match! task nodeid = {} your node id = {}".format(task_nodeId, nodeId)
```

### Comparing `taskhub-0.7.0/taskhub/server.py` & `taskhub-0.7.1/taskhub/server.py`

 * *Files identical despite different names*

### Comparing `taskhub-0.7.0/test/test_serve.py` & `taskhub-0.7.1/test/test_serve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 import requests
 
 from taskhub.server import serve
 from retry import retry
-from loger import log
+
 import traceback
 
 
 def sync(task):
 
     back_end_url = "http://127.0.0.1/api/"
+
     @retry(tries=5, delay=1, backoff=1)
     def req(task):
         print(task)
         r = requests.post(back_end_url, json=task.get_dict())
         r.raise_for_status
         return r.json()
 
-    log("syncing...")
+    print("syncing...")
     try:
         r_data = req(task)
     except:
-        log("sync: req 时发生异常：{}".format(traceback.format_exc()), 1)
+        print("sync: req 时发生异常：{}".format(traceback.format_exc()), 1)
         return False
     else:
         if r_data.get("code") == 200:
-            log("synced!", 4)
+            print("synced!", 4)
             return True
         else:
-            log("sync: 返回状态异常：{}".format(r_data))
+            print("sync: 返回状态异常：{}".format(r_data))
             return False
 
 
-
 if __name__ == "__main__":
     serve(
-        port=2333, 
-        passwd="1qaz2wsx", 
-      sync=sync)
+        ip="127.0.0.1",
+        port=2333,
+        passwd="1qaz2wsx",
+        sync=sync)
```

