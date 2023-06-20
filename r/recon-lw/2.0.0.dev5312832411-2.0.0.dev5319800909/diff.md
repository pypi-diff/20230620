# Comparing `tmp/recon_lw-2.0.0.dev5312832411.tar.gz` & `tmp/recon_lw-2.0.0.dev5319800909.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/recon_lw-2.0.0.dev5312832411.tar", last modified: Mon Jun 19 14:05:25 2023, max compression
+gzip compressed data, was "dist/recon_lw-2.0.0.dev5319800909.tar", last modified: Tue Jun 20 07:35:57 2023, max compression
```

## Comparing `recon_lw-2.0.0.dev5312832411.tar` & `recon_lw-2.0.0.dev5319800909.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/
--rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-19 14:05:01.000000 recon_lw-2.0.0.dev5312832411/package_info.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw/
--rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/EventsSaver.py
--rw-r--r--   0 runner    (1001) docker     (122)     4942 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/LastStateMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/LiveObjectsCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/SequenceCache.py
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/StateSequenceGenerator.py
--rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/TimeCacheMatcher.py
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/recon_lw.py
--rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/recon_ob.py
--rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/recon_ob_cross_stream.py
--rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/recon_lw/recon_ob_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-19 14:05:25.000000 recon_lw-2.0.0.dev5312832411/test/
--rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-19 14:04:36.000000 recon_lw-2.0.0.dev5312832411/test/test_recon_ob.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/
+-rw-r--r--   0 runner    (1001) docker     (122)       69 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-06-20 07:35:30.000000 recon_lw-2.0.0.dev5319800909/package_info.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw/
+-rw-r--r--   0 runner    (1001) docker     (122)     1908 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/EventsSaver.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4936 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/LastStateMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2507 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/LiveObjectsCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2916 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/SequenceCache.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1108 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/StateSequenceGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3716 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/TimeCacheMatcher.py
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13503 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/recon_lw.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32984 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/recon_ob.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22143 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/recon_ob_cross_stream.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6018 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/recon_lw/recon_ob_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      294 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        9 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1582 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-20 07:35:57.000000 recon_lw-2.0.0.dev5319800909/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     4050 2023-06-20 07:35:00.000000 recon_lw-2.0.0.dev5319800909/test/test_recon_ob.py
```

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/EventsSaver.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/EventsSaver.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/LastStateMatcher.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/LastStateMatcher.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,21 +50,21 @@
             if key2 is not None:
                 stream_time = ts2
                 index_key = recon_lw.time_stamp_key(ts2) + "_" + key2
                 i = self._state_time_index.bisect_key_left(index_key)
                 current_len = len(self._state_time_index)
                 next_key = None
                 if i < current_len:
-                    next_key = recon_lw.time_stamp_key(self._state_time_index[i+1][0]) + "_" + \
-                               self._state_time_index[i+1][1]
+                    next_key = recon_lw.time_stamp_key(self._state_time_index[i][0]) + "_" + \
+                               self._state_time_index[i][1]
                 if i == current_len or index_key != next_key:
                     self._state_time_index.add([ts2, key2, order, o])
                     self._state_cache_add_item(ts2,key2)
                 else:
-                    rec = self._state_time_index[i+1]
+                    rec = self._state_time_index[i]
                     if order >= rec[2]:
                         rec[2] = order
                         rec[3] = o
 
         #flush
         if stream_time is not None:
             self._flush(stream_time)
```

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/LiveObjectsCache.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/LiveObjectsCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/SequenceCache.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/SequenceCache.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/StateSequenceGenerator.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/StateSequenceGenerator.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/TimeCacheMatcher.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/TimeCacheMatcher.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/recon_lw.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/recon_lw.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/recon_ob.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/recon_ob.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/recon_ob_cross_stream.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/recon_ob_cross_stream.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw/recon_ob_stats.py` & `recon_lw-2.0.0.dev5319800909/recon_lw/recon_ob_stats.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/recon_lw.egg-info/SOURCES.txt` & `recon_lw-2.0.0.dev5319800909/recon_lw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/setup.py` & `recon_lw-2.0.0.dev5319800909/setup.py`

 * *Files identical despite different names*

### Comparing `recon_lw-2.0.0.dev5312832411/test/test_recon_ob.py` & `recon_lw-2.0.0.dev5319800909/test/test_recon_ob.py`

 * *Files identical despite different names*

