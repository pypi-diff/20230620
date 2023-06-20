# Comparing `tmp/qps_limit-0.1.0-py3-none-any.whl.zip` & `tmp/qps_limit-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 4004 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       77 b- defN 23-Jun-19 02:45 qps_limit/__init__.py
--rw-rw-r--  2.0 unx     7483 b- defN 23-Jun-18 15:36 qps_limit/wrapper.py
--rw-rw-r--  2.0 unx     1646 b- defN 23-Jun-19 02:45 qps_limit-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-19 02:45 qps_limit-0.1.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-19 02:45 qps_limit-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx        1 b- defN 23-Jun-19 02:45 qps_limit-0.1.0.dist-info/zip-safe
-?rw-rw-r--  2.0 unx      547 b- defN 23-Jun-19 02:45 qps_limit-0.1.0.dist-info/RECORD
-7 files, 9856 bytes uncompressed, 3028 bytes compressed:  69.3%
+Zip file size: 4083 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       77 b- defN 23-Jun-20 12:14 qps_limit/__init__.py
+-rw-rw-r--  2.0 unx     8059 b- defN 23-Jun-20 11:41 qps_limit/wrapper.py
+-rw-rw-r--  2.0 unx     1636 b- defN 23-Jun-20 12:15 qps_limit-0.1.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-20 12:15 qps_limit-0.1.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-20 12:15 qps_limit-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx        1 b- defN 23-Jun-20 12:15 qps_limit-0.1.1.dist-info/zip-safe
+?rw-rw-r--  2.0 unx      547 b- defN 23-Jun-20 12:15 qps_limit-0.1.1.dist-info/RECORD
+7 files, 10422 bytes uncompressed, 3107 bytes compressed:  70.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: qps_limit/__init__.py
 Comment: 
 
 Filename: qps_limit/wrapper.py
 Comment: 
 
-Filename: qps_limit-0.1.0.dist-info/METADATA
+Filename: qps_limit-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: qps_limit-0.1.0.dist-info/WHEEL
+Filename: qps_limit-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: qps_limit-0.1.0.dist-info/top_level.txt
+Filename: qps_limit-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: qps_limit-0.1.0.dist-info/zip-safe
+Filename: qps_limit-0.1.1.dist-info/zip-safe
 Comment: 
 
-Filename: qps_limit-0.1.0.dist-info/RECORD
+Filename: qps_limit-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qps_limit/__init__.py

```diff
@@ -1,5 +1,5 @@
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 from .wrapper import MWrapper
 
 __all__ = ['MWrapper']
```

## qps_limit/wrapper.py

```diff
@@ -167,28 +167,33 @@
         func: Callable[..., Coroutine[Any, Any, Any]],
         params: Iterable[Tuple[Tuple, Dict]],
         num_workers: int = 1,
         worker_max_qps: float = None,
         streaming: bool = False,
         callback: Callable = None,
         progress: bool = True,
+        ordered: bool = True,
         verbose: bool = False
     ):
 
         self.func = func
         self.params = params
         self.num_workers = num_workers
         self.worker_max_qps = worker_max_qps
         self.streaming = streaming
         self.callback = callback
         self.progress = progress
+        self.ordered = ordered
         self.verbose = verbose
 
         self.workers = []
-        self.queue = multiprocessing.Queue()
+        if self.ordered:
+            self.dict = multiprocessing.Manager().dict()
+        else:
+            self.queue = multiprocessing.Queue()
         self.count_iterator, self.param_iterator = itertools.tee(self.params, 2)
         self.count = 0
         for _ in self.count_iterator:
             self.count += 1
 
         for mod in range(self.num_workers):
             self.workers.append(
@@ -219,34 +224,46 @@
                 max_qps=self.worker_max_qps,
                 max_workers=16 if not self.worker_max_qps else max(16, self.worker_max_qps),
                 callback=self.callback,
                 progress=self.progress
             )
             assert len(idxs) == len(results)
             for idx, res in zip(idxs, results):
-                self.queue.put((idx, res))
+                if self.ordered:
+                    self.dict[idx] = res
+                else:
+                    self.queue.put((idx, res))
         else:
             result_iterator = streaming_batch_run(
                 func=self.func,
                 params=param_iterator,
                 max_qps=self.worker_max_qps,
                 max_workers=16 if not self.worker_max_qps else max(16, self.worker_max_qps),
                 callback=self.callback,
                 progress=self.progress
             )
             for idx, res in zip(idx_iterator, result_iterator):
-                self.queue.put((idx, res))
+                if self.ordered:
+                    self.dict[idx] = res
+                else:
+                    self.queue.put((idx, res))
 
     def start(self):
         start_time = time.time()
         for worker in self.workers:
             worker.start()
         consume = 0
         while consume < self.count:
-            yield self.queue.get()
+            if self.ordered:
+                while consume not in self.dict:
+                    pass
+                yield (consume, self.dict[consume])
+                del self.dict[consume]
+            else:
+                yield self.queue.get()
             consume += 1
         assert consume == self.count
         end_time = time.time()
         if self.verbose:
             print('elapsed time: {:.2f}s average qps: {:.2f}/{:.2f}'.format(
                 end_time - start_time,
                 self.count / (end_time - start_time),
```

## Comparing `qps_limit-0.1.0.dist-info/METADATA` & `qps_limit-0.1.1.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qps-limit
-Version: 0.1.0
+Version: 0.1.1
 Summary: Run functions under any limited rate
 Home-page: https://github.com/antct/rate-limit
 Author: tt
 Author-email: 527892245@qq.com
 License: GPLv2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -61,15 +61,15 @@
 engine = MWrapper(
     func=func,
     params=params(),
     num_workers=10,
     worker_max_qps=10,
     streaming=False,
     callback=callback,
-    progress=True
+    progress=True,
+    ordered=True,
+    verbose=True
 )
 
-for i, r in engine.start():
-    print(i, r)
+for idx, r in engine.start():
+    print(idx, r)
 ```
-
-> elapsed time: 10.11s average qps: 98.96/100.00
```

